<h1>I love WEB sprint 13</h1>
<ul>
  <li><a href="#week1">Week 1</a></li>
  <li><a href="#week2">Week 2</a></li>
  <li><a href="">Week 3</a></li>
</ul>

<h2 id="week1">Week 1</h2>
<h3>Leervragen</h3>
<ol>
  <li>Hoe kan ik Svelte kit leren en wat is dit? Hoe kan ik hier het beste mee beginnen</li>
  <li>Hoe kan ik het best een stappenplan maken voor het maken van complexere interacties</li>
  <li>Hoe kan aan de hand van de  i-love-web, mijn bewijslast goed te laten zien en opslaan</li>
</ol>

<h3>Week planning van wat ik heb gedaan:</h3>
<h4>Maandag</h4>
<ul>
  <li>Squads gemaakt, groepje gevormt met Kaan, Robin, YuJing en Koen</li>
  <li>Besproken wat we ongeveer wilde maken en afspraak gemaakt dat iedereen een schets maakt voor woensdag</li>
</ul>

<h4>Dinsdag</h4>
<ul>
  <li>Schets gemaakt en onderzoek gedaan naar sveltekit</li>
</ul>

<h4>Woensdag</h4>
<ul>
  <li>
    Schets gekozen
    <ul>
      <li><a href="https://github.com/KaanKalmi/your-tribe-for-life-squad-page/issues/3">Zie issue voor onze schetsen</a></li>
    </ul>
  </li>
  <li>Schets uitgewerkt (Robin)</li>
  <li>Taken verdeeld, d.m.v. componenten te verdelen</li>
</ul>

<h4>Donderdag</h4>
<ul>
  <li>Aan mijn component gewerkt brief formulier en aan mijn eigen visitekaartje begonnen, setup Sveltekit vooral neerzetten.</li>
  <img width="692" alt="screenshot van het brief formulier" src="https://github.com/user-attachments/assets/d4b3ee10-4da3-431a-b924-3989d6baef98">
</ul>

<h4>Vrijdag</h4>
<ul>
  <li>Feedback gegeven eerste jaars visitekaartje</li>
  <li>
    Feedback geschreven in issues jaar 1
    <ul>
      <li><a href="https://github.com/Ties7/your-tribe-profile-card/issues">Issue Ties</a></li>
      <li><a href="https://github.com/nmiaa/your-tribe-profile-card/issues">Issue Mia</a></li>
    </ul>
  </li>
  <li>Met groepje gezeten en onze componenten gepusht</li>
  <li><a href="https://github.com/fdnd-task/your-tribe-for-life-squad-page/commit/da2301c2dfc7db790e0b8db3f42ae31b7fe23d7f">Zie mijn push/ commit</a></li>
  <li>
    Feedback geven aan Squadpagina jaar 2
    <ul>
      <li><a href="https://github.com/Jesse-Kramer/your-tribe-for-life-squad-page/issues/2">Groepje van Jesse</a></li>
      <li><a href="https://github.com/zoepje/your-tribe-for-life-squad-page/issues/6">Groepje van Zoe</a></li>
    </ul>
  </li>
  <li>
    We hebben met zn alle ideeën besproken voor onze eigen visitekaartje. We hebben onze ideeën voor onze visitekaartje in onze eigen Github gezet als issue, we gaan elkaar feedback geven op het idee en ontwerp. <a href="https://github.com/Lmikkers/your-tribe-for-life-profile-card/issues/1">Mijn issue/ ideeën voor ontwerp</a>
    <ul>
      <li><a href="https://github.com/yujing-student/your-tribe-for-life-profile-card/issues/1#issuecomment-2337616494">Feedback Yu jing</a></li>
      <li><a href="https://github.com/KaanKalmi/your-tribe-for-life-profile-card/issues/1#issuecomment-2337619343">Feebdack Kaan</a></li>
      <li><a href="https://github.com/Robin1224/your-tribe-for-life-profile-card/issues/1#issuecomment-2337623496">Feedback Robin</a></li>
      <li><a href="">Feedback Koen (nog geven)</a></li>
    </ul>
  </li>
</ul>



<h2>Aantekeningen</h2>
<em>📅 3 sept</em>
<p>Aantekeningen van de presentatie over `Svelte` en `Svelte Kit` van Justus.</p>

<h3>Client side rendering uitzetten:</h3>
> Export let car = false

`(+ page.js in de root van de route folder) `


<h3>Mapjes svelte uitleg:</h3>
**Static** is public map (client side) 
- CSS >  global.css

**SRC** map meest belangrijkst > daar gebeurd het meeste in 


Handig om te weten
``` html
<body data-sveltekit-preload-data=“hover”>
      %Sveltekit.body%
</body>
```

> gebruikservaring is beter en lazy loading staat aan

**Routes** > daar staan alle pagina’s
**Lib** > shorthand voor library, daar staan de componenten in, voor hergebruik van componenten.

`+page.svelte` -> lijkt op `ejs` -> hier combineer je data met html
In dit `+page.svelte` bestand krijg je `html + css + js`

Npm run dev (server starten)

Css definiëren per pagina


<h3>Data ophalen:</h3>
Export let data (in je `+page.svelte`) (haalt data op)

`+page.server.js -> fetchjson -> functie load -> await -> return { persons: persons}`

In je routes mapje bijv. `[id] -> page.server.js + page.svelte -> filters zoals persons/id`

<h3>Routes aanmaken</h3>
Als je een map aanmaakt in het mapje routes met een page bestand maakt ie een route
In je `page.server.js` kan je data sturen naar deze page bestanden


<h3>Svelte installatie</h3>
<p>Open de terminal en volg onderstaande om een Sveltekit project aan te maken</p>
<ol>
  <li>
    npm create svelte@latest
    <ul>
      <li>Welcome to SvelteKit!</li>
    </ul>
  </li>
  <li>
    Where should we create your project?
    <ul>
      <li>(hit Enter to use current directory)</li>
    </ul>
  </li>
  <li>
    Directory not empty. Continue?
    <ul>
      <li>Yes</li>
    </ul>
  </li>
  <li>
    Which Svelte app template?
    <ul>
      <li>Skeleton project</li>
    </ul>
  </li>
  <li>
    Add type checking with TypeScript?
    <ul>
      <li>No</li>
    </ul>
  </li>
  <li>
    Select additional options (use arrow keys/space bar)
    <ul>
      <li>none</li>
    </ul>
  </li>
  <li>Your project is ready! (KLAAR)</li>
</ol>




<hr>




<h2 id="week2">Week 2</h2>
<h3>Leervragen</h3>
<ol>
  <li>Hoe kan ik het beste omgaan met Sveltekit en als ik iets niet snap dit dan opzoeken?</li>
  <li>Hoe werkt het uitladen van data van de API via Sveltekit?</li>
  <li>Hoe weet ik nou of ik een beetje bijloop? Aangezien de presentaties niet meer worden gedeeld en hoe kan ik dit goed bijhouden?</li>
</ol>

<h3>Week planning van wat ik heb gedaan:</h3>

<h4>Maandag</h4>
<ul>
  <li>Person card: Data uitgeladen van mijn id.</li>
  <ul>
    <li>Ik zag alleen met het pushen dat ik was vergeten eerder te pushen, dit wil ik voortaan wel gaan doen.</li>
    <li><a href="https://github.com/Lmikkers/your-tribe-for-life-profile-card/commit/fd847fc34a3d9a330eeea21639ab59f0b83ee49c">Zie commit</a></li>
    <li><a href="https://github.com/Lmikkers/your-tribe-for-life-profile-card/issues/2">Issue closed</a></li>
  </ul>
  <li>Ik heb een Figma workshop gevolgd van CYD, <a href="#workshopFigma">link naar aantekeningen</a></li>
  <li>
    Daarna zijn wij als groepje bezig geweest om ideeën op te doen voor onze squad page. Wij hebben een gezamenlijke Figma aangemaakt en daarin hebben wij inspiratie geplakt.
    <ul>
      <li><a target="_blank" href="https://www.figma.com/design/U3B7QUtyz6JV8pEQoQMkXT/Inspiratie-squadpage?node-id=1-3&t=XTkGg2IUDcDijNSZ-1">Link naar Figma</a></li>
    </ul>
  </li>
  <li>Daarna ben ik bezig geweest om componenten te ontwerpen voor de squad page, zoals: postzegel en envelop.</li>
  <li>We hebben in het bestand mapjes aangemaakt van wat we hebben geleerd vanuit de workshop: Inspo, Design, Components en Assets.</li>
</ul>

<h4>Dinsdag</h4>
<ul>
  <li>Verder gewerkt aan de componenten uitwerken en een breakdown schets gemaakt.</li>
  <li>Verder gewerkt aan mijn visitekaartje en ik heb wat schetsen gemaakt voor andere ideeën.</li>
</ul>

<h4>Woensdag</h4>
<ul>
  <li>Herhaling van progressive enhancement gehad en uitleg gekregen over creative coding.</li>
  <li>Geleerd hoe je een schoon Sveltekit project aanmaakt, met `fetch-node.js` en `export let cs = false`</li>
  <li>
    Aan squadpage verder gewerkt, in Figma wat dingen geprobeerd en een nieuwe branch aangemaakt om verder op Yu Jing haar werk te kunnen.      <ul>
      <li><a href="https://github.com/KaanKalmi/your-tribe-for-life-squad-page/tree/id-pagina-larrisa">Link naar nieuwe branch</a></li>
      <li><a href="https://github.com/users/KaanKalmi/projects/10/views/1?pane=issue&itemId=78625649">Issue persoon pagina [id]</a></li>
    </ul>
  </li>
  <li><a href="#progressiveEnhancement">Aantekeningen Justus: Progressive enhancement met Svelte</a></li>
</ul>


<h2>Aantekeningen</h2>

<h3 id="workshopFigma">Aantekeningen Figma workshop</h3>
<em>📅 09 sept</em>
<p><a href="https://www.figma.com/community/file/1414605941438286466">Link Figma workshop van CYD</a></p>
<ul>
  <li>Teksten uitrekken = cool</li>
  <li>
    Verdeel je werk d.m.v. het te verdelen in:
    <ul>
       <li>Inspo: Inspiratie zoeken, screenshots insta, Pinterest</li>
      <li>Design: Hier komt het volledige design te staan, je kunt ook v1. v2 gebruiken zodat je je proces opslaat.</li>
      <li>Components: hier zet je alle componenten neer die je nodig hebt</li>
      <li>Assets page: Mapje voor overzicht van foto's</li>
    </ul>
  </li>
  <li><b>Design system:</b> styleguide maar dan groter, kleuren, iconen, buttons, componenten</li>
</ul>

<h4>TIP: </h4>
<ul>
  <li>Maak in je groepje afspraken voor typografie, kleuren, etc</li>
  <li>Voor lettertype, kun je een eigen type aanmaken: Dit kun je doen door een nieuwe text style toe te voegen , zet px erbij zodat het extra duidelijk is in de naam</li>
</ul>

<h4>Typografie en kleuren:</h4>
<ul>
  <li>Niet te veel font stylen</li>
  <li>Lettersparing mee spelen</li>
  <li>Lineheight, tenminste 1.2, 120% (spacing in % want gaat mee met tekstformaat)</li>
</ul>

<h4>Grotes artboard</h4>
<ul>
  <li>Mobiel 375px max</li>
  <li>Desktop 1440px </li>
</ul>

<hr>

<h3 id="progressiveEnhancement">Aantekeningen Progressive enhancement met Svelte</h3>
<em>📅 11 sept</em>
<p><b>Enhancement:</b> Een strategie waar je gebaseerd op de browser features van de gebruiker extra dingen kan doen. Iedereen krijgt basisfunctionaliteit. Als iemand sneller internet/nieuwere browser enz. Krijgen ze een enhanced version.</p>

<h4>
  Creative coding <br/>
  ===  <br/>
  Progressive Enhancement (*should be) <br/>
  === <br/>
  content(html, kan server-side gerenderde html zijn) first
</h4>

<p><b>Progressive Enhancement:</b> content first</p>

<h4>Stappenplan: voor een schoon Svelte project</h4>
<ol>
  <li>Maak een tijdelijk kopie van de folder van de squadpage repo</li>
  <li>Installer een clean install van SvelteKit voor de squadpage</li>
  <li>Voeg in /routes/+page.js deze regel code toe `export let cs = false`</li>
  <li>Neem in /lib/fetch-node.js de code over uit hetzelfe bestand van je laatste node.js project van sprint 12</li>
  <li>Importeer deze function in /routes/+page.server.js</li>
  <li>Check aan de hand van het voorbeeld of je alles goed gedaan hebt</li>
  <li>Copy / paste jullie toegevoegde svelte code terug in /route/+page.svelte</li>
</ol>

<p><b>@supports</b> > feature detection zorgt ervoor dat de pagina css blijft werken</p>

<h4>Sveltekit creative coding live coding Justus</h4>
<ul>
  <li>Fetchjson bestand met zelfde code als die we al hebben</li>
  <li>Routes aanmaken</li>
  <li>+page.svelte data ophalen + checken of links geldig zijn</li>
  <li>Svelte for vs-code, svelte intellisense, svelte snippets</li>
</ul>

``` css
@supports (animation-timeline: scroll()) {
    ul li {
        view-timeline-name: --happy-scroller;
        view-timeline-axis: inline;
        view-timeline-inset: -10% -10%;
        animation-range: 25% 25%;

        animation: linear appear both;
        animation-timeline: --happy-scroller;
    }

    ul li a {
        animation: linear appear both;
        animation-timeline: --happy-scroller;
    }

    @keyframes appear {
        0% {
            rotate:-10deg;
            opacity:.1;
            scale:.5;
        }
        50% {
            opacity:1;
            scale:1;
            rotate:0;
        }
        100% {
            opacity: .1;
            scale:.5;
            rotate: 10deg;
        }
    }
  }
```

<h4>Creative coding met JS 👍</h4>
<a href="https://github.dev/joostf/squadpage-sveltekit/tree/creative-coding-csr">github repo met voorbeeld</a>

<p>
  Niet alles is op te lossen met css;<br/>
  Bijv. Als je iets creatiefs wil doen op basis van interactie met de gebruiker. Dan kan je met client-side-js de interface verder enhancen.</p>

<ul>
  <li>`svelte:window<`/li>    
  <li>`+page.js === export let csr = true` (Client side rendering van js aan/uitzetten)</li>    
  <li>`Static`, daar komt sveltekit niet aan</li>    
</ul>

``` js
 onMount(() => {
    console.log(document) // document is defined, because it's called in the onMount function
  })
```

<ul>
  <li>Door `onMount` te gebruiken kun je `client side console log` gebruiken, door de `onMount`</li>
  <li>Als je het wil doen net als vorig jaar, kun je dit doen door alles in de static folder te zetten, of om `onMount` te gebruiken.🐥</li>
  <li>Svelte transition module <a href="https://svelte.dev/docs/svelte-transition">(svelte docs)</a> 👍</li>
  <li>Pagina staggeren (inladen op scroll?) kan hier ook mee👽</li>
  <li>Dingen laten zien met checkbox en svelte.fade -> <a href="https://github.dev/joostf/squadpage-sveltekit/tree/creative-coding-csr">tadaaa</a></li>
</ul>
