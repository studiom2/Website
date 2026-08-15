# STUDIO M2 VLOEREN — MASTERPLAN

Dit document is de centrale source of truth voor het project. Besluiten, statussen, open vragen en de actieve taak worden hier bijgehouden voordat werk buiten de vastgelegde scope start.

## 0. Document control

| Veld | Waarde |
| --- | --- |
| Versie | 0.1.0 |
| Datum | 2026-08-15 |
| Projectstatus | DISCOVERY |
| Huidige actieve taak | M2-DISC-001 + M2-DISC-002 |

Statuswaarden in dit document: `DONE`, `READY`, `ACTIVE`, `BLOCKED` en `TODO`.

## 1. Project vision

Studio m2 vloeren legt vloeren bij klanten. Naast de dienstverlening op locatie beschikt Studio m2 over een rijdende showroom: een bus met vloerstaaltjes waarmee advies en materiaalkeuze bij de klant thuis kunnen plaatsvinden.

De website moet Studio m2 professioneel presenteren, vertrouwen opbouwen, het aanbod en eerder werk inzichtelijk maken en geïnteresseerden helpen om contact op te nemen of een afspraak aan huis te plannen. De rijdende showroom is daarbij een belangrijke propositie.

De website wordt nadrukkelijk geen webshop. Er komen geen producten in Shopify en er is geen online bestel- of betaalproces nodig. Shopify wordt gebruikt als CMS, hostingplatform en Theme Editor.

## 2. Business information

Onderstaande informatie moet tijdens discovery worden verzameld en gevalideerd. Onbekende gegevens mogen niet worden ingevuld op basis van aannames.

| Onderwerp | Waarde | Status |
| --- | --- | --- |
| Bedrijfsnaam / juridische naam | [NOG TE BEPALEN] | TODO |
| Publieke handelsnaam | Studio m2 vloeren (te bevestigen) | TODO |
| Telefoonnummer | [NOG TE BEPALEN] | TODO |
| E-mailadres | [NOG TE BEPALEN] | TODO |
| Vestigingsplaats / adres | [NOG TE BEPALEN] | TODO |
| Werkgebied | [NOG TE BEPALEN] | TODO |
| KvK-nummer | [NOG TE BEPALEN] | TODO |
| Openingstijden / bereikbaarheid | [NOG TE BEPALEN] | TODO |
| Socialmedia-kanalen en URL's | [NOG TE BEPALEN] | TODO |
| Diensten | [NOG TE BEPALEN] | TODO |
| Vloersoorten | [NOG TE BEPALEN] | TODO |
| Merken | [NOG TE BEPALEN] | TODO |
| Garantie en service | [NOG TE BEPALEN] | TODO |

## 3. Goals

- Een professionele, consistente uitstraling realiseren.
- Vertrouwen opbouwen bij potentiële klanten.
- Uitgevoerde projecten overtuigend tonen.
- Diensten en beschikbare vloersoorten duidelijk presenteren.
- De rijdende showroom als onderscheidende propositie promoten.
- Gekwalificeerde leads genereren.
- Afspraken aan huis stimuleren.
- De lokale organische vindbaarheid verbeteren.

Meetbare KPI's en prioriteiten zijn [NOG TE BEPALEN].

## 4. Target audience

**Status: DISCOVERY**

De primaire en secundaire doelgroepen, hun regio, behoeften, bezwaren, besliscriteria en klantreis zijn [NOG TE BEPALEN]. Er worden vóór afronding van discovery geen definitieve persona's of doelgroepaannames vastgelegd.

## 5. Positioning

De rijdende showroom is voorlopig een belangrijke onderscheidende propositie: klanten kunnen thuis advies krijgen en vloerstaaltjes in hun eigen ruimte en lichtsituatie beoordelen.

De definitieve positionering, bewijsvoering, tone of voice en verhouding tot andere onderscheidende punten worden tijdens discovery vastgesteld. Status: `DISCOVERY`.

## 6. Technical stack

- Shopify als CMS, hostingplatform en Theme Editor.
- Het officiële Shopify Skeleton Theme als codebasis.
- Shopify CLI voor lokale ontwikkeling, validatie en theme-preview/deployment.
- Visual Studio Code als ontwikkelomgeving.
- Codex als ontwikkel- en documentatie-assistent.
- Git voor versiebeheer.
- GitHub-repository `studiom2/Website` als remote repository.
- Shopify development theme voor ontwikkeling en review.
- Geen product-, catalogus-, winkelwagen-, checkout- of andere e-commercefunctionaliteit nodig voor de beoogde website.

Aanwezige upstream e-commercebestanden worden in deze fase niet verwijderd of aangepast. Eventuele latere opschoning vereist een apart, goedgekeurd architectuurbesluit en taak.

## 7. Development environment

| Onderdeel | Waarde |
| --- | --- |
| Shopify store | `qpuig0-px.myshopify.com` |
| Development theme ID | `203725832524` |
| GitHub | `studiom2/Website` |
| Lokale map | `C:\Users\Admin\Desktop\STUDIO_M2\studio-m2-theme` |

## 8. Development workflow

De vaste werkwijze is:

`discovery → besluit → taak → implementatie → test → preview → review → commit → volgende taak`

Toelichting:

1. **Discovery:** ontbrekende informatie en randvoorwaarden verzamelen.
2. **Besluit:** keuze en motivatie vastleggen in dit masterplan.
3. **Taak:** scope, resultaat en acceptatiecriteria definiëren.
4. **Implementatie:** uitsluitend binnen de goedgekeurde scope werken.
5. **Test:** relevante functionele en kwaliteitscontroles uitvoeren.
6. **Preview:** resultaat in het development theme controleren.
7. **Review:** feedback en akkoord verzamelen.
8. **Commit:** alleen de beoordeelde wijziging bewust vastleggen.
9. **Volgende taak:** register en actieve taak bijwerken.

## 9. Governance / Codex rules

Deze regels zijn bindend voor alle projectwerkzaamheden:

- Publiceer nooit zonder expliciete opdracht naar het live theme.
- Wijzig geen Shopify-billing, abonnementen of betaalgegevens.
- Wijzig geen domeinen, DNS-records of domeininstellingen.
- Installeer geen apps met kosten zonder expliciete toestemming.
- Voer geen grote scopewijzigingen uit zonder deze vooraf als besluit en taak vast te leggen.
- Ontwikkel en test altijd eerst in het development theme.
- Voeg geen onnodige e-commercecode of product-/catalogusfunctionaliteit toe.
- Test relevante wijzigingen op zowel mobiel als desktop.
- Maak content zoveel mogelijk beheerbaar via de Shopify Theme Editor.
- Hardcode geen bedrijfsdata wanneer theme settings, section settings of andere beheerbare contentmodellen logisch zijn.
- Verzin geen designrichting voordat referenties en discovery zijn afgerond.
- Behoud bestaande upstream Skeleton-bestanden totdat een expliciete taak wijziging of verwijdering toestaat.
- Werk dit masterplan bij wanneer status, scope, besluiten of open vragen veranderen.
- Commit, push of publiceer alleen wanneer de actuele opdracht dat expliciet toestaat.

## 10. Preliminary sitemap

**Status: VOORLOPIG / DISCOVERY**

- Home
- Vloeren
- Rijdende showroom
- Projecten
- Werkwijze
- Over Studio m2
- Contact
- Afspraak aan huis

Paginahiërarchie, navigatie, URL's en eventuele samenvoegingen worden pas definitief na doelgroep-, content- en SEO-discovery.

## 11. Content requirements

- [ ] Logo in geschikte bestandsformaten en varianten
- [ ] Kleuren en overige huisstijlrichtlijnen
- [ ] Lettertypes en gebruiksrechten
- [ ] Gevalideerde bedrijfsgegevens
- [ ] Overzicht en omschrijving van diensten
- [ ] Overzicht en omschrijving van vloersoorten
- [ ] Merken en toestemming/richtlijnen voor merkvermelding
- [ ] Projectfoto's met context en publicatierechten
- [ ] Foto's van de bus / rijdende showroom met publicatierechten
- [ ] Reviews en toestemming voor publicatie
- [ ] Socialmedia-kanalen en correcte links
- [ ] Voorbeeldwebsites en toelichting op wat aanspreekt
- [ ] Relevante concurrenten
- [ ] Gewenste SEO-regio's en prioriteit per regio

Aanvullend te bepalen: kernboodschappen, tone of voice, FAQ's, processtappen, CTA-teksten, formulierteksten, metadata en eventuele video.

## 12. UX and conversion

- De primaire conversie is waarschijnlijk een afspraak aan huis via de rijdende showroom; dit moet tijdens discovery worden bevestigd.
- Definitieve primaire en secundaire CTA's zijn [NOG TE BEPALEN].
- Mobiele bruikbaarheid is belangrijk en wordt vanaf ontwerp tot oplevering volwaardig meegenomen.
- De rol en zichtbaarheid van contact, WhatsApp en direct bellen moeten worden beoordeeld.
- Formuliervelden, opvolgproces, succesmelding en foutafhandeling zijn [NOG TE BEPALEN].
- Conversie mag niet ten koste gaan van toegankelijkheid, duidelijkheid of vertrouwen.

## 13. Design system

**Status: BLOCKED pending discovery.**

Geblokkeerd totdat merkassets, referentiewebsites, gewenste uitstraling en contentbehoeften zijn verzameld en beoordeeld.

## 14. Theme architecture

**Status: BLOCKED pending discovery/design.**

Templates, sections, blocks, globale settings en contentmodellen worden pas ontworpen nadat sitemap, contentmodel en designrichting zijn goedgekeurd. Product- of catalogusarchitectuur is niet nodig.

## 15. SEO

**Status: DISCOVERY.**

Te onderzoeken: zoekintentie, diensten, vloersoorten, werkgebied, zoektermen, concurrentie, informatiearchitectuur, metadata, structured data en contentprioriteiten.

Er worden geen massale lokale landingspagina's gemaakt voordat de SEO-structuur en de inhoudelijke kwaliteit expliciet zijn goedgekeurd. Plaatsnamen en servicegebieden worden niet verzonnen.

## 16. Analytics

**Status: TODO.**

Vast te stellen en waar nodig in te richten:

- Analyticsplatform en account/eigenaarschap: [NOG TE BEPALEN]
- Google Search Console: [NOG TE BEPALEN]
- Conversiegebeurtenissen en KPI's: [NOG TE BEPALEN]
- Consentvereisten en meetgedrag vóór/na toestemming: [NOG TE BEPALEN]
- Rapportage, toegang en bewaartermijnen: [NOG TE BEPALEN]

## 17. Legal/privacy

**Status: TODO.**

- Privacyverklaring en verantwoordelijke partij: [NOG TE BEPALEN]
- Cookiebeleid en consentmechanisme: [NOG TE BEPALEN]
- Formulierdoeleinden, grondslag, bewaartermijn en ontvangers: [NOG TE BEPALEN]
- Algemene voorwaarden / garantievoorwaarden: [NOG TE BEPALEN]
- Verplichte bedrijfsvermeldingen: [NOG TE BEPALEN]
- Rechten en toestemming voor foto's, reviews, logo's en merken: [NOG TE BEPALEN]

Juridische teksten moeten door de verantwoordelijke opdrachtgever of een bevoegde adviseur worden aangeleverd of goedgekeurd.

## 18. Testing

Per implementatietaak wordt bepaald welke controles relevant zijn. Voor oplevering omvat het testplan minimaal:

- [ ] **Responsive:** afgesproken mobiele, tablet- en desktopbreedtes
- [ ] **Browser:** afgesproken actuele browsers en apparaten
- [ ] **Accessibility:** toetsenbord, focus, semantiek, labels, contrast en alternatieve teksten
- [ ] **Performance:** beeldoptimalisatie, laadtijd en afgesproken kernmetingen
- [ ] **Forms:** validatie, fouten, verzending, spambeperking en succesflow
- [ ] **Links:** interne, externe, telefoon-, e-mail- en eventuele WhatsApp-links
- [ ] **Theme Editor:** settings, blocks, previews, lege states en beheerbaarheid
- [ ] **Console errors:** geen onverklaarde JavaScript-, netwerk- of Liquid-fouten

Concrete browsers, apparaten, breakpoints en acceptatiedrempels zijn [NOG TE BEPALEN].

## 19. Launch

**Status: TODO — pre-launch checklist wordt tijdens implementatie ingevuld.**

### Content en configuratie

- [ ] [NOG TE BEPALEN]

### Kwaliteit en acceptatie

- [ ] [NOG TE BEPALEN]

### SEO, analytics en legal

- [ ] [NOG TE BEPALEN]

### Publicatie en rollback

- [ ] Expliciet akkoord voor live-publicatie ontvangen
- [ ] Publicatieplan: [NOG TE BEPALEN]
- [ ] Rollbackplan: [NOG TE BEPALEN]

### Controle na livegang

- [ ] [NOG TE BEPALEN]

## 20. Future roadmap

**Status: TODO.**

Mogelijke toekomstige fasen, optimalisaties en uitbreidingen worden hier pas toegevoegd nadat ze inhoudelijk zijn besproken en goedgekeurd: [NOG TE BEPALEN].

## 21. Task register

| ID | Taak | Status | Afhankelijkheid / opmerking |
| --- | --- | --- | --- |
| M2-GOV-001 | Projectbasis opzetten | DONE | Basis aanwezig |
| M2-DISC-001 | Bedrijfsinformatie verzamelen | READY | Huidige actieve taak |
| M2-DISC-002 | Referentie/voorbeeldwebsites analyseren | READY | Huidige actieve taak |
| M2-DISC-003 | Concurrentie en positionering analyseren | BLOCKED | Wacht op bedrijfsinformatie en relevante markt/context |
| M2-DISC-004 | Definitieve sitemap bepalen | BLOCKED | Wacht op discovery, content en SEO-inzichten |
| M2-DES-001 | Designrichting bepalen | BLOCKED | Wacht op merkassets en referentieanalyse |
| M2-ARCH-001 | Theme architectuur bepalen | BLOCKED | Wacht op definitieve sitemap, contentmodel en designrichting |
| M2-DEV-001 | Implementatie starten | BLOCKED | Wacht op goedgekeurde designrichting en architectuur |

### M2-GOV-001 — Projectbasis opzetten

**Status: DONE**

Resultaat:

- Shopify-account/store aanwezig.
- GitHub-repository aanwezig.
- Shopify Skeleton Theme aanwezig.
- Git-repository gekoppeld.
- Eerste baseline-commit gepusht.
- Shopify CLI gekoppeld.
- Development theme actief.

## 22. Decision log

### DEC-001 — Shopify als platform

Shopify wordt gebruikt als platform ondanks dat de website geen webshop is. Het platform dient als CMS, hostingplatform en Theme Editor.

### DEC-002 — Skeleton Theme als basis

Het officiële Shopify Skeleton Theme wordt gebruikt in plaats van Dawn.

### DEC-003 — Development theme eerst

Ontwikkeling en controle gebeuren eerst via het Shopify development theme. Publicatie naar het live theme vereist een expliciete opdracht.

### DEC-004 — Centrale source of truth

`docs/MASTERPLAN.md` is de centrale source of truth van het project.

## 23. Open questions

Open vragen blijven `[NOG TE BEPALEN]` totdat het antwoord is aangeleverd, geverifieerd en waar relevant als besluit is vastgelegd.

### Business en positionering

- Wat zijn de volledige juridische bedrijfsnaam en publieke handelsnaam?
- Wat zijn het telefoonnummer, e-mailadres, adres, KvK-nummer en de bereikbaarheid?
- Wat is het exacte werkgebied en welke regio's hebben prioriteit?
- Welke diensten, vloersoorten en merken biedt Studio m2 aan?
- Welke garantie, nazorg en service worden geboden?
- Wat zijn de belangrijkste onderscheidende punten naast de rijdende showroom?
- Hoe werkt de rijdende showroom praktisch: beschikbaarheid, regio, kosten, duur en voorbereiding?
- Wie zijn de belangrijkste concurrenten en alternatieven voor de klant?

### Doelgroep en conversie

- Wie zijn de primaire en secundaire doelgroepen?
- Welke behoeften, zorgen en besliscriteria hebben zij?
- Wat is de primaire conversie: afspraak aan huis, offerteaanvraag, bellen of iets anders?
- Welke secundaire CTA's zijn nodig?
- Hoe worden aanvragen ontvangen, toegewezen en opgevolgd?
- Is WhatsApp gewenst en welk account/nummer mag daarvoor worden gebruikt?

### Content

- Welke logo-, kleur-, typografie- en huisstijlbestanden zijn beschikbaar?
- Welke project-, team- en busfoto's zijn beschikbaar en mogen worden gepubliceerd?
- Welke reviews mogen met naam, bron en toestemming worden gebruikt?
- Welke teksten bestaan al en wie levert of keurt nieuwe teksten goed?
- Welke socialmedia-kanalen zijn actief?
- Zijn FAQ's, werkwijze, merkeninformatie en garantievoorwaarden beschikbaar?
- Welke voorbeeldwebsites spreken aan, welke elementen specifiek en waarom?

### Design en UX

- Welke merkwaarden en gewenste uitstraling moet het ontwerp uitdragen?
- Welke visuele stijlen of patronen moeten juist worden vermeden?
- Welke referenties zijn richtinggevend voor layout, fotografie, typografie en interactie?
- Welke navigatiestructuur en pagina's zijn noodzakelijk?
- Zijn er specifieke toegankelijkheids- of apparaatvereisten bovenop de basisnormen?

### SEO

- Op welke diensten, vloersoorten en regio's moet de website gevonden worden?
- Is er bestaand zoekwoorden-, concurrentie- of verkeersdata beschikbaar?
- Bestaat er een huidig domein of bestaande website met te behouden URL's en autoriteit?
- Welke lokale bedrijfsvermeldingen en profielen bestaan al?
- Wie is verantwoordelijk voor doorlopende SEO-content en actualisatie?

### Functionaliteit en techniek

- Welke formulieren en velden zijn nodig?
- Naar welk adres of systeem moeten formulierinzendingen worden gestuurd?
- Is planning of agenda-integratie gewenst, nu of later?
- Welke analytics-, consent- en marketingtools zijn toegestaan?
- Zijn meertaligheid of extra talen nodig?
- Welke content moet door Studio m2 zelfstandig in de Theme Editor beheerd kunnen worden?
- Welke browser-, apparaat- en performancecriteria gelden voor acceptatie?
- Wie beoordeelt previewwijzigingen en wie mag live-publicatie autoriseren?

### Legal en beheer

- Wie levert of keurt privacy-, cookie- en voorwaardenpagina's goed?
- Welke bewaartermijnen en toestemmingen gelden voor leads en analytics?
- Wie wordt eigenaar van Shopify, GitHub, analytics en Search Console?
- Wat is na livegang het proces voor onderhoud, back-ups, incidenten en contentupdates?

## 24. Current active task

**M2-DISC-001 + M2-DISC-002**

- `M2-DISC-001 — Bedrijfsinformatie verzamelen` is `READY`.
- `M2-DISC-002 — Referentie/voorbeeldwebsites analyseren` is `READY`.

De eerstvolgende input bestaat uit gevalideerde bedrijfsinformatie en referentie-/voorbeeldwebsites met per voorbeeld een korte toelichting op wat wel en niet aanspreekt. Er start geen design- of implementatiewerk voordat de relevante discovery-uitkomsten zijn vastgelegd en beoordeeld.
