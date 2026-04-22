# Astro Starter Kit: Minimal

```sh
npm create astro@latest -- --template minimal
```

> 🧑‍🚀 **Seasoned astronaut?** Delete this file. Have fun!

## 🚀 Project Structure

Inside of your Astro project, you'll see the following folders and files:

```text
/
├── public/
├── src/
│   └── pages/
│       └── index.astro
└── package.json
```

Astro looks for `.astro` or `.md` files in the `src/pages/` directory. Each page is exposed as a route based on its file name.

There's nothing special about `src/components/`, but that's where we like to put any Astro/React/Vue/Svelte/Preact components.

Any static assets, like images, can be placed in the `public/` directory.

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |

## 👀 Want to learn more?

Feel free to check [our documentation](https://docs.astro.build) or jump into our [Discord server](https://astro.build/chat).

## Woensdag 1 april

Vandaag ben ik begonnen met het verkennen van mogelijke concepten voor de API-opdracht.

In eerste instantie had ik twee ideeën:

Een Pokédex-app
Een boekenapp (vergelijkbaar met Goodreads)

Met een overleg met Cyd  bleek dat het Pokémon-idee wat simpel en minder onderscheidend was. De data en structuur zijn erg duidelijk en makkelijk te implementeren, waardoor er minder ruimte is voor verdieping en creativiteit.

Daarom heb ik besloten om verder te gaan met het boekenconcept.

Ik wil een app maken waarmee gebruikers:

boeken kunnen zoeken en doorbladeren
een detailpagina voor elk boek kunnen openen
boeken kunnen opslaan (bijvoorbeeld als “wil ik lezen”)

De docent adviseerde me ook om de API van Hardcover te gebruiken, die goed past bij dit soort apps.

### De volgende stap
-De gedrukte versie beter bestuderen (eindpunten, gegevensstructuur)
-De eerste opvraagprocedure in Astro testen
-Bepalen welke subpagina’s ik nodig heb (overzicht + details)

#### Concept:
*boekenapi

*features
-search bar
-list of books
-detail page
-favorites
<!-- content-api1: https://openlibrary.org/
     contentapi2: https://hardcover.app/ -->
<!-- web-pi: localStorage
 -->
## Voortgangsgesprek - week 1 
2 april

Tijdens de voortgangsgesprek heb ik mijn concept gepresenteerd: een boekenapp geïnspireerd op Goodreads, omdat ik van lezen houd en deze app zelf ook gebruik.

De feedback die ik heb gekregen:

* Het is een goed en duidelijk idee, maar bedenk wat jouw app uniek of andersmaakt dan Goodreads.
* Denk na over je eigen ervaring: wat mis je in Goodreads of wat kan er verbeterd worden?
* Probeer de API uit en bekijk de gegevensstructuur, zodat je beter kunt bepalen welke functies je wilt toevoegen.
* Overweeg om visuele interacties toe te voegen, zoals scroll-animaties en overgangen.
* Een mogelijk extra concept is een ‘op stemming gebaseerde’ functie, waarbij gebruikers boeken kunnen ontdekken op basis van hun stemming.


## Woensdag 9 april
Vandaag heb ik gewerkt met een content API in mijn Astro-project.
Ik heb de Open Library API gebruikt om boekgegevens op te halen en deze weergegeven op een overzichtspagina.

Ik heb geleerd hoe ik:

-data kan ophalen met fetch()
-JSON-data kan gebruiken (response.json())
-een lijst van boeken kan tonen met .map()
-Daarna heb ik een detailpagina gemaakt met een dynamische route ([...id].astro), zodat elke boek een eigen pagina heeft.
Bronen:

<!-- dynamic routes: https://docs.astro.build/en/guides/routing/ -->
## Voortgangsgesprek - week 2
10 april
 Tijdens het voortgangsgesprek heb ik feedback gekregen op mijn project. De belangrijkste punten zijn:
* Filtering en zoeken: Het filteren en zoeken van boeken moet op de server-side gebeuren, niet via JavaScript op de client.
* Interface (UI): Meer aandacht besteden aan de interface, vooral voor:
    * de pagina waar boeken worden opgeslagen
    * het beheren van lijsten
* Tags bij boeken: Bij elk boek een duidelijke tag toevoegen, zoals:
    * genre
    * collectie / categorie
* Visuele stijl per genre: De “vibe” van een boek visueel weergeven. Bijvoorbeeld:
    * horror → donkerdere kleuren, sterke box-shadows
    * andere genres → eigen kleuren en stijlen
* Moeilijkheidsgraad APIs: Volgens Cyd zijn LocalStorage en Web Share API relatief eenvoudig. Daarom wordt er van mij verwacht dat ik extra focus leg op:
    * UI/UX
    * visuele kwaliteit en interactie

