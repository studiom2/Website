# REFERENTIEANALYSE — BOMMELSVLOEREN

Ondersteunend discoverydocument bij [`MASTERPLAN.md`](./MASTERPLAN.md). Het masterplan blijft de centrale source of truth.

## 0. Scope, bron en beperkingen

**Status:** DONE

**Analyse-ID:** M2-DISC-002

**Analysedatum:** 2026-08-15

Geanalyseerde lokale snapshot:

- `PVC Visgraat Vloer Rotterdam _ Bommelsvloeren — Specialist Regio Rijnmond.html`
- Bijbehorende lokaal opgeslagen assets-map met CSS, JavaScript en afbeeldingen

De analyse beschrijft uitsluitend wat in de opgeslagen homepage-HTML en bijbehorende assets zichtbaar of technisch afleidbaar is. Niet alle interacties kunnen vanuit een statische snapshot worden uitgevoerd. Gesloten dropdowns, de inhoud van het mobiele menu, formulierafhandeling en niet-opgeslagen pagina's zijn daarom alleen benoemd wanneer daarvoor voldoende HTML-, class- of scriptbewijs bestaat.

De bron is een functionele referentie, geen ontwerp- of contenttemplate. Teksten, vormgeving, branding, claims, bedrijfsgegevens en code worden niet gekopieerd.

## 1. Samenvatting

Bommelsvloeren combineert een duidelijke lokale specialisatie met veel herhaalde conversieroutes. De homepage werkt als een lange landingspagina: aanbod, advies aan huis, voorbeeldvloeren, projecten, reviews, vakmanschap, lokale SEO-content en een afsluitende offerte-CTA volgen elkaar logisch op.

De belangrijkste bruikbare principes voor Studio m2 zijn:

- Een primaire CTA die in header, content en afsluiting terugkomt.
- De advies-aan-huispropositie vroeg tonen en inhoudelijk uitleggen.
- Vloersoorten visueel en informatief presenteren.
- Vertrouwen opbouwen met gerealiseerde projecten, gevalideerde reviews en vakmanschap.
- Lokale vindbaarheid ondersteunen met relevante, unieke content en correcte technische metadata.
- Meerdere contactmogelijkheden aanbieden zonder de primaire route onduidelijk te maken.

Studio m2 kan zich duidelijker onderscheiden door de bus niet alleen als “advies aan huis” te beschrijven, maar consequent als **rijdende showroom** te positioneren en zichtbaar te maken.

## 2. Header

### 2.1 Topbar

De topbar staat buiten de sticky header en is alleen vanaf het `md`-breakpoint zichtbaar (`hidden md:block`). Hij bevat:

- Een klikbare e-maillink met hulptekst.
- Een korte werkgebiedvermelding.
- Een link naar contact.
- Vijf sterren, een score van 5,0 en een zichtbaar aantal van 55 Google-reviews, gekoppeld aan de reviewpagina.

**Toepassing Studio m2:** gebruik een compacte trust-/contactbalk alleen wanneer telefoon, e-mail, werkgebied en reviews zijn gevalideerd. Op kleine schermen verdient eenvoud voorrang.

### 2.2 Hoofdheader

De hoofdheader is sticky (`sticky top-0`) en gebruikt een lichte transparante achtergrond met blur. Op desktop bestaat de rij uit:

- Links: een telefoonlink met de tekst dat bellen of WhatsApp mogelijk is.
- Midden: woordmerk/tagline en home-link.
- Rechts: primaire CTA naar de contactpagina.

Op mobiel:

- De telefoonmodule is verborgen (`hidden lg:inline-flex`).
- Een menuknop met toegankelijk label “Menu openen” verschijnt (`lg:hidden`).
- Het logo blijft centraal.
- De primaire CTA blijft zichtbaar, maar compacter.

De desktopnavigatie is pas vanaf `lg` zichtbaar en bevat:

- PVC Vloeren → `/collectie`
- Tapijt & Stoffering → `/collectie#tapijt-stoffering`
- Laminaat → `/collectie#laminaat`
- Projecten → `/projecten`
- Bommelsvloeren → `/over-ons`

Chevron-iconen suggereren dropdowns bij enkele categorieën, maar de gesloten snapshot bevat geen dropdowninhoud. Die functionaliteit kan daarom niet volledig worden bevestigd.

### 2.3 Conversie en aandachtspunten

- De offerte-CTA blijft tijdens scrollen bereikbaar door de sticky header.
- Een vaste WhatsApp-knop rechtsonder biedt een tweede directe contactroute.
- De desktoptekst “Bel of WhatsApp ons” is technisch gekoppeld aan een `tel:`-link; WhatsApp zelf loopt via de losse zwevende `wa.me`-link. Studio m2 moet labels en linkgedrag eenduidig maken.
- Headerclaims en reviewdata mogen bij Studio m2 pas worden gepubliceerd na verificatie.

## 3. Homepage-secties in bronvolgorde

Header en footer staan buiten onderstaande elf `main`-secties.

| # | Sectie | Doel | Content en interactie | CTA | Mogelijke toepassing Studio m2 |
| --- | --- | --- | --- | --- | --- |
| 1 | Hero met twee nevencategorieën | Direct aanbod, regio en vervolgstap duidelijk maken | Grote visgraatafbeelding met H1; daarnaast kaarten voor laminaat en tapijt; hover/beeldzoom | Collectie bekijken; gratis adviesgesprek; categorie-links | Eén heldere waardepropositie, echte project-/busfoto, primaire afspraak-CTA en secundaire vloerenroute; alleen bevestigde vloersoorten tonen |
| 2 | USP-strip | Bezwaren vroeg wegnemen | Vier compacte voordelen over advies, voorbereiding, afwerking en snelheid | Geen | 3–4 gevalideerde USP's; rijdende showroom als eerste punt; geen levertermijnclaim zonder bevestiging |
| 3 | Merkenmarquee | Merkvertrouwen en assortimentbreedte tonen | Bewegende, dubbel weergegeven merkenlijst | Geen | Alleen gebruiken bij bevestigde merken en toestemming; anders weglaten |
| 4 | Vloercategorieën | Oriëntatie op type/patroon ondersteunen | Introductie plus vier visuele categoriekaarten met afbeelding en korte uitleg | Volledige collectie en categorie-anchors | Informatieve vloerenhub met categoriekaarten, geen Shopify-producten |
| 5 | Gratis advies aan huis | Adviespropositie uitleggen en converteren | Foto, uitleg over selectie, stalen, locatiebezoek en werkgebied | Adviesgesprek aanvragen | Omvormen tot prominente rijdende-showroomsectie met busfoto, voordelen, verwachtingen en afspraak-CTA |
| 6 | Nieuwe/bestseller-vloeren | Concrete dessins en prijsoriëntatie tonen | Vier productachtige kaarten met naam, categorie, korte beschrijving en prijs per m² | Per kaart een offerte-link; link naar alle dessins | Niet overnemen als productcatalogus; eventueel inspiratievoorbeelden zonder prijs, SKU of productlogica |
| 7 | Recente projecten | Vakmanschap bewijzen | Drie foto's met projectnaam, plaats, jaar en categorie | Alle projecten | Projectkaarten met echte foto's en gevalideerde metadata; detailpagina's alleen indien genoeg content beschikbaar is |
| 8 | Reviews | Sociaal bewijs leveren | Score, zichtbaar reviewaantal, vier reviewcards met sterren, tekst, naam/foto en relatieve datum | Alle reviews | Reviewsectie en eventueel reviewoverzicht, uitsluitend met bron, toestemming en actuele data |
| 9 | Vakmanschap / over | Merkverhaal en kwaliteitsperceptie versterken | Werkfoto, vakmanschapsverhaal en herhaalde Google-score | Ons verhaal | Menselijk verhaal over werkwijze/vakmanschap; claims pas na bedrijfsdiscovery |
| 10 | Informatieve lokale SEO-content | Zoekintentie beantwoorden en lokale relevantie vergroten | Uitleg over een vloertype en regio's in twee tekstkolommen | Geen | Unieke, behulpzame content over bevestigde vloersoorten en werkgebied; geen plaatsnamen overnemen |
| 11 | Afsluitende CTA | Bezoeker na de volledige bewijsopbouw laten converteren | Korte samenvatting van advies aan huis | Offerte aanvragen | Afspraak voor rijdende showroom als primaire actie; offerte als mogelijke vervolgstap [NOG TE BEPALEN] |

## 4. Navigatie en informatiearchitectuur

### 4.1 Interne hoofdroutes zichtbaar in de snapshot

- `/` — Home
- `/collectie` — Collectie / vloeren
- `/projecten` — Projecten
- `/over-ons` — Over ons
- `/reviews` — Reviews
- `/veelgestelde-vragen` — Veelgestelde vragen
- `/contact` — Contact / offerte / advies
- `/privacy` — Privacyverklaring

### 4.2 Collectie-anchors en subcategorieën

- `/collectie#pvc-visgraat`
- `/collectie#pvc-rechte-plank`
- `/collectie#pvc-hongaarse-punt`
- `/collectie#pvc-tegels`
- `/collectie#laminaat`
- `/collectie#tapijt-stoffering`

De structured data noemt daarnaast diensten/categorieën voor gietvloeren en egaliseren, maar daarvoor zijn in de opgeslagen homepage geen aparte anchors gevonden.

### 4.3 Linkstructuur en beperkingen

- De homepage stuurt veel verschillende CTA-labels naar dezelfde `/contact`-route.
- Projectkaarten zijn in de snapshot niet individueel gelinkt; alleen “Alle projecten” leidt naar `/projecten`.
- De productachtige vloerkaarten hebben geen detailpagina; iedere offerteknop gaat rechtstreeks naar `/contact`.
- Een eventuele individuele project- of vloerroute kan op basis van deze snapshot niet worden bevestigd.

## 5. Conversieanalyse

### 5.1 Conversieroutes

De primaire route is contact/offerte via `/contact`. Deze wordt herhaald in:

- De sticky header.
- De hero als adviesgesprek.
- De advies-aan-huissectie.
- Iedere productachtige vloerkaart.
- De afsluitende CTA.

Secundaire routes zijn:

- `tel:` voor direct bellen.
- `mailto:` in de desktop-topbar.
- Een vaste `wa.me`-knop voor WhatsApp.
- Verdiepende routes naar collectie, projecten, reviews en over ons.

### 5.2 Trustelementen

- Reviewscore en reviewaantal in topbar, reviewsectie, vakmanschapssectie en footer.
- Projectfoto's met plaats, jaar en categorie.
- Merkenlijst.
- Concrete USP's over voorbereiding en afwerking.
- Bedrijfsadres, telefoon, e-mail en KvK in footer/structured data.
- Lokale werkgebiedvermeldingen.

### 5.3 Aanbeveling Studio m2

Gebruik één primaire terminologie, bijvoorbeeld “Plan de rijdende showroom” of “Maak een afspraak aan huis” [NOG TE BEPALEN]. Een offerte kan een vervolgstap of secundaire CTA zijn. Bellen en WhatsApp blijven nuttige snelroutes als de eigenaar die kan en wil opvolgen.

De opgeslagen homepage bevat geen formulier. De velden, validatie, privacytoestemming, verzendroute en bevestiging van `/contact` kunnen dus niet uit deze bron worden geanalyseerd.

## 6. Reviews en social proof

Zichtbaar op de homepage:

- Score: 5,0 uit 5.
- Zichtbaar aantal: 55 Google-reviews/beoordelingen.
- Vier reviewcards met vijf sterren, tekst, naam, profielfoto en relatieve datum.
- Een link naar `/reviews`.
- Compacte reviewvermeldingen in topbar, vakmanschapssectie en footer.

Technisch aandachtspunt in de bron:

- De `LocalBusiness` structured data bevat `aggregateRating.reviewCount: 5`, terwijl de pagina zichtbaar 55 beoordelingen vermeldt. Dat is inconsistent en moet bij Studio m2 worden voorkomen.

Voor Studio m2 zijn reviewscore, aantal, tekst, namen, foto's en bron allemaal `[NOG TE BEPALEN]`. Publiceer geen reviews zonder geldige bron en toestemming. Als live synchronisatie niet beschikbaar is, moet handmatig beheer een duidelijke actualisatiedatum en eigenaar krijgen.

## 7. Projecten

De homepage toont drie projecten met:

- Grote projectfoto.
- Projectnaam.
- Plaats of gebied.
- Jaar.
- Categorie (in de snapshot: visgraat).

De projectkaarten zelf zijn niet gelinkt in de opgeslagen HTML. Alleen de overzichts-CTA verwijst naar `/projecten`. Daardoor is een projectdetailstructuur niet aantoonbaar.

Aanbevolen voor Studio m2:

- Een beheerbaar projectenoverzicht met echte beelden.
- Minimaal: titel, vloer-/patroontype, plaats of globaal gebied, jaar en korte toelichting.
- Optioneel: detailpagina met galerij, uitgangssituatie, werkzaamheden en resultaat wanneer voldoende content bestaat.
- Geen klantadres of andere persoonsgegevens publiceren.

## 8. Vloeren en collectie zonder productcatalogus

Bommelsvloeren gebruikt twee presentatieniveaus:

1. Categoriekaarten voor visgraat, rechte plank, Hongaarse punt en betonlook/PVC-tegels.
2. Productachtige inspiratiekaarten met dessin, categorie, beschrijving en prijs per m².

Voor Studio m2 is het eerste niveau bruikbaar. Het tweede niveau past niet bij de huidige scope, omdat er geen Shopify-producten, prijzen of webshoplogica komen.

Vertaling naar Studio m2:

- Maak `Vloeren` een informatieve hub.
- Gebruik categoriekaarten voor uitsluitend bevestigde vloersoorten.
- Geef per categorie uitleg over uitstraling, toepassing, aandachtspunten, mogelijke patronen en relevante projecten.
- Gebruik sfeer-/projectbeelden als inspiratie, niet als bestelbare artikelen.
- Koppel iedere categorie aan afspraak/contact, niet aan winkelwagen of checkout.
- Beheer categorieën via pagina's, metaobjects en/of theme-editorcontent; de definitieve techniek volgt pas in M2-ARCH-001.

## 9. Rijdende showroom / advies aan huis

Bommelsvloeren ondersteunt “gratis advies aan huis” op meerdere niveaus:

- Secundaire CTA in de hero.
- Eerste USP direct onder de hero.
- Een volledige uitlegsectie met stalen en locatiebezoek.
- Vermelding in lokale SEO-copy.
- Afsluitende CTA.
- Een service-aanbod in structured data.

Studio m2 kan dit sterker en eigen maken door **Rijdende showroom** als vaste productnaam/propositie te gebruiken:

- Toon de bus en vloerstaaltjes prominent met eigen fotografie.
- Leg in drie korte stappen uit wat vóór, tijdens en na de afspraak gebeurt [NOG TE BEPALEN].
- Benoem pas na bevestiging: kosten, duur, beschikbaarheid, werkgebied, aantal stalen en eventuele voorwaarden.
- Leg het klantvoordeel uit: materiaalkeuze en advies in de eigen woonomgeving.
- Geef de propositie een eigen pagina en een primaire CTA vanuit header, hero en relevante vloerenpagina's.
- Laat de contactroute context meenemen, bijvoorbeeld onderwerp “Rijdende showroom” [PROPOSED].

## 10. SEO-analyse

### 10.1 Metadata

De snapshot bevat:

- Een lokale, dienstgerichte `<title>`.
- Meta description.
- Canonical naar de homepage.
- `author`, `keywords` en Google Site Verification.
- Open Graph title, description, URL, type, locale, site name en afbeelding.
- Twitter summary-card en afbeelding/title/description.
- Preload van de heroafbeelding.

De aanpak is bruikbaar, maar Studio m2 moet eigen metadata op basis van eigen aanbod en goedgekeurd werkgebied krijgen. De `keywords`-metatag is geen noodzakelijke prioriteit.

### 10.2 Structured data

Er staat één JSON-LD-graph met:

- `LocalBusiness` en `HomeAndConstructionBusiness`.
- Naam, juridische naam, URL, telefoon, e-mail, adres, geo, kaartlink en openingstijden.
- Werkgebieden als steden en een geografische radius.
- Instagramprofiel.
- Prijs-/betaalgegevens.
- KvK-identificatie.
- Aggregate rating.
- Diensten via `makesOffer` en `hasOfferCatalog`.
- Offerteactie via `ReserveAction`.
- Gekoppeld `WebSite`-object met taal en publisher.

Voor Studio m2 mag structured data uitsluitend bevestigde, zichtbare en actuele informatie bevatten. De schema-typen en properties moeten tijdens implementatie opnieuw op geschiktheid en geldigheid worden beoordeeld. De reviewcount-inconsistentie in de referentie mag niet worden overgenomen.

### 10.3 Content- en headingstructuur

- Eén H1 op de homepage.
- Tien H2's en vijftien H3's.
- De USP-strip gebruikt H3's zonder eigen H2; visueel begrijpelijk, maar semantisch verdient een passende sectiekop of andere markup overweging.
- Lokale termen, diensten en plaatsnamen komen terug in hero, categoriecontent, projecten, adviessectie en informatieve tekst.
- Afbeeldingen hebben meestal beschrijvende alt-teksten met vloer- en regiocontext.
- Interne links verbinden home met collectie, categorie-anchors, projecten, reviews, over, FAQ, contact en privacy.

Studio m2 moet lokale SEO baseren op werkelijk werkgebied, relevante zoekintentie en inhoudelijke waarde. Geen massale of dunne plaatslandingspagina's zonder goedgekeurde strategie.

## 11. Footer

De footer bevat vier functionele groepen:

- Merkintroductie en compacte positionering.
- Reviewscore en link naar reviews.
- Collectie-/categorieanchors.
- Contactgegevens, Instagram en volledige secundaire navigatie.

De onderste balk bevat copyright, bedrijfsnaam, KvK en een merkzin. De zichtbare footer toont geen openingstijden; die staan wel in structured data.

Voor Studio m2 zijn minimaal gewenst: logo/naam, korte propositie, kernnavigatie, vloeren/diensten, gevalideerde contact- en bedrijfsgegevens, privacylink en eventuele socials. KvK en overige juridische gegevens volgen pas na aanlevering.

## 12. Responsive en mobiel

Uit de HTML/classes blijkt:

- Topbar verborgen onder `md`.
- Desktoptelefoon verborgen onder `lg`.
- Mobiele menuknop zichtbaar onder `lg`.
- Desktopnavigatie verborgen onder `lg`.
- Header-CTA blijft op mobiel zichtbaar met kleinere padding/tekst.
- Typografie schaalt via `md`-classes.
- Meerkolomsgrids schakelen op mobiel naar gestapelde content.
- Bij de advies- en vakmanschapssecties verandert de volgorde van beeld en tekst tussen mobiel en desktop.
- De vaste WhatsApp-knop blijft rechtsonder beschikbaar.

De gesloten mobiele drawer staat niet in de opgeslagen DOM. Openen, focusmanagement, scroll-lock, sluitgedrag en submenu's moeten daarom later zelfstandig toegankelijk worden ontworpen en getest.

## 13. Animaties en interacties

Zichtbaar of uit classes afleidbaar:

- Sticky header.
- Mobiele menuknop met JavaScript-interactie.
- Vaste WhatsApp-knop.
- Marquee voor merken.
- Fade-up animatie bij contentintroductie.
- Hoverzoom (`scale-105`) op beelden in kaarten.
- Kleur- en transformtransities op links, knoppen en kaarten.
- Kleine diagonale/pijlverplaatsingen bij hover.
- Backdrop blur op de sticky header.

Niet aangetroffen op de opgeslagen homepage:

- Formulieren.
- Carousel-/sliderbediening.
- Video.
- Individuele project- of vloerkaartlinks.

Studio m2 moet motion subtiel inzetten, `prefers-reduced-motion` respecteren en geen essentiële informatie alleen via hover ontsluiten.

## 14. Studio m2 feature matrix

`MUST`, `SHOULD`, `COULD` en `NO` zijn discoveryprioriteiten, geen definitief architectuurbesluit.

| Feature | Bommelsvloeren | Studio m2 gewenst? | Studio m2 implementatie | Prioriteit | Opmerking |
| --- | --- | --- | --- | --- | --- |
| Responsive sticky header | Ja | Ja | Compacte header met logo, navigatie en primaire afspraak-CTA | MUST | Mobiel en desktop toegankelijk testen |
| Desktop-topbar | Ja | Waarschijnlijk | Contact/trustbalk met alleen bevestigde data | SHOULD | Kan op mobiel vervallen |
| Primaire CTA in header | Offerte | Ja | Afspraak rijdende showroom / aan huis [NOG TE BEPALEN] | MUST | Eén consistente primaire term kiezen |
| Direct bellen | Ja | Te bevestigen | `tel:`-link op geschikte plekken | SHOULD | Alleen met bevestigd nummer en bereikbaarheid |
| WhatsApp | Zwevende knop | Te bevestigen | Duidelijke `wa.me`-route met toegankelijk label | SHOULD | Alleen als opvolging organisatorisch geregeld is |
| Hero met fotografie | Ja | Ja | Eigen project- of busbeeld en eigen waardepropositie | MUST | Geen bronbeeld of broncopy gebruiken |
| USP-strip | Vier USP's | Ja | 3–4 gevalideerde voordelen | MUST | Geen onbevestigde snelheid/garantieclaims |
| Rijdende showroom | Als advies aan huis | Ja, sterker | Eigen prominente sectie plus detailpagina en CTA | MUST | Kernonderscheid van Studio m2 |
| Vloerencategorieën | Visuele categoriekaarten | Ja | Informatieve categoriekaarten/-pagina's | MUST | Alleen bevestigde soorten |
| Shopify-productcatalogus | Productachtige kaarten | Nee | Geen products, prijzen, cart of checkout | NO | Past niet bij vastgesteld projectmodel |
| Prijzen per m² | Ja | Niet nu | Geen prijzen tot expliciete goedkeuring | NO | Scope en prijsmodel onbekend |
| Inspiratievoorbeelden | Ja | Ja | Niet-bestelbare sfeer-/projectvoorbeelden | SHOULD | Duidelijk scheiden van projecten |
| Merkenmarquee | Ja | Mogelijk | Rustige merkvermelding of logo-overzicht | COULD | Merken en rechten eerst bevestigen |
| Werkwijze | Via USP/copy | Ja | Duidelijke stappen van advies tot oplevering | MUST | Inhoud nog verzamelen |
| Projectenoverzicht | Ja | Ja | Beheerbare kaarten met beeld en metadata | MUST | Echte Studio m2-projecten vereist |
| Projectdetailpagina's | Niet aantoonbaar | Mogelijk | Detailcases als contentvolume voldoende is | COULD | SEO- en beheerlast afwegen |
| Reviewsectie | Ja | Ja | Geverifieerde reviews met bron/toestemming | MUST | Geen score/aantal verzinnen |
| Aparte reviewpagina | Ja | Waarschijnlijk | Overzicht of externe reviewroute [NOG TE BEPALEN] | SHOULD | Afhankelijk van beschikbare reviews |
| Vakmanschaps-/over-sectie | Ja | Ja | Persoonlijk verhaal en bewijs | MUST | Bedrijfsinformatie nodig |
| Lokale SEO-content | Ja | Ja | Unieke service-/regiocontent | MUST | Werkgebied eerst bevestigen |
| FAQ-preview en pagina | Alleen route zichtbaar | Ja | Homepagepreview plus volledige FAQ | SHOULD | Vragen uit klantgesprekken verzamelen |
| Herhaalde CTA's | Ja | Ja | Contextueel na belangrijke bewijsblokken | MUST | Niet iedere kaart identiek belasten |
| Contact-/offerteformulier | Niet zichtbaar op homepage | Ja | Kort, privacybewust formulier | MUST | Velden en afhandeling [NOG TE BEPALEN] |
| Footer met contact/legal | Ja | Ja | Bedrijfsdata, navigatie, privacy en socials | MUST | Alleen gevalideerde gegevens |
| LocalBusiness structured data | Uitgebreid | Ja, indien passend | Alleen zichtbare en bevestigde data | MUST | Validatie en consistentie vereist |
| Open Graph/social metadata | Ja | Ja | Paginaspecifieke metadata en eigen beelden | MUST | Beheerbaarheid meenemen |
| Marquee-animatie | Ja | Niet noodzakelijk | Alleen wanneer functioneel en toegankelijk | COULD | Geen prioriteit voor conversie |
| Hoverzoom/transities | Ja | Subtiel | Eigen motionregels met reduced-motion | COULD | Geen designrichting vastleggen |
| Massale lokale pagina's | Niet zichtbaar | Nee zonder strategie | Eerst SEO-structuur goedkeuren | NO | Bestaande governance blijft gelden |

## 15. Voorlopige Studio m2-sitemap

**Status: PROPOSED — nog geen definitief besluit.**

- Home
- Vloeren
  - PVC
  - Visgraat
  - Hongaarse punt
  - Rechte plank
  - Laminaat
  - Aanvullende soorten `[NOG TE BEPALEN]`
- Rijdende showroom
- Projecten
- Werkwijze
- Over Studio m2
- Reviews
- Veelgestelde vragen
- Contact / offerte
- Privacy

Open punten:

- De feitelijke vloersoorten moeten nog worden bevestigd.
- Bepalen of patronen onder PVC vallen of zelfstandige pagina's verdienen.
- Bepalen of “Contact / offerte” één pagina wordt en hoe de afspraakroute daarin landt.
- Bepalen of projecten detailpagina's krijgen.
- Bepalen welke juridische pagina's naast privacy nodig zijn.

## 16. Voorlopige homepage-blueprint Studio m2

**Status: PROPOSED — input voor M2-DISC-004 en M2-DES-001.**

1. Header met compacte trust/contactinformatie en primaire afspraak-CTA.
2. Hero met eigen waardepropositie, eigen fotografie en primaire rijdende-showroom-CTA.
3. Korte USP-strip met uitsluitend bevestigde voordelen.
4. Rijdende showroom: bus, stalen, klantvoordeel en afspraakroute.
5. Vloersoorten: informatieve categoriekaarten zonder productlogica.
6. Werkwijze: van eerste contact en advies tot leggen en nazorg `[NOG TE BEPALEN]`.
7. Uitgelichte projecten met echte Studio m2-beelden.
8. Reviews/social proof met gevalideerde brongegevens.
9. Vakmanschap / Over Studio m2.
10. Werkgebied en behulpzame lokale SEO-content op basis van bevestigd werkgebied.
11. FAQ-preview met link naar alle vragen.
12. Afsluitende CTA voor afspraak aan huis / rijdende showroom, met offerte als mogelijke secundaire route.
13. Footer met navigatie, vloeren/diensten, contact, bedrijfsgegevens, socials en privacy.

De definitieve volgorde hangt af van beschikbare fotografie, doelgroepinzichten, bedrijfsinformatie en de gekozen primaire conversie.

## 17. WAT WE NIET OVERNEMEN

- Geen directe kopie van ontwerp, layoutcompositie, kleuren, typografie of beeldstijl.
- Geen teksten, slogans, metadata, reviews of alt-teksten kopiëren.
- Geen naam, logo, branding, foto's, merkenlijst of bedrijfsgegevens overnemen.
- Geen Bommelsvloeren-code of assets opnemen in het Shopify-theme.
- Geen Shopify-productcatalogus, winkelwagen of checkout toevoegen.
- Geen productachtige kaarten, dessinprijzen of prijsclaims zonder een later expliciet besluit.
- Geen claims over levertijd, snelheid, garantie, duurzaamheid, merken, regio's of gratis dienstverlening zonder bevestiging.
- Geen reviewscore of reviewaantal publiceren zonder actuele, controleerbare bron.
- Geen onnodige marquee, animatie of hovergedrag overnemen omdat het in de referentie staat.
- Geen SEO-teksten of plaatsnamen kopiëren; Studio m2 krijgt eigen, relevante content.
- Geen schema-data toevoegen die niet ook correct, actueel en zichtbaar op de website wordt ondersteund.
- Geen inconsistentie tussen zichtbare reviewdata en structured data.

## 18. Conclusie voor vervolgdiscovery

M2-DISC-002 kan op basis van deze analyse naar `DONE`. De referentie geeft voldoende richting voor functionele dekking en contentstructuur, maar legt geen design of architectuur vast.

Nog nodig voordat sitemap, ontwerp of architectuur definitief kan worden:

- Gevalideerde bedrijfsinformatie en werkgebied (M2-DISC-001).
- Bevestigde vloersoorten, diensten en merken.
- Beschikbare project-, bus- en bedrijfsfotografie.
- Beschikbare reviews en publicatierechten.
- Keuze van primaire CTA en opvolgproces.
- Aanvullende concurrentie-/positioneringsanalyse.
