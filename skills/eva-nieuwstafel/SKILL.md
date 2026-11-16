---
name: "eva-nieuwstafel"
description: "Maakt een nieuwstafel-opzet voor Eva (NPO 1): gesprek over het nieuws van de dag met meerdere duiders, in het exacte dossierformat. Gebruik bij 'nieuwstafel over', 'tafelopzet', 'opzet nieuws van de dag', 'actueel blok' bij Eva."
---

# Eva — nieuwstafel opzet

Laad ook `eva-context` als die beschikbaar is (vaste duiders, dossiervreter). Dit format is afgeleid uit zes echte Eva-nieuwstafels (Ouwehand, Donald Pols, vakbonden, Iran-deal, geweld en politiek, asiel in het Catshuis) en uit hoe nieuwstafels uiteindelijk in het draaiboek kwamen (Albert Heijn-hack, dieseldeal + NAVO-speech, AI-tweets Jetten, Christa Pike + Catshuis + pest in Rusland, Haagse politiek, midterms). **Geen RTL-format: geen voice-over, geen los PR-tekstblok.**

**Doel: schrijf de opzet zo dat er na het overleg met presentator en hoofdredacteur zo min mogelijk herschreven hoeft te worden.** Dus al kort, al in Eva's stem, gebouwd op de stellingen van de gasten.

## Werkwijze
1. **Input checken**: onderwerp(en), tafel (welke duiders en betrokkenen, wie is bevestigd), duur in minuten met blokverdeling (vragen = minuten als bovengrens, per blok; ontbreekt de duur: neem 15 minuten en meld het).
2. **Dossier bouwen** (dossiervreter): wat er precies gebeurde vandaag, cijfers, wie wat zei, wat onbevestigd is, welke reacties de redactie nog moet opvragen. Alles met bron en datum.
3. **Rollen verdelen**: wie is de nieuwsbron of betrokkene, wie duidt Den Haag, wie is de dwarse stem, wie de expert. Elke gast krijgt een duidelijke functie en, uit het voorgesprek, een **stelling**.
4. **Blokken bepalen** met minuten, dan vragen schrijven.
5. **Controle**: loop de Eindcheck uit `eva-context` af (vragen per blok, korte doorvragen, 'jij zegt' en citeervragen, één lijn, fragmenten, iedere gast aan bod, cijfers, belangencheck) en meld de uitkomst in 3 regels onder de opzet. Volg voor stap 2 het Research-protocol uit `eva-context`.

## Skelet (exact zo, genummerd)
```
[KOP IN HOOFDLETTERS: gastnamen of thema, bv. VAKBONDEN OP RAMKOERS / IRAN-DEAL?! / ACTUEEL (POLITIEK) / NIEUWSTAFEL: CHRISTA PIKE - CATSHUIS - PEST IN RUSLAND]
1 Contact toevoegen
2 Naam redacteur
3 TITEL
Default
4 Aanleiding
[vaak leeg; anders 1 regel: vertrek X / debat over Y]
5 Wat inspireert, is nieuw en moet uit dit gesprek gehaald worden?
6 Opzet
TITEL GESPREK
[presentatie-intro]
PR PLAY 20 COMPLEET: [NAAM NIEUWSFRAGMENT]
([totaal] MIN - [blok] - [blok] - ...)
------ BLOKNAAM (X MIN)
[vragen]
------ BLOKNAAM (X MIN)
[vragen]
DANK & APPLAUS
7 TAKEOVER
TAKEOVER [kop]
ZUIL: [NAAM]  (4–7 zuilen)
8 DLS
[stills]
Graag aanvullen in het draaiboek :-)
9 PLAY Compleet
10 BETA MEELEES
11 OVERSTART
12 Voorgesprek [naam gast]
13 Voorgesprek [naam gast]
...
[Achtergrond / dossier]
[Voor het draaiboek]
```

## De presentatie-intro
- 40–70 woorden (in het draaiboek vaak rond de 50), hooguit 90 bij een ingewikkeld verhaal. Schrijf vanuit de kijker en diens portemonnee of verbazing ("daar zullen veel mensen van zijn geschrokken ... je bent meer dan 2000 euro kwijt"), niet vanuit de details van het bericht. Opent met de kern van het nieuws in een pakkende, concrete eerste zin, soms met een citaat uit de krant of een beeldspraak:
  - "Chaos bij de Albert Heijn. Prijskaartjes kloppen niet, boodschappen worden niet bezorgd en vrijwel alle distributiecentra liggen stil."
  - "Premier Jetten ligt opnieuw onder vuur vanwege het gebruik van AI in zijn uitingen op social media."
  - "Hij voerde dit weekend campagne op een plek waar hij zich normaal gesproken geen zorgen hoeft te maken."
  - "'Een duiventil vol ruzie en afsplitsingen', zo omschrijft de Telegraaf de Partij voor de Dieren vandaag."
  - "Het is bonje tussen de boze bonden en het kabinet."
  - "Nog geen maand geleden trok de overstap van Donald Pols ... voor opgetrokken wenkbrauwen. Gisteren begon hij aan zijn nieuwe baan. En vandaag is hij alweer ontslagen."
- Spelen met beeldspraak en woordgrappen mag ("kikkers in de kruiwagen houden", "wespennest"), maar de feiten moeten kloppen.
- Bewijs in de intro mag: een voorbeeld als DLS met de letterlijke tekst ("Het gaat bijvoorbeeld om dit bericht: DLS WESTERBORK").
- Eindigt bij voorkeur op een punchline ("...maar het signaal van Trump is glashelder: met Poetin kan hij zaken doen.", "En hij neemt geen halve maatregelen.") en dan `PR PLAY 20 COMPLEET: [NAAM]`. Liever geen vraag als slotzin.
- Live-situaties: "Op dit moment debatteert de Tweede Kamer over..." / "Op dit moment wordt er in het Catshuis topoverleg gevoerd..."

## Meerdere onderwerpen aan één tafel
Een nieuwstafel kan 2–3 onderwerpen hebben (bv. 9 - 6 - 7 MIN). Elk onderwerp krijgt:
- een eigen scheiding `--------------CATSHUISOVERLEG`
- een eigen TAKEOVER-nummer (200 / 300 / 400) en eigen PR PLAY-reeks (20 / 30 / 40)
- een korte overgang in Eva's spreektaal: "En dan iets heel anders, en dichter bij huis." / "Dan ander Haags nieuws:" / "En dan gaan we naar Rusland."
Gasten van andere items mogen meedoen ("@ Casper van Eijck, als arts, hoe luister je naar dit hele verhaal?").

## Fragmenten
- Genummerd per onderwerp (`PLAY 20`, `21`, ... / `30`, `31`, ...). Varianten: `PLAY COMPLEET`, `PLAY OVERSTART`, `PLAY MEELEES` (ondertitelde quote), `DLS [NAAM]`.
- Elke play wordt ingeleid met een korte overgangszin zonder @: "Dit is wat de CEO van Ahold vanmiddag zei tegen de NOS:" / "Dit is hoe Zelensky reageerde op de dieseldeal:" / "Zo reageerde premier Jetten vanmiddag na het gesprek:" / "Even kijken hoe ze allemaal reageerden."
- Onder de play: de kernquote (letterlijk of samengevat) tussen haakjes; bij Engels de vertaling. URL met timecode `(48:00 - 48:32)` als die bekend is.
- **Reacties van partijen die niet aan tafel zitten** als tekstblok: "Wij hebben de Rijksvoorlichtingsdienst gevraagd om een reactie en zij zeggen: '...'" / "Wij spraken een arbeidsrechtadvocaat en zij zegt: ..." / `--> reactie Tata Steel: ...`. Citaten uit regionale media of persberichten letterlijk, met DLS.
- Een gast die een fragment heeft aangedragen: "@ Hannah, jij wilde graag dit fragment laten zien:" / "@ Simon, waarom wil je hem laten zien?"
- Niet zelf gezien of geverifieerd: [ZOEKEN] met beschrijving van waar het te vinden is.

## Vragen
- Elke vraag begint met `@ [Naam], ...`. Vaste duiders met voornaam en 'je'. **De eerste vraag aan een nieuwe gast introduceert die met functie**: "@ Danny Mekić, tech-expert, ...", "@ Elif, jij bent journalist voor WNL, je hebt jarenlang in Den Haag rondgelopen. ...", "@ Koen Petersen, Amerikanist, liefhebber. Nog vier weken te gaan tot de midterms. Hoe staat het ervoor?", "@ Hans van den Heuvel, u bent voorzitter van de vakbond CNV en was vanmiddag bij het overleg aanwezig. Hoe was het?"
- Verwacht antwoord uit het voorgesprek tussen haakjes eronder, vooral bij de sleutelvragen.

### De 'jij zegt'-motor (belangrijkste les uit de draaiboeken)
De nieuwstafel draait op de stellingen die gasten in het voorgesprek innamen. Schrijf die als vraag uit:
- "@ Maarten, jij zegt: wij Europeanen moeten vooral in de spiegel kijken. Waarom?"
- "@ Jort, jij ziet nog een ander motief bij Trump voor deze deal, wat dan?"
- "@ Helga, jij denkt niet dat Trump alleen maar over de pest belt. Waarom?"
- "@ Hajar, toch zeg jij: ik ben bang dat cijfers er niet toedoen. Waarom niet?"
- "@ Toen wij u hierover belden vanochtend zei u: ik schaam me ervoor dat we hier een discussie over hebben. Waarom?"
- "@ Marieke, jij zei tegen mijn redacteur Maud: vergeet niet, Trump is een kunstenaar als het gaat om beeldvorming!"
- "@ Wouter, de kop boven jouw column vandaag was: '...'. Wat bedoel je daarmee?"
Geen voorgesprek? Laat de stelling open als `@ Hajar, jij zegt: XXX` en zet in de aandachtspunten welke stelling je van deze gast wilt hebben.

### De korte-vragenregel
- De eerste vraag over een onderwerp draagt de context. **De rest is kort**: "@ Wouter?", "@ Werkt dit?", "@ Kan Trump dat betalen?", "@ Simon, wat denk jij?", "@ Mats, waar kijk ik naar?", "@ Ron, wat vind jij?", "@ Heeft hij een punt?"
- Geen lange 'reactie?'-rondes langs de hele tafel; liever stelling → één tegenstem → door.
- Elke gast moet in elk groot blok minstens één keer aan bod komen.

### Toon en kickers
- Eva's spreektaal en ik-vorm: "@ Coks, ik denk dat iedereen de pest associeert met de middeleeuwen!", "@ Sarah, jij bent heel grappig, maar even serieus: wat is de weg terug?", "@ Simon, dan nu de hamvraag der hamvragen: ...", "@ Tom, wat is het nou? Deal or no deal?"
- Laat duiders hun eigen voorbeelden meebrengen: "@ Jij hebt de voorbeelden voor ons meegenomen."
- Persoonlijke haak: "@ Jort, ik begreep dat jij vanmiddag met Marianne Thieme aan het lunchen was toen dit nieuws naar buiten kwam?"
- **Persoonlijke kicker** aan het eind van een blok of tafel: "@ Jort, word jij nu zenuwachtig?", "@ Ron, gebruik jij eigenlijk AI voor je social media posts?", "@ Maarten, geweldig als je zo wordt aangekondigd?", "@ Heeft één van jullie nog iets hoopvols te melden op deze stralende Tweede Pinksterdag?"
- Slotvraag anders: vooruitblik ("gaan ze er onderling uitkomen?").
- Optionele vragen tussen dubbele haakjes `((@ ...))`; reservevragen tussen enkele haakjes `(@ Koen, ...)`. Ze tellen niet mee voor het maximum. `OF` tussen alternatieve fragmenten of vragen.
- Afsluiten met een luchtig fragment mag (`PLAY MEELEES: MACDONALDS`) en dan `DANK & APPLAUS`.

## Blokken
- Totaalduur met blokverdeling bovenaan: `(15 MIN)`, `(14 MIN - 5 - 5 - 4)`, `(18 MIN - 6 - 6 - 6)`, `(30 MIN - 5-9-4-4-6-2)`.
- Bloknamen kort en inhoudelijk: `WAAROM DEZE DEAL? 7 min`, `CAMPAGNESTUNTS 8 min`, `VVD (5 MIN)`, `BOX 3 (4 MIN)`, `EERSTE REACTIES`, `CIJFERS`, `JURIDISCH`, `SLOT`. Een scheiding zonder naam (`---------`) mag tussen deelvragen. Een harde overgang naar een tweede verhaal: `===== OVERSTAP =====`.
- Onthullingsverhaal: begin bij de bron of onthuller, reconstrueer wat er gebeurde, en ga daarna naar de bredere tafel (moraal, gevolgen, afrekening).

## 7 TAKEOVER
Een kop met een draai, vaak als vraag of woordspel: "DIESELDEAL: CADEAU VOOR POETIN?", "ALBERT HEIJN GEHACKT?", "OPTIMISME IN CATSHUIS?", "PANIEK IN RUSLAND?", "TRUMP SLAAT OM ZICH HEEN". Plus 4–7 `ZUIL: [NAAM]`: de hoofdrolspelers over wie gepraat wordt.

## 8 DLS
Alle mensen en beelden die genoemd worden, één per regel. Groepeer bij politiek (`Kabinet`, `Coalitie`, `Oppositie`, `Polder`, `Kamer`, `Uitvoering`, `Overig`). Screenshots van posts en reacties als aparte DLS ("Reactie L1", "Trump Truth Social EU"). Aanwijzingen en bron-URL erbij waar nodig. Afsluiten met `Graag aanvullen in het draaiboek :-)`.

## 12+ Voorgesprekken
Per gast een kop `Voorgesprek [Naam] ([redacteur])`. Minne voert en schrijft ze zelf. Claude levert per gast **aandachtspunten**: welke stelling we van deze gast willen (dat wordt de 'jij zegt'-vraag), wat te checken, welk fragment of voorbeeld ze zelf willen meenemen, waar ze tegenover een andere gast staan, en een persoonlijke haak voor een kicker. Sluit per gast af met `Opstelling:` (in één regel de verwachte positie aan tafel), als die bekend is.
Belstatus hoort in veld 4 Aanleiding, als `Bellijst:` met `Wat kan:` / `Staat uit:` / `Niet:` en de redacteur tussen haakjes. Meld per gast ook de choreografie als die afwijkt (komt pas in blok 2 binnen, luistert eerst).

## Achtergrond
Het dossier van de dag: tijdlijn, kerncitaten, cijfers met bron, relevante artikelen met kop `MEDIUM - DATUM`. Wat onbevestigd is: expliciet markeren.

## Voor het draaiboek
Lever dit mee, zodat het overleg sneller gaat:
- **TITEL per gast** (onderschrift), exact zo: regel 1 voornaam, regel 2 achternaam, regel 3 `functie // over X // over Y`. Voorbeeld: `Maarten` / `van Rossum` / `oud-diplomaat en toponderhandelaar // over de diesel-deal tussen de VS en Rusland // over Donald Trump`. Bij meerdere onderwerpen per gast alle onderwerpen noemen.
- **TAKEOVER-kop** per onderwerp (zie boven).
- **Teaser** voor promo en live teaser, 1–2 zinnen: "Chaos bij de Albert Heijn. Door een mogelijke cyberaanval wordt het steeds lastiger om alle supermarkten nog te bevoorraden: lege schappen dreigen."
- **Cold-open-regel**, een halve zin: "Lege schappen bij de Albert Heijn?", "Paniek in Rusland".
- **Leadertekst**, 2–4 woorden: "Woede om diesel-deal", "De tweets van Jetten".
- **Intro-regel** voor 'Wat heb ik voor jullie vanavond?', 1–2 zinnen.

## Lessen uit de draaiboeken (sep–nov 2026)
Gebaseerd op vier directe opzet-draaiboekvergelijkingen (Belastingplan, Zorgpremie, Schuiling, De Mos) en negen nieuwstafels in het draaiboek.
- **Eén lijn**: nieuws -> waarom -> wat schuurt -> wat nu. Een montage als concept, een lange tussenpresentatie, een reconstructieblok of een apart analyseblok (beeldvorming) haalden het draaiboek niet. Een reconstructie wordt één vraag: "Kun jij nog even kort uitleggen waar deze zaak om draait?"
- **Vaste opener: het laatste nieuws aan de Haagse duider of de betrokkene.** "@ Eerst even het laatste nieuws: Wouter, wat weten we?" / "@ Wouter, wat is de laatste stand van zaken?" / "@ Laila, hoe is de stemming in het Witte Huis op dit moment?" / "@ Marcel, was je geschrokken toen je het nieuws hoorde vandaag?"
- **Per fragment**: één inleidende zin, het fragment, één korte reactievraag aan één persoon, eventueel één tegenstem ("@ Hajar, heeft Bennie gelijk?"). Hooguit 3 à 4 fragmenten per 13-18 minuten; de rest als reserve.
- **"@ Tafel, wat denken jullie?"** bestaat, maar hooguit 2 à 3 keer in een lang blok.
- **Stelling als emotie**: "En dat maakt jou heel boos, waarom?" werkt naast de letterlijke 'jij zegt'. Bied bij elke 'jij zegt' ook die korte variant aan.
- **Eva als stem van de kijker**: "Dus iedereen thuis zit te kijken en denkt: ...", "Heel veel mensen zullen nu denken: had die boete maar betaald.", "Hoe moet ik dat met elkaar rijmen?"
- **Citaat van iemand die niet aan tafel zit**: Eva leest het voor in de vraag, met "ik citeer"; daar is geen fragment voor nodig.
- **Wederhoor als voorgelezen tekst**: "Wij hebben vandaag gebeld met [naam]. Een woordvoerder liet weten..." / "Zijn advocaten laten aan ons weten dat..."
- **Politicus aan tafel** krijgt de meeste vragen, met korte doorvraag: "Hebben ze tegen u gezegd hoe ze dit gaan betalen? / Heeft u dat gevraagd?"
- **Uitleg-expert** krijgt basisvragen voor de kijker: "wat is een patch?"
- **Peiler aan tafel**: cijfers als `GRAPH` met exacte percentages in de tekst.
- **Column of eerdere uitspraak van de duider met datum**: "Wouter, jij schreef op 24 augustus al in je column..." / "gisteren zei jij hier aan tafel..."
- **Gast van een ander item** krijgt een vraag in het nieuwsblok (minister in het slot, arts bij het zorgnieuws, oud-politiechef bij de rechtszaak).
- **Slot**: de vervolgstap of meest waarschijnlijke uitkomst als opdracht of vraag: "Geef mij even een routekaart voor de komende 24 uur." / "Joost, wat is de meest waarschijnlijke uitkomst van deze week?" / "zou u adviseren om in cassatie te gaan?" Of een samenvattende stelling + "Wat vind je hiervan?". Een slotnotitie voor de regie mag: "Optimistisch eindigen".
- **Overgangszinnen**: "We gaan er een schep bovenop doen." / "Laten we wat beter naar die deal kijken." / "Laten we even naar de nabije toekomst kijken."
- **Zuilen**: lever de hoofdrolspelers (4–7); het draaiboek vult op een grote politieke dag zelf aan tot 14 of meer.
- **Tafel kan nog wisselen**: schrijf vragen op rol (jurist, verslaggever uit de zaal, Haagse duider) zodat ze overeind blijven als een andere gast aanschuift.