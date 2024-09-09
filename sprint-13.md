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
  <li>Ik heb een Figma workshop gevolgd van CYD, <a href="#">link naar aantekeningen</a></li>
</ul>


Aantekeningen
