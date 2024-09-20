<h1>I love WEB sprint 13</h1>
<ul>
  <li><a href="#week1">Week 1</a></li>
  <li><a href="#week2">Week 2</a></li>
  <li><a href="#week3">Week 3</a></li>
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
  <li>Bezig geweest met het maken van animatie <a href="https://codepen.io/MrBlank/pen/JjXxovL">Bron envelop animatie</a></li>
</ul>

<h4>Donderdag</h4>
<ul>
  <li>Verder gewerkt aan squadpage en visitekaartje</li>
</ul>

<h4>Vrijdag</h4>
<ul>
  <li>In de ochtend gewerkt aan squadpage <a href="https://github.com/KaanKalmi/your-tribe-for-life-squad-page/issues/20">Link Github</a></li>
  <li><a href="#weloveweb1">We <3 Web Vasilis van Gemert</a></li>
  <li>Code review, feedback gegeven aan <a href="https://github.com/rutgerkock/your-tribe-for-life-profile-card/issues">Rutger</a> en <a href="https://github.com/amirnapoletano/SPRINT-13-your-tribe-for-life-profile-card/issues">Amirna</a></li>
    <li><a href="feedback1">Feedback</a> gekregen van Koop en Krijn, de aantekeningen hebben we in onze Teams neergezet</li>
</ul>

<h3 id="feedback1">Feedback:</h3>
<h4>Project Board:</h4>
<ul>
    <li>Readme vroeg opzetten, zodat iedereen hier aan kan meewerken tijdens het maken van het project, en zodat wanneer je er aan werkt mensen mee kunnen werken en kunnen lezen hoe ze het kunnen runnen wanneer ze bijv feedback willen geven</li>
    <li>Probeer om bij issues te zetten wat er gedaan moet worden, en achteraf ook wat je gedaan hebt (met evt een link naar een commit)</li>
    <li>Dan kun je uiteindelijk in retrospects verwijzen naar issues als bewijslast, en hoef je dit niet dan nog dubbelop ook in bijv een wiki te schrijven</li>
    <li>Bewijslast op een rijtje zetten en dergelijken doen we bij retrospect, tijdens de sprints zelf gewoon alles bijhouden in issues en pull requests wat je maakt, dan maak je de portflow en dergelijken in de retrospect.</li>
    <li>Als er taken zijn die je kan opsplitsen, vergeet er geen issue van te maken. Bijv bij design hebben we een checklist gemaakt waarin een paar elementen staan die gedesigned moeten worden, maar je kan miss beter bij ieder van deze een aparte issue maken</li>
    <li>Je kan tags toevoegen bij issues op je projectboard om bijvoorbeeld MOSCOW te onderhouden en zo prioriteiten te kunnen stellen, of bijvoorbeeld moeilijkheidsgraad per taak bij te houden, zodat je bij te grote/moeilijke taken deze kan opsplitsen in meerdere kleinere taken. Dit helpt ook bij plannen</li>
    <li><strong>MOSCOW op taken zetten!! dit heb je nodig voor vrijdag</strong></li>
</ul>
<h4>Code/design:</h4>
<ul>
    <li>Andersom denken bij dingen bijv verbergen of tonen, zodat als iemand javascript niet aan heeft staan, alles altijd zichtbaar is, en dit alleen dynamisch verborgen en getoond kan worden via javascript</li>
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
  <li>`svelte:window`</li>    
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


<hr>


<p><strong>Vrijdag: 13 sept </strong>🦉</p>
<h3 id="weloveweb1">We love web <a href="http://www.vasilis.nl">Vasilis</a> van Gemert</h3>

<h4>Achtergrond</h4>
<ul>
    <li>Opgeleid als kunstenaar</li>
    <li>Is half Grieks</li>
    <li>Liefde met het web begon omdat ie het tof vond, toffe dingen maken en gratis.</li>
    <li>Kan veel met het web, hij vind web van tegenwoordig erg SAAI</li>
    <li>Maak toffe dingen en zet er alt teksten bij</li>
    <li>Doel: laten zien dat je van alles kan maken en creatief kan zijn het web, maar gebruik wel alt tekst bv je kunt het altijd toegankelijk maken.</li>
</ul>

<h4>Pagina&rsquo;s die hij heeft gemaakt&nbsp;<br>Homepage:&nbsp;</h4>
<ul>
    <li>Update zijn website wanneer er iets nieuws uitkomt, zoals animaties, lettertype, css</li>
    <li>Gemaakt toen Flexbox uitkwam om te experimenteren</li>
    <li>CSS animaties, nieuw dan zet hij het in zijn website</li>
</ul>

<h4>Love Nonsense</h4>
<ul>
    <li>Favoriete website <a href="https://lovenonsense.com">https://lovenonsense.com</a><ul>
            <li>Liefde voor onzinnige dingen</li>
            <li>Poppetjes: 2010, is een lettertype, wat iemand heeft gemaakt &gt; nut van onzin</li>
        </ul>
    </li>
</ul>

<h4>Flipping things <a href="http://www.vasilis.nl/flipping-things">Vasilis/flipping-things</a></h4>
<ul>
    <li>Flipt schilderijen, met achterkant schilderij en voorkant</li>
    <li>Veel kleurtjes en gekke dingen</li>
    <li>Houdt van Eastereggs🐣</li>
</ul>

<h4>Clocks <a href="https://vasilis.nl/clocks/">allemaal klokkies</a></h4>
<ul>
    <li>Houdt van klokken maken: omdat het beweegt</li>
    <li><a href="http://www.vasilis.nl/greek-time">Vasilis/greek-time</a> -&gt; klok die precies de tijd geeft (+/- een uurtje) (daar begon zn onderzoek naar klokken)</li>
    <li><a href="http://www.vasilis.nl/binary-clock">Vasilis/binary-clock</a> -&gt; nerd klok die telt in binary -&gt; dingen flippen was nieuw toen hij het maakte (3D)</li>
    <li><a href="http://www.vasilis.nl/wowclock">Vasilis/wowclock</a> -&gt; WOW ⌚️</li>
    <li><a href="http://www.vasilis.nl/decimal-clock">Vasilis/decimal-clock</a> -&gt; moeilijk leesbaar, leuk concept</li>
    <li><a href="https://vasilis.nl/clocks/hsl-clock/02/">Vasilis.nl/clocks/hsl-clock/02/</a></li>
    <li><a href="http://Vasilis.nl/clocks/pix-clock/">Vasilis.nl/clocks/pix-clock/</a> -&gt; Toegankelijkheid &gt; hij heeft van elke foto een beschrijving gemaakt voor blinde mensen</li>
</ul>

<h4>Toegankelijkheid</h4>
<ul>
    <li><strong>HvA nieuw schoolgebouw:&nbsp;</strong>getest 100% toegankelijk &gt; theoretisch, maar is het totaal niet.</li>
    <li>Denk echt na en zorg ervoor dat mensen er echt iets mee kunnen</li>
    <li><strong>Screenreader:</strong>&nbsp;<ul>
            <li>Leest alle headings op</li>
            <li>Houdt het kort voor screenreaders en overzichtelijk</li>
            <li>Iconen, goede naam geven</li>
            <li>Laat zien dat screenreaders alles op lezen, heel het menu door etc. Duurt erg lang en werkt slecht<ul>
                    <li>Kun je oplossen door bv navigatie weg te halen</li>
                    <li>Mensen komen voor de content</li>
                </ul>
            </li>
        </ul>
    </li>
</ul>


<hr/>

<h2 id="week3">Week 3</h2>
<h3>Leervragen</h3>
<ol>
  <li></li>
  <li></li>
  <li></li>
</ol>

<h3>Week planning van wat ik heb gedaan:</h3>
<h4>Maandag</h4>
<ul>
  <li>Uitleg gekregen over <a href="#projectManagement">project management</a>, met epics, stories en tasks</li>
  <li>Planning poker gedaan op ons project. Hierdoor hebben we een betere blik gekregen op de taken en hoeveel tijd dit ongeveer gaat kosten. We hebben ze verdeeld in hoogtes van cijfers, in mijn aantekeningen leg ik uit hoe en wat <a href="#planningPoker">planning poker</a> is.</li>
  <li>MoSCoW, Must have, Should have, Could have and Wont have. Met deze methode hebben wij ons project board verdeeld. Door dit te doen konden we onze taken prioriseren. <a href="https://github.com/users/KaanKalmi/projects/10/views/1">ons projectboard</a></li>
</ul>
<h4>Dinsdag</h4>
<ul>
  <li></li>
  <li></li>
</ul>
<h4>Woensdag</h4>
<ul>
  <li>Nieuw project gekozen voor sprint 14</li>
  <li>Ons werk samen gemerged, dit bleek best lastig te zijn, kregen best veel conflicten
    <ul>
      <li><a href="https://github.com/fdnd-task/your-tribe-for-life-squad-page/commit/cd43d1a2a6fe9b8c08532d9b2fd8abaab0af01e5">Merge</a></li>
    </ul>
  </li>
  <li>Verder gewerkt aan mijn visitekaartje</li>
</ul>


<h2>Aantekeningen week 3</h2>
<h3 id="projectManagement">Project management</h3>
<h4>Epic &gt; Stories &gt; Tasks</h4>
<h4>Epics </h4>
<p>Een handige manier om werk te organiseren en een hi&euml;rarchie te cre&euml;ren. Het idee is om werk op te splitsen in opleverbare stukken, zodat grote projecten kunnen worden afgerond en klanten op regelmatige basis waarde krijgen. Epics helpen teams werk op te splitsen terwijl ze naar een groter doel werken.</p>

<p>Epics zijn dus grote stukken werk die worden opgesplitst in kleinere taken, die vervolgens in sprints kunnen worden voltooid. Dit helpt teams om gefocust te werken en regelmatig waarde te leveren.&nbsp;</p>

<p>Voorbeelden:</p>
<ul>
    <li>De website van ... optimaliseren in zoekmachines (Hema, kruidvat etc)</li>
    <li>De website van &hellip; verbeteren</li>
    <li>In een zin noemen van wat je in een project gaat doen</li>
</ul>

<p><strong>Stories:</strong></p>
<p>Dingen die je moet doen die onder een Epic vallen<br><br>Voorbeelden:</p>
<p>Een nieuwe e-commerce website lanceren voor&hellip;</p>
<ul>
    <li>Een winkelmand toevoegen</li>
    <li>Betalingsmogelijkheid toevoegen</li>
    <li>Een klantenserviceportal toevoegen</li>
</ul>
<p>Een bestaande website verbeteren voor&hellip;</p>
<ul>
    <li>Website sneller maken (-&gt; begin met testen)</li>
    <li>Website gebruiksvriendelijker maken (-&gt; testen)</li>
    <li>Website toegankelijker maken (-&gt; testen!!!)</li>
</ul>
<p><br><strong>User stories</strong></p>
<ul>
    <li>Als bezoeker, wil ik producten kunnen verwijderen uit mijn winkelmandje als ik iets gevonden heb wat beter past bij wat ik nodig heb.</li>
    <li>Als bezoeker, wil ik producten in mijn winkelmandje kunnen doen om overzicht te houden wat ik aanschaf.</li>
    <li>Als bezoeker, wil ik overzicht houden op het uit te geven bedrag zodat ik het gevoel heb in controle te zijn.</li>
    <li>Betalingsmogelijkheden toevoegen</li>
</ul>

<p>Met <strong>Userstories</strong> heb je meer grip op je project</p>
<ul>
    <li>Kan je taken maken?</li>
    <li>Heb je genoeg grip?</li>
</ul>

<p>Voorbeeld taken onder user story een winkelmandje toevoegen:</p>
<ul>
    <li>Database voor winkelmandje</li>
    <li>Overzicht winkelmandje tonen in HTML+CSS</li>
    <li>Producten verwijderen uit DB</li>
</ul>

<p>&mdash;&gt; Wees specifieker dan dit</p>
<h4>Voorbeelden:</h4>
<ul>
    <li>Interface ontwerpen voor het verwijden van producten. (Nadenken over elementen, semantiek, enz.)</li>
    <li>Interface ontwerpen voor het aantal producten aanpassen.</li>
    <li>Enz.&nbsp;</li>
</ul>

<h4 id="planningPoker">Planning poker</h4>
<p>Is een consensus-gebaseerde techniek voor het schatten. Leden van de squad geven schattingen door genummerde kaarten op tafel te leggen of op schrijven zonder hardop te zeggen.<br>Kaarten worden omgedraaid of besproken en de schattingen worden vervolgens gesproken.<br>Zo heb je als team door wat er moet gebeuren en krijg je een goed beeld van je taken.</p>
