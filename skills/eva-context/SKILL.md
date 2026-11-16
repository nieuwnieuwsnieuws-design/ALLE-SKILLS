---
name: "eva-context"
description: "Werkcontext voor Minne als redacteur bij talkshow Eva (NPO 1): programma, toon, vaste duiders, dossiervreter. Gebruik bij elk Eva-werk: opzet, gast, item, vanavond, duider, dossier, tafel."
---

# Eva — werkcontext

Minne is redacteur bij **Eva**, de talkshow van Eva Jinek op NPO 1 (AVROTROS, productie MediaLane), live vanuit De Hallen (Kinkerstraat, Amsterdam). Dit is het fundament onder alle Eva-skills. **Er is geen RTL Tonight-format meer.** Nooit een voice-over-blok, nooit een RTL-intro-sjabloon, nooit 'PR-tekst + VO' als losse onderdelen.

## Programma en toon
- Actualiteiten én cultuur, sport, muziek en human interest. Journalistiek scherp, maar warmer, persoonlijker en informeler dan een late-avond nieuwsshow.
- Eva spreekt in de eerste persoon en brengt zichzelf in: haar eigen tafel ("Maarten van Rossum heeft hier bij mij aan tafel gezegd..."), haar eigen verleden ("Ik heb ook heel lang bij de NOS gewerkt"), haar eigen reactie ("Ik zou geïntimideerd zijn!", "Ik vond het ontroerend"), haar redactie ("jij zei tegen mijn redacteur Maud...").
- Ruimte voor emotie, humor en het menselijke verhaal, nooit ten koste van de feiten.
- Redactievergadering elke werkdag 09:00. Opzetten worden vaak door 2–4 redacteuren samen gemaakt (veld 'Naam redacteur').

## Van opzet naar uitzending
Workflow: Minne (vaak met collega's) maakt de opzet → overleg met presentator en hoofdredacteur → het wordt het stuk in het draaiboek. De opzet moet dus zo dicht mogelijk bij het draaiboek liggen. Wat er in dat overleg gebeurt (afgeleid uit draaiboeken oktober 2026):
- **Vragen worden korter.** De eerste vraag over een onderwerp draagt de context; de rest is kort: "@ Wouter?", "@ Werkt dit?", "@ Kan Trump dat betalen?", "@ Wat deed dit met jou?", "@ Moeilijk om te spelen?"
- **'Jij zegt'-stellingen uit het voorgesprek blijven staan** en dragen het gesprek: "@ Maarten, jij zegt: wij Europeanen moeten vooral in de spiegel kijken. Waarom?"
- **Lange ping-pongrondes en meerdere 'reactie?'-vragen verdwijnen.**
- **Eva's eigen stem komt erbij**: ik-zinnen, uitroepen en stellingen in plaats van vragen ("@ Je hebt je niet ingehouden!").
- **Persoonlijke kickers blijven**: een luchtige, persoonlijke vraag aan het eind van een blok ("@ Ron, gebruik jij eigenlijk AI voor je social media posts?", "@ Jort, word jij nu zenuwachtig?").
- Achtergrond en verwachte antwoorden verdwijnen grotendeels; alleen het verwachte antwoord bij een sleutelvraag blijft staan.

## Draaiboek in vogelvlucht
A promo (opgenomen 18:15) → B live teaser (18:55) → C cold open → D intro ("Goedenavond, welkom allemaal! Welkom in De Hallen! Wat heb ik voor jullie vanavond?") → E, F, G... items → afkondiging. Itemtypes: nieuwstafel (soms met 2–3 onderwerpen), een-op-een, opkomst + gesprek + optreden (muziek), live schakeling, opgenomen gesprek. Per item: TAKEOVER-kop, zuilen, TITELS per gast, PLAY Compleet, OVERSTARTS, DLS. Nummerreeksen per item (bv. item E: PLAY 20-reeks, TAKEOVER 200, DLS 250-reeks; item F: 50-reeks / 500; item G: 80-reeks / 800).

## Rol van Minne
Nieuws volgen, gasten bellen en briefen, items voorbereiden, vragen en presentatieteksten schrijven, beeld zoeken (DLS, fragmenten), meedenken in de vergadering.
- Voorgesprekken voert en schrijft Minne altijd zelf. Claude levert aandachtspunten per gast, nooit een verzonnen voorgesprek.
- Lengte: reken met de duur in minuten. **Vragen = minuten, als bovengrens en per blok** (blok van 4 min = hooguit 4 vragen). Definitieve draaiboeken zitten op 0,8 tot 1,0 vraag per minuut. Optionele vragen tussen dubbele haakjes tellen niet mee. Ontbreekt de duur: vraag die, of neem 13 minuten bij een een-op-een en 15 bij een nieuwstafel en meld dat.
- Definitief beeld vult ze aan in het draaiboek.

## Twee gesprekstypes
| Type | Wat | Skill |
|---|---|---|
| Een-op-een | Eén hoofdpersoon de diepte in: bewindspersoon, opgestapte partijleider, premier, insider, sporter, auteur, artiest | `eva-een-op-een` |
| Nieuwstafel | Het nieuws van de dag met meerdere duiders/betrokkenen | `eva-nieuwstafel` |

Beide gebruiken hetzelfde genummerde dossierskelet (1 Contact toevoegen → 2 Naam redacteur → 3 TITEL → 4 Aanleiding → 5 Wat inspireert → 6 Opzet → 7 TAKEOVER → 8 DLS → 9 PLAY Compleet → 10 BETA MEELEES → 11 OVERSTART → 12+ Voorgesprek(ken) → Achtergrond), plus een blok 'Voor het draaiboek'. Het volledige format staat in die skills.

## Vaste duiders (seizoen 2, gemeten: 137 afleveringen, sep 2025 – jun 2026)
Vaste kern: Wouter de Winther 56× (Haagse politiek, De Telegraaf) · Tom van 't Einde 33× (buitenland, VS) · Maarten van Rossum 30× (oud-diplomaat en toponderhandelaar; geopolitiek, VS) · Jort Kelder 24× (economie, elite, dwarse blik) · Ron Fresen 19× (Den Haag, oud-NOS) · Hajar Yagkoubi 18× · Helga Salemon 17× (Rusland) · Joost Vullings 16× (politiek) · Veerle Hammerstein 14× (strafrechtadvocaat) · Rozemarijn Lubbe 13×.
Daarna o.a.: Simon den Haak (campagnestrateeg), Eva Brandemann, Laila Frank (Amerika), Frank van Leeuwen, Splinter Chabot, Marleen de Rooy, Coks Donders (historicus, koningshuis), Huib Modderkolk (tech/veiligheid), Peter Pannekoek, Pieter Klok, Mats Akkerman (WNL), Beatrice de Graaf, Robbert Dijkgraaf, Marcel Levi (zorg), Alexander Klöpping.
Ook gezien in seizoen 3: Elif Isitman (WNL), Sarah Bakker (PowNed), Danny Mekić (tech), Koen Petersen (Amerikanist), Marieke de Vries (oud-correspondent VS).
- Gemiddeld 6 gasten per aflevering; kleine vaste duidersclub, daaromheen veel eenmalige gasten.
- Politici komen selectief aan tafel. Verwar nooit 'aan tafel' met 'besproken als onderwerp'.
- Tafelgasten worden over items heen ingezet: de arts van het volgende item reageert op een nieuwsonderwerp ("@ Casper van Eijck, als arts, hoe luister je naar dit hele verhaal?").
- Seizoen 3 loopt sinds 29 augustus 2026: check bij twijfel of een duider nog vast is. Bron: de sheet 'EVA' in Google Drive, tabbladen 'ARCHIEF S3' (wie zat wanneer bij welk onderwerp) en 'DESKUNDIGEN' (duiders per expertise). Kijk daar voordat je een duider voorstelt.
- In draaiboeken van sep-nov 2026 gezien: Wouter de Winther, Hajar Yagkoubi, Joost Vullings, Ron Fresen, Elif Isitman, Sarah Bakker, Mats Akkerman, Simon van Teutem (politicoloog), Rozemarijn Lubbe (opiniepeiler), Splinter Chabot, Jort Kelder, Maarten van Rossum, Laila Frank, Coks Donders, Marcel Levi, Danny Mekić, Huib Modderkolk, Veerle Hammerstein, Richard Korver (strafrechtadvocaat), Wim Voermans.

## Dossiervreter
Proactief, ook ongevraagd: per grote nieuwsgebeurtenis een gefactcheckt dossier met vaste kop:
1. Wat er precies gebeurd is (feiten met bron en datum)
2. Kerncijfers
3. Betrokkenen
4. Waar het schuurt / wie het bestrijdt
5. Wat nog onbevestigd is (expliciet markeren)
6. Welke Eva-duiders erbij passen
Elke claim herleidbaar naar een bron. Dit voedt de intro en de Achtergrond van een opzet én de redactievergadering.

## Werkafspraken
- Nederlands. Essentie eerst. Buitenlandse gast: vragen in het Engels, presentatieteksten in het Nederlands.
- Lever een opzet als platte tekst die Minne direct in het dossiersysteem kan plakken, tenzij ze om een document vraagt.
- Feiten altijd checken (web), datum in de bron noemen. Wat niet geverifieerd is: [CHECK].
- Fragmenten die Claude niet zelf heeft gezien: [ZOEKEN] met beschrijving waar het waarschijnlijk te vinden is.
- Vragen die de gast citeren (iets wat die eerder zei, in een interview, boek of voorgesprek) en dan laten uitweiden: altijd een paar in elke opzet.
- Presentatieteksten eindigen bijna nooit op een vraag; liever op een punchline ("Eén ding wist je altijd zeker: Gerri Eickhof is erbij."). Dit geldt niet voor de vragen zelf. Het programma zet er in het draaiboek soms toch een vraag achter ("kan de VVD hiermee leven?"); lever zelf de punchline.
- Twijfel markeren: alles wat niet geverifieerd of onzeker is krijgt [CHECK]. Dat zijn de rode markeringen: in een Google Doc echt rood kleuren, in platte tekst blijft het [CHECK]. Een omstreden cijfer of nuance zet je direct onder de vraag waar het in zit, niet alleen in de Achtergrond: wat in de Achtergrond staat, haalt het draaiboek niet.
- Voorgesprekken uitwerken (opname of aantekeningen van Minne): structuur van het gesprek behouden, lopende tekst, antwoorden in de ik-vorm van de gast, niets invullen wat er niet staat, partijnamen laten staan zoals gezegd ('Pro', niet 'PvdA'), twijfelwoorden [CHECK]. Volledig uitgetypt in de chat.

## Research-protocol (voor elke opzet)
Graaf diep; een dunne research is de vaakst gehoorde klacht. Minimaal:
1. **Het nieuws van vandaag**: 3 of meer zoekrondes, primaire bron erbij (Kamerbrief, persbericht, uitspraak, rapport), datum bij elke claim.
2. **Eigen woorden van elke gast**: recente interviews, columns, boek, socials, eerdere optredens bij Eva. Doel: minstens 3 letterlijke citaten met bron en datum, voor de citeervragen.
3. **Kamer en debat**: bij politieke onderwerpen de `debatten`-koppeling gebruiken (search_transcripts, get_transcript) voor letterlijke uitspraken van Kamerleden en bewindspersonen, met datum en debat.
4. **Tegenstem**: wie bestrijdt dit, met citaat. En de wederhoor die de redactie nog moet opvragen.
5. **Cijfers**: elk getal uit twee bronnen of met [CHECK]; noteer of een cijfer omstreden is.
6. **Beeld**: per fragment waar het staat (programma, datum, timecode) of [ZOEKEN].
7. **Belangencheck**: heeft een gast een belang of een band met een bron (partner schreef het stuk, eigen medium onthulde het, partij in de zaak)? Meld het in de aandachtspunten en stel voor hoe Eva het benoemt.
8. **Claims uit het voorgesprek natrekken**: functies, jaartallen, cijfers en toeschrijvingen die de gast noemde. Fouten melden in de aandachtspunten.

## Wat het overleg met een opzet doet (zes directe vergelijkingen, sep-nov 2026)
Vergeleken: Belastingplan, Berendsen + Van Rossum, Zorgpremie, Schuiling, De Mos + Fresen (nieuws) en Lex Paleaux (een-op-een). Schrijf de opzet meteen zo:
- **Eén lijn per gesprek.** Een raamwerk-opener met bijpassend slot, een montage als concept, een tweede analyseblok of een tweede onderwerp haalden het draaiboek niet. Kies de lijn nieuws -> waarom -> wat schuurt -> wat nu.
- **Kijkersperspectief als vraag**: "Heel veel mensen zullen nu denken: had die boete maar betaald." / "Veel mensen die nu kijken zullen denken: ... hoe is dat in godsnaam mogelijk?"
- **Eva's eigen verbazing of boosheid**, soms in hoofdletters voor nadruk: "IEDER JAAR WEER", "Hoe moet ik dat met elkaar rijmen?", "waarom zijn we hier niet veel bozer over?", "ik begrijp het niet zo goed. Waarom doet hij dit?"
- **Citeervraag en 'jij zegt' kort en letterlijk.** Die blijven staan, soms aangescherpt met een conclusie als stelling ("Kortom: de belangen van Europa worden niet behartigd. Dat is de conclusie."). Lange of grappige quotes sneuvelen vaker.
- **Kritiek loopt vaak via duider, fragment of kijker**, minder via een rij confrontatievragen aan de gast zelf.
- **Beeldspraak als drager van een politieke vraag sneuvelde** ('rechtse boyband', 'open huwelijk'). Lichte humor in een opener komt wel voor ("Er waren geen koekjes bij.").
- **Jargon en insidergrappen uitschrijven voor de kijker**: naam + functie voluit.
- **Aanspreekvorm consequent**: 'u' bij een bewindspersoon in elke vraag.
- **Fragmenten: 3 à 4 per 13-18 minuten.** Meer leveren mag, als reserve gemarkeerd. Elk fragment: één inleidende zin, daarna één korte reactievraag aan één persoon.
- **Verwachte antwoorden**: hooguit 3 per gesprek, in trefwoorden.
- **Lege aanspreekregel** als reactiemoment mag: "@ Tom Berendsen,".
- **Blokminuten erbij**: "(14 min) 6 - 5 - 3".
- **"AC:"** staat in het draaiboek voor een autocue-overgangszin naar een fragment; in de opzet volstaat de zin zelf.
- **Gast van een ander item** krijgt een vraag in het nieuwsblok.
- Het overleg voegt vooral korte doorvragen toe ("@ Richard, voelt het zoet?", "@ Hajar, wat denk jij?").

## Dossierkaart in Tinkerlist
De veldnamen zijn leidend, de nummers verschillen per kaart. Gezien: Contact toevoegen, Naam redacteur, TITEL, Aanleiding, Wat inspireert, Opzet, TAKEOVER, DLS, BEELDLIJST (lijst PLAY COMPLEET + lijst OVERSTARTS, met URL en timecode), Voorgesprek per gast. De bellijst staat vaak in Aanleiding: `Bellijst:` met `Wat kan:` / `Staat uit:` / `Niet:` en de redacteur tussen haakjes. Voorgesprekken staan er volledig uitgeschreven in, als vraag en antwoord, gast in ik-vorm, met vooraf één zin over hoe de gast praat.

## Voor het draaiboek: promo, cold open, leader (gezien in 6 draaiboeken)
- Promo en live teaser: 2 à 3 onderwerpen, elk 1 à 2 zinnen, gescheiden door een losse regel `EN`. Eerste onderwerp vaak een tegenstelling: "Goed nieuws: ... Het slechte nieuws: ..."
- Cold open: één zin met alle onderwerpen: "Het rommelt binnen de VVD, het Beter Leven-keurmerk werkt niet EN James Blunt zingt 'Goodbye My Lover'!"
- Leadertekst: per onderwerp 2 à 4 woorden of de gastnaam ("Deal splijt coalitie").
- Takeover-kop: feitelijk en kort, vaak alliteratie of vraag: "BOETE VOOR BURGEMEESTER", "WIE KRIJGT DE SCHULD?", "DEAL SPLIJT COALITIE", "OH OH DEN HAAG".

## Andere itemtypes (nog geen eigen skill; gebruik dit stramien)
- **Opkomst + gesprek + optreden** (muziek): `6000 OPKOMST SG INTRO LOS`, PR-intro met 2 à 3 fragmenten en DLS inline, eindigend op "Hier is [naam]!", dan `TITEL BEELDVULLEND`, `PLAY GELUID`, `OPKOMST`, duur als "(11 MIN TOT ZINGEN)". Gesprek afgewisseld met `OPTREDEN AAN TAFEL: ... (1'07 MIN)` of `SPELEN: ...`. Slot: Eva stuurt de artiest naar het podium, kondigt tour of album aan, optreden op podium is een eigen item.
- **Kort actueel met één expert** (6-9 min): wat weten we -> wie zit erachter -> hoe werkt het -> wat als het erger wordt -> wat kunnen wij doen. Eén concreet detail of vergelijking per vraag ("dertien Eiffeltorens op elkaar").
- **Human interest met twee gasten**: beurtelings per gast, Eva vertelt zelf de zware feiten en vraagt naar het vervolg, benoemt gevoel ("Het lijkt me zo moeilijk dat je hier niks van wist."), slot "voor mensen die nu kijken, wat wil jij dat ze weten?". Triggerwarning-regel met hulplijn waar nodig.
- **In memoriam-tafel**: korte stellingen zonder vraagteken, per gast "hoe leerde je haar kennen / wat betekende ze", veel fragmenten, slot "wat is haar erfenis?" en voorlezen.
- **Uitkomst nog onbekend** (uitspraak, stemming, uitslag): lever intro, eerste vragen, takeover, teaser en cold open in twee varianten (A/B) en zet `AANVULLEN NA [moment]` waar het antwoord moet komen.

## Eindcheck (afvinken en in 3 regels melden onder de opzet)
1. Vragen per blok niet meer dan de blokminuten; totaal geteld en vermeld.
2. Ongeveer de helft van de vragen is een korte doorvraag (2-10 woorden).
3. Minstens 3 citeervragen of 'jij zegt'-vragen, letterlijk, met bron in de Achtergrond.
4. Eén lijn: geen tweede onderwerp of dubbel concept.
5. Minstens één kijkersperspectief-vraag en één Eva-ik-zin.
6. Fragmenten: hooguit 4 in de lijn, rest als reserve; elk met vindplaats of [ZOEKEN].
7. Elke gast komt in elk groot blok aan bod; aanspreekvorm consequent.
8. Elk cijfer, elke naam en functie gecheckt of [CHECK]; omstreden cijfers gemarkeerd bij de vraag.
9. Belangencheck gedaan; claims uit voorgesprek nagelopen.
10. Intro op lengte (nieuws 40-70 woorden, portret 80-150) en eindigend op een punchline.