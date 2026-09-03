# Hairville — Homepage concept (Studio JAPI salesdemo)

Dit is een salesconcept: één volledig uitgewerkte, werkende homepage om tijdens
een verkoopgesprek te laten zien hoeveel sterker de website van Hairville kan
worden. Het is geen volledige website en geen live-gekoppeld systeem.

## Bron
- Bestaande website: https://hairville.weebly.com/ (+ contactpagina)
- Aangeleverde foto's en merkkleuren van de klant zelf

## Bedrijfsgegevens (overgenomen, niet verzonnen)
- Kapsalon Hairville, Heggestraat 2, 5664 BH Geldrop
- Telefoon: 040-8451522 · E-mail: info@hairville.nl
- Openingstijden: wo 09:00-18:00, do 09:00-20:00, vr 09:00-18:00, za 08:00-16:00, ma/di/zo gesloten
- Facebookpagina: bestaande link overgenomen

## Designrichting
Warm, premium salongevoel: ivoorwitte achtergrond, near-black (#181818) voor
tekst/donkere vlakken, rood (#c93a3a, afgeleid van de opgegeven #eb4747) als
sterke accentkleur. Editorial in plaats van generieke "hero + 3 cards"-opbouw:
asymmetrische hero-split, een prijslijst in menukaart-stijl (past bij een
kapsalon) in plaats van standaard servicekaarten, en een donkere CTA-sectie
voor het maken van een afspraak.

- Kleuren: `--color-primary #c93a3a`, `--color-ink #181818`,
  `--color-paper #faf7f3`, volledige set in `assets/css/styles.css` (`:root`)
- Typografie: **Newsreader** (serif, koppen) + **Manrope** (sans, body),
  geladen via Google Fonts. Dit is een ontwerpkeuze omdat het exacte
  bestaande lettertype niet uit de bronwebsite kon worden afgeleid —
  later te bevestigen met de klant.
- Logo: bestaand logo hergebruikt (`assets/images/logo-hairville.webp`)

## Gebruikte content
- Introtekst, diensten (knippen/kleuren/wassen/verzorging) en toon herschreven
  op basis van de summiere bestaande tekst, met behoud van de kernboodschap
- Contactgegevens en openingstijden 1-op-1 overgenomen

## Gebruikte foto's (allemaal van de klant, geen stockfoto's)
| Bestand | Gebruikt in |
|---|---|
| `logo-hairville.webp` | Header, footer |
| `salon-stoelen.webp` | Hero |
| `wachtruimte.webp` | Sfeersectie |
| `pand-entree.webp` | Sfeersectie |

Geen tijdelijke/stockbeelden nodig; alle secties zijn gevuld met echt
fotomateriaal van de klant.

## Verzonnen content — vóór salesgesprek te bevestigen
Op uitdrukkelijk verzoek voor dit concept toegevoegd, zodat de homepage
compleet en "af" aanvoelt. Dit zijn **voorbeelden**, geen echte gegevens van
Hairville:
- Alle prijzen en behandelduren in de sectie "Diensten & tarieven"
- De tekst en cijfers in de sectie "Over Hairville" (bijv. "al jaren",
  aantal styling plekken is wel af te lezen van de foto, de rest is invulling)
- De antwoorden in de FAQ-sectie (parkeren, cadeaubon, geen-afspraak-nodig)

Vervang deze onderdelen door de echte informatie van Hairville voordat dit
concept extern gedeeld wordt als zijnde definitieve informatie.

## Online boeken — bewust niet zelf gebouwd
Een eigen boekingssysteem bouwen we niet op de website zelf: een agenda die
realtime beschikbaarheid bijhoudt, dubbele boekingen voorkomt en aansluit op
de planning van de salon vraagt om een gespecialiseerde externe dienst
(bijvoorbeeld Salonized, Treatwell of Booqable), niet om iets dat je met
statische HTML/CSS/JS bouwt.

Daarom staat er nu een knop **"Boek online (binnenkort)"** naast de
telefoon-CTA in de sectie "Afspraak maken". Deze knop is bewust nog een
demo-link (`href="#"`, gemarkeerd met een code-comment in `index.html` bij
`id="boeken"`) totdat er een keuze is gemaakt voor een extern
boekingssysteem. Zodra dat gekozen is, hoeft alleen de `href` van die knop
vervangen te worden door de URL van dat systeem (of een widget-embed-code als
het systeem die aanbiedt).

## Demo-functionaliteit / placeholders
- Interne links (Diensten, De salon, Afspraak maken, Contact) zijn werkende
  anchor-links binnen deze ene pagina — er zijn geen aparte onderliggende
  pagina's, dit is een homepage-concept
- Telefoon-, e-mail- en Facebooklinks werken echt
- De knop "Boek online (binnenkort)" is nog een placeholder, zie hierboven

## Later nodig voor definitieve website
- Bevestiging van definitieve huisstijlkleuren en lettertype
- Echte, actuele prijslijst
- Keuze en koppeling van een extern boekingssysteem (zie hierboven)
- Eventueel: teamfoto's, reviews, voor-en-na foto's van klanten

## Techniek
Pure HTML/CSS/vanilla JavaScript, geen frameworks of build-stap nodig.
`index.html` direct openen in de browser is voldoende.

```
/
├── index.html
├── README.md
├── FOTOS-NODIG.md
└── assets/
    ├── css/styles.css
    ├── js/main.js
    └── images/
```
