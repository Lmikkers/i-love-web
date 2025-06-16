# [`CSS` Weekly](https://css-weekly.com/)
> Hier "probeer" ik elke week kort de interessante dingen uit de CSSWeekly mail te noteren :)

## Fix Reading flow - flex
> [Issue #613](https://css-weekly.com/issue-613/)


Bij gebruik van `flexbox` of `grid` waar visuele ordening anders is dan de bronvolgorde (bijv. via order, row-reverse, grid-areas etc.) kan het onverwachte focus-volgorde-gedrag veroorzaken voor toetsenbordgebruikers. reading-flow lost dit op door die focus-volgorde af te stemmen op wat visueel wordt getoond 

**Oplossing**
> Leest columns links > rechts
``` css
  reading-flow: grid-columns
```

> Leest rows boven > beneden
``` css
  reading-flow: grid-rows;
```

***

## Creating Blob Shapes using clip-path: shape()
> [Linkje](https://frontendmasters.com/blog/creating-blob-shapes-using-clip-path-shape/?utm_source=CSS-Weekly&utm_campaign=Issue-613&utm_medium=web)

Met `clip-path` gekke vormen maken, vet, zie linkje
![image](https://github.com/user-attachments/assets/b16b475a-cabb-4988-a63e-4abc42d48d12)


***

## Margin trim
> [Issue #612](https://css-weekly.com/issue-612/) | 
> [Linkje Margin trim](https://webkit.org/blog/16854/margin-trim/?utm_source=CSS-Weekly&utm_campaign=Issue-612&utm_medium=web)

The margin-trim property lets you tell a container to trim the margins off its children — any margins that push up against the container. In one fell swoop, all of the margin space between the children and the container is eliminated.
`margin-trim`
![image](https://github.com/user-attachments/assets/529d43e5-219a-4c22-b6b2-b99c03d76145)

*** 

> Linkedin

## Accessible CSS Images
Je kunt nu in css `::before` pseudo elementen een `alt` geven. 
Dit kun je doen door:

``` css
.element::before{
  content: "😌" / "Dit is een smiley die aan het relaxen is"
}
```

***

## Trends
### `Apple` Liquid Glass
Nieuwe design van Apple is bekend, `liquid glass`. 
- [Introductie apple liquid glass ](https://www.apple.com/nl/newsroom/2025/06/apple-introduces-a-delightful-and-elegant-new-software-design/)
![image](https://github.com/user-attachments/assets/1d375d06-e2d7-40b6-bca6-3c8c29822964)
- Ik vind het er wel leuk uitzien, alleen zoals de foto hierboven vind ik het erg eentonig. Vraag me ook af of dit voor toegankelijkheid wel goed is? Aangezien heel veel wegvalt en dezelfde kleuren zijn. Maar denk dat Apple hier wel iets voor heeft gevonden.

![image](https://github.com/user-attachments/assets/1807d90e-422f-4fa9-9c69-3af92aed11f8)
- Ik vind glas effect wel wat hebben in het menu balkje, ook met scrollen ziet dit er leuk uit, speels. In safari ook goeie oplossing, hierdoor zie je meer van de pagina.

- **Design concept**: `Skeuomorphism`
> **Skeuomorphism** digital interfaces mimic real-world objects, using visual cues like texture, shadows, and shapes to make them feel familiar and intuitive to users

**Linkjes**
- [Adopting liquid glass](https://developer.apple.com/documentation/technologyoverviews/adopting-liquid-glass)
- [Human interface guidelines](https://developer.apple.com/design/human-interface-guidelines)
- [🎥 Meet Liquid Glass | Apple](https://m.youtube.com/watch?v=IrGYUq1mklk)
- [🎥 Get to know the new design system | Apple](https://m.youtube.com/watch?v=DS2ildqCrB0)
