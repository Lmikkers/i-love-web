# Sprint 16 | Don't Repeat Yourself
> I-love-web
- [Week 1](https://github.com/Lmikkers/i-love-web/blob/main/sprint-16.md#week-1)
- [Week 2](https://github.com/Lmikkers/i-love-web/blob/main/sprint-16.md#week-2)
- [Week 3](https://github.com/Lmikkers/i-love-web/blob/main/sprint-16.md#week-3)

## Week 1 
### 👩‍🎓 Leervragen
1. Wat is een morphological chart en waar gebruik je die voor?
2. Hoe geef je een custom propertie een juiste naam/ benaming? 
3. Waarom schrijf je custom properties in de `:root`? Dit kan ook in de `body tag`

   
### 📅 Weekplanning
#### Maandag
> 👩‍🎓 Wat ik heb geleerd:
- Workshop over Component as a Building Block gehad
- Met groepje gekeken naar welke componenten erzijn
- Component gekozen > [Zie issue](https://github.com/fdnd-agency/buurtcampus-oost/issues/199)
- Component analyseren > [Analyseren issue](https://github.com/Lmikkers/component-building-block/issues/1)

#### Dinsdag
> 👩‍🎓 Wat ik heb geleerd: 
- Aan mijn Morphological Chart gewerkt
- <img width="800" alt="Scherm­afbeelding 2024-11-13 om 15 44 33" src="https://github.com/user-attachments/assets/2a506a63-7b4d-4c72-bae5-075c7d0e097e">

#### Woensdag
> 👩‍🎓 Wat ik heb geleerd: Hoe je meer info kunt vinden over de font die je gebruikt en hoe je die kunt animeren
- Mentor voor de eerstejaars geweest, ik heb ze geholpen met custom properties, linken van stylesheets en de algemene structuur/benaming.
   - <img width="474" alt="Scherm­afbeelding 2024-11-18 om 09 52 19" src="https://github.com/user-attachments/assets/d2836284-4a4f-4cc9-8b45-46debaa47055">
- Workshop typografie in Web design

> Bron fonts uitzoeken: [wakamaifondue.com](https://wakamaifondue.com/)

### Vrijdag
> 👩‍🎓 Wat ik heb geleerd:
- Ik heb een ontwerp gemaakt in Figma over de morphologische kaart > [Zie issue ontwerpen](https://github.com/Lmikkers/component-building-block/issues/2)

### 📝 Aantekeningen | week 1
#### Component library (lib)
Een verzameling vooraf gemaakte, geteste en goed gedocumenteerde UI-componenten die eenvoudig kunnen worden gebruikt ub de gebruikersinterface van een product

> Quality Assurance!


***
## Week 2 
### 👩‍🎓 Leervragen
1. Hoe zet je een project online via Netlify en Svelte?
2. Hoe weet je wat voor structuut je wilt toepassen in je project?
3. Hoe kan ik chaos bedwingen in mijn code?

   
### 📅 Weekplanning
#### Maandag
> 👩‍🎓 Wat ik heb geleerd:
- Workshop Advanced Component Concepts [> Aantekeningen](https://github.com/Lmikkers/i-love-web/blob/main/sprint-16.md#advanced-component-concepts)
- Atomic Design Methode toegepast aan component > [Zie issue]()

#### Dinsdag
> 👩‍🎓 Wat ik heb geleerd:
-
-
#### Woensdag
> 👩‍🎓 Wat ik heb geleerd:
-
-
#### Donderdag
> 👩‍🎓 Wat ik heb geleerd:
-
-
### Vrijdag
> 👩‍🎓 Wat ik heb geleerd:
-
-
### 📝 Aantekeningen | week 2
> 📅  Ma 18 november 
## Advanced Component Concepts

> Svelte 5 > [What’s new in svelte 5](https://vercel.com/blog/whats-new-in-svelte-5)

### Structuur in jouw component library
- Doe super netjes want je wilt niet slechte dingen herhalen 👍
- DRY

### Chaos bedwingen door:…
> Afspraken (conventies) te maken over

- Naamgeving van componenten
- Naamgeving van Variaties en componenten
- Naamgeving van Properties binnen componenten
- Metanaamgeving: componenten, patronen etc.
- Indeling $lib folder

#### Metanaamgeving is…
- Geneste componenten
- Variaties op componenten
- Samengestelde componenten

### Structuur
#### Page-section-component
- Een volledige pagina, met verschillende sections die bestaan uit componenten.

#### Functional Layering: (Een manier van werken, hoeft niet specifiek zo)
- Inputs: knoppen, formulieren
- Display: tabellen, grafieken
- Navigation: navigatie, menu’s. Breadcrumbs, skip-to-content
- Structural: Layout elementen die structuur bieden, grids / containers

#### LEGO 🧱 
- Bricks: Kleine niet herbruikbare stukjes, icoon of tekstblok
- Blocks: Herbruikbare basis componenten, een knop of een afbeelding
- Assemblages: Gecombineerde componenten met een specifieke functie, formulier of een kaart
- Constructions: Complexe pagina-secties of templates, dashboard

#### Atomic Design: Methode om design systeem te creëren 
- Atoms: label, input, button
- Molecules: groep atomen bij elkaar, zoekformulier met een label, input en button
- Organism: groep moleculen die samen een sectie van je website vormen, een header balk met een zoekformulier
- Templates: een groep organismen die samen een paginatype vormen, een overzichtspagina of detailpagina
- Pages: ingevuld template met inhoud
￼

#### Presenter-Container
- Presentational components: UI-specifieke, stalles componenten die bepalen hoe data getoond wordt (bijvoorbeeld een img)
- Container component: Componenten die de presentational components van data voorzien en hun gedrag bepalen
- Compositions: Combinatie van containers en presentational components die specifieke pagina-secties vormen.

***

## Week 3 
### 👩‍🎓 Leervragen
1. Leervraag 1
2. Leervraag 2
3. Leervraag 3
### 📅 Weekplanning
#### Maandag
> 👩‍🎓 Wat ik heb geleerd:
- Ik ben mentor geweest voor de eerste jaar, ik heb met ze meegedaan met de opdracht Gestalt wetten onderzoeken. Ik heb de wet Proximity Law onderzocht. Nawal deed Similarity en Reyhan deed Common Region. Na dat we het hebben onderzocht hebben we het aan elkaar gepresenteerd en uitgelegd hoe je dit in je ontwerp kunt toepassen.
> Ik ben gaan kijken hoe ik Proximty Law kan toepassen in bieb in bloei, ik ben gaan kijken naar het formulier, door white space en groepering heb ik het geprobeerd duidelijker te maken voor de gebruiker.
  - ![image](https://github.com/user-attachments/assets/59583b41-d804-46db-b47c-54e0801a15c9)
- [Aantekeningen Proximity Law](https://github.com/Lmikkers/i-love-web/blob/main/sprint-16.md#law-of-proximity)

#### Dinsdag
> 👩‍🎓 Wat ik heb geleerd:
-
-
#### Woensdag
> 👩‍🎓 Wat ik heb geleerd:
-
-
#### Donderdag
> 👩‍🎓 Wat ik heb geleerd:
-
-
### Vrijdag
> 👩‍🎓 Wat ik heb geleerd:
-
-

### 📝 Aantekeningen | week 3
## Law of Proximity:
📅 25 november | Mentor

> Presenteer aan elkaar hoe je de wet kan gebruiken voor web design.

- Relatie met objecten die dicht bij staan > Zie Google zoek resultaten
- **Proximity = nabijheid**
- Proximity helpt gebruikers informatie sneller en efficiënter te begrijpen en te organiseren.

- White space
- Heading text dichterbij tekst dan de **spacing** er tussen
- **Formulier:** Related fields together > daardoor kun je beter scannen en makkelijker er doorheen￼
    - ![image](https://github.com/user-attachments/assets/7a08b585-b900-43d1-a9f4-4d19174b2ec8)
- **Far-away items:** Word vaker overheen gekeken (tunnel vision)
- Gerelateerde items dichtbij en white space gebruiken > Visual Design ++
- Groeperingen visueel duidelijk maken > bruikbaarheid vergroot, doordat gebruikers snel alleen die UI-elementen kunnen vinden

###  Illustrate the principle of proximity
* `Grids of Objects`
* `Lists of Text`
* S`hape and Space Dependencies`
* `Full Bleed Elements` : Layout structuur geven zodat het brein structuur snel kan waarnemen
*` Typography`: Space between


#### Bronnen
- [lawsofux.com/law-of-proximity](https://lawsofux.com/law-of-proximity/)
- [Proximity Principle in Visual Design, by Aurora Harley](https://www.nngroup.com/articles/gestalt-proximity/)
- [Gestalt Principles of Design — Proximity, by Christopher Butler](https://www.chrbutler.com/gestalt-principles-of-design-proximity/)

