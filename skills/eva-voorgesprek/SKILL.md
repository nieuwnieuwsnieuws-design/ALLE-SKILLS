---
name: "eva-voorgesprek"
description: "Werkt een opgenomen voorgesprek (audio of ruw transcript) voor talkshow Eva uit tot een leesbaar vraag-antwoordstuk in de ik-vorm van de gast. Gebruik bij 'voorgesprek met', 'werk dit voorgesprek uit', 'transcribeer', 'idem' + naam, of een geüploade opname."
---

# Eva — voorgesprek uitwerken

Minne voert zelf telefonische voorgesprekken met gasten en duiders en neemt ze op (meestal `Record_online-voice-recorder.com_[N].mp3`). Deze skill maakt daar een uitwerking van die hij direct in het veld 'Voorgesprek [naam]' van de Tinkerlist-kaart kan plakken. Laad ook `eva-context` als die beschikbaar is.

**Kernregel: dit is transcriberen, niet schrijven.** Niets verzinnen, niets aanvullen, niets 'verbeteren' naar wat je verwacht. Alleen invullen wat overduidelijk uit de context volgt.

## Werkwijze
1. **Bestand vinden.** Zoek de opname zelf op (uploads of attachments). Bij meerdere opnames op één dag loopt de nummering op in de volgorde van de gesprekken. Zegt Minne alleen 'idem' + een naam: pak de eerstvolgende nog niet uitgewerkte opname en lever in exact dezelfde vorm als de vorige. Vraag niets wat je zelf kunt vinden.
2. **Transcriberen** (zie Techniek). Check de duur met ffprobe en vergelijk die met het laatste tijdstip in het transcript; meld gaten.
3. **Sprekers scheiden.** De opname heeft geen sprekerlabels. Leid af wie wat zegt uit inhoud en volume (Minne klinkt hard, de gast zachter via de telefoon). Waar dat onzeker is: markeren.
4. **Uitwerken** in het vaste format hieronder.
5. **Controleren**: elke naam, elk getal en elke partij staat er zoals het gezegd is; elke twijfel is gemarkeerd; niets toegevoegd.

## Techniek (wat betrouwbaar werkte)
- `pip install --break-system-packages -q faster-whisper` als het ontbreekt.
- Direct een mp3 aan faster-whisper geven mislukte soms stil (wel 'klaar', geen tekst). Zet daarom altijd eerst om: `ffmpeg -v error -y -i "$F" -ac 1 -ar 16000 -f f32le audio.raw`, laad met `numpy.fromfile('audio.raw', dtype=numpy.float32)` en geef die array aan `WhisperModel.transcribe()`.
- Model: `WhisperModel('large-v3-turbo', device='cpu', compute_type='int8', cpu_threads=2)`; `language='nl'`, `beam_size=5`, `vad_filter=True`.
- `initial_prompt`: één zin met programma, gast en onderwerp plus de namen en termen die waarschijnlijk vallen (bv. "Voorgesprek van talkshow Eva met Wouter de Winther over het belastingplan, amendementen, Pro, VVD, CDA, D66, JA21"). Schrijf partijnamen daarin zoals ze nu heten: **Pro**, nooit 'PvdA' of 'GroenLinks-PvdA'.
- Schrijf per segment `[mm:ss] tekst` weg naar een bestand en flush per regel. Draai lange opnames op de achtergrond en lees het bestand daarna.
- Onverstaanbaar of weggevallen stuk: knip dat deel los, normaliseer (`highpass`, `dynaudnorm`) en transcribeer het opnieuw, eventueel met `vad_filter=False` of het model `large-v3`. Blijft het onverstaanbaar: zo melden, niet raden.

## Format van de uitwerking
```
## Voorgesprek [Naam gast]

**[Vraag of onderwerp van Minne, kort en in volzin]**

[Antwoord van de gast in lopende tekst, in de ik-vorm van de gast.]

**[Volgende vraag]**

[Antwoord.]

### Let op
- [twijfelstukken, met tijdstip]
- [sprekertoewijzing die onzeker is]
- [claims van de gast die nog gecheckt moeten worden]
```
Regels:
- **Structuur van het gesprek behouden**: zelfde volgorde, vraag-antwoord. Niet thematisch herordenen, niet samenvatten.
- **Vragen van Minne vetgedrukt**, kort en opgeschoond. **Antwoorden van de gast niet vet, in de ik-vorm** ("Toen ik het hoorde, was het een feest van herkenning"), nooit "X merkt op" of "hij vindt".
- **Lopende tekst** in goede volzinnen, geen opsommingstekens. Stopwoorden, herhalingen en valse starts mogen weg; woordkeus, toon en typische uitdrukkingen van de gast blijven staan, want daar komen de 'jij zegt'-vragen uit.
- **Niets weglaten wat inhoud heeft**: ook praktische afspraken (beschikbaarheid, tijdstip, wat de gast wil laten zien, wat gevoelig ligt of niet op tv mag) horen erin.
- Boven de uitwerking in het antwoord: één of twee zinnen met de kern (wat is de stelling van de gast, wat is weggevallen of onzeker). Geen verdere analyse, tenzij gevraagd.
- Lever **altijd volledig uitgetypt in de chat**, zodat het direct te kopiëren is.

## Namen en partijen
- Partijnamen staan er zoals ze gezegd zijn. **Altijd 'Pro', nooit 'PvdA'.** Niet omzetten naar een naam die je verwacht.
- Namen die fonetisch doorkomen (bv. 'Roosmarijn', 'Vloer Bremer'): vergelijk met de gastenlijst en vaste duiders uit `eva-context`. Alleen corrigeren als het overduidelijk dezelfde persoon is; anders markeren.
- Cijfers, data en functies: overnemen zoals gezegd. Een vermoedelijke fout van de gast niet stil herstellen maar onder 'Let op' zetten.

## Twijfel markeren
- In de chat kan geen kleur. Markeer een twijfelwoord, -naam of -passage daar als `[?zo gehoord]`, bv. `Rijnda [?zo gehoord]`. Een weggevallen of onverstaanbaar stuk: `[onverstaanbaar 00:19–00:49]`.
- Zit er echte twijfel in (meer dan een enkele naam): zet dezelfde uitwerking er ook bij als **Google Doc met die passages in rood**, zodat Minne in één oogopslag ziet wat hij moet nabellen. Is Google Docs niet gekoppeld: meld dat en lever een doc waar rood wel kan.
- Onder 'Let op' staat elk twijfelstuk nog één keer, met tijdstip.

## Varianten (alleen op verzoek)
- **Lopend verhaal**: geen vragen, één doorlopende tekst in de ik-vorm van de gast (gebruikt bij een kort belletje met een woordvoerder). Sluit af met de openstaande punten: wat is toegezegd, wie belt wie terug.
- **Uitgebreid**: vóór de uitwerking een samenvatting in één zin, 3–5 bruikbare 'jij zegt'-stellingen in de letterlijke woorden van de gast, en een factcheck van de claims (wat klopt, wat niet te verifiëren is, met bron en datum). Daarna de volledige uitwerking.
- **Met tijdcodes en sprekerlabels** (M voor Minne, eerste letter van de gast): het ruwe, opgeschoonde transcript.
Zegt Minne niets over de variant: lever het standaardformat.

## Niet doen
- Geen introductie over wie de gast is of wat het item wordt, tenzij het in de opname gezegd is.
- Geen vragen of antwoorden reconstrueren uit een weggevallen stuk.
- Geen voorgestelde gespreksopbouw, quotes of webbronnen toevoegen aan het standaardformat; dat hoort bij de opzet (`eva-nieuwstafel`, `eva-een-op-een`) of bij de variant 'Uitgebreid'.
- Wat na het ophangen nog op de opname staat (Minne tegen een collega): apart onder een kopje 'Na het gesprek', niet door het voorgesprek heen.