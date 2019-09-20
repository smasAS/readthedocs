--- 
title: Retningslinjer
---

Her er retningslinjer for hvordan man bør gå frem og hva man bør tenke når man bruker Alphamal for å bygge et nytt nettsted.

# Sette generelle innstillinger

En god regel er å alltid starte med å sette globale innstillinger (farger, fonter, knapper o.l) og dette justeres på to steder:

**1. Tilpass**  
BeaverBuilder temaet gir oss mange muligheter for justeringer via funksjonen "Tilpass". Det vi som regel bør endre på her er følgende ting som ligger under "Generelt":  

- Bakgrunn  
- Uthevingsfarge  
- Overskrifter  
- tekst og knapper  

Legg merke til at man også har responsive innstillinger her.

<div style="padding:55.05% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/354204953?title=0&byline=0&portrait=0" style="position:absolute;top:0;left:0;width:100%;height:100%;" frameborder="0" allow="autoplay; fullscreen" allowfullscreen></iframe></div><script src="https://player.vimeo.com/api/player.js"></script> <br>

**2. Globale innstillinger i BB**  
BeaverBuilder pluginen gir oss mulighet til å justere på globale innstillinger via "Verktøy". Ofte trenger man ikke å røre dette, men noen ganger kan det være greit å endre f.eks **maks sidebredde** og responsive **breakpoints**.

<div style="padding:55.05% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/354205783?loop=1&title=0&byline=0&portrait=0" style="position:absolute;top:0;left:0;width:100%;height:100%;" frameborder="0" allow="autoplay; fullscreen" allowfullscreen></iframe></div><script src="https://player.vimeo.com/api/player.js"></script> <br>

# Endre header og footer

Dette gjør vi ved hjelp av BeaverThemer. Alphamal kommer med flere ferdige alternativer til dette.

# Egen CSS og JS

All CSS og JS som vi selv legger inn skal enten legges til via **Globale innstillinger** eller via en modul (om modulen har mulighet for å legge til dette).

Når man legger til CSS/JS i *globale innstillinger (cmd + U)* vil dette gjelder globalt for hele nettstedet. Det finnes også noe som heter *Oppsett CSS & Javascript (cmd + Y)* men denne skal vi unngå å bruke, da kode som legges inn her kun gjelder for den aktuelle siden du er inne å redigerer på.

## Retningslinjer for bruk av CSS
- Style kun klasser og ikke ID'er
- Style kun klasser som er "faste" (laget av deg selv eller fast i en modul) og ikke de som er genersik opprettet.  
<small>BB lager mange genersike css-klasser som f.eks ligner på *fl-node-5bb4998c4461c*. Disse er genersik laget og kan plutselig endre seg om noen gjør en justering her eller der. Derfor legger vi heller inn våre egne klasser, som vi vet at ikke kommer til å endre seg (eller bruker klasser fra en modul som du ser at ikke er opprettet genersik).</small>
- Unngå bruk av ```!important```

# Globale elementer

Mye av det vi laget kan godt lages som **globale rader, kolonner eller moduler**.  

Har vi f.eks. en standard sidetopp, som skal se lik ut på alle sider, så bør det brukes et globalt element for å oppnå dette. På denne måten sparer vi oss mye tid om det skulle komme noen justeringer i etterkant - da trenger vi bare å gjøre justeringer **ett sted** og ikke på absolutt alle sider hvor samme sidetoppen er brukt.

## Hvordan lage en global sidetopp

1. Start med å sette opp sidetoppen på en vanlig side ved hjelp av BB.
2. Bruk [field connections](https://kb.wpbeaverbuilder.com/article/388-field-connection-basics-themer) for å koble til f.eks sidetittel til en tittel-modul + eventuelt fremhevet bilde som bakgrunnsbilde.
3. Lagre den aktuelle raden / kolonnen / modulen som global.
4. Nå kan du dra inn det globale elementer hvor enn du trenger å bruke det.

<div style="padding:54.5% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/355545316?loop=1&title=0&byline=0&portrait=0" style="position:absolute;top:0;left:0;width:100%;height:100%;" frameborder="0" allow="autoplay; fullscreen" allowfullscreen></iframe></div><script src="https://player.vimeo.com/api/player.js"></script><br>

# Lage sidemaler
For innlegg, sider, custom post types, arkiver, søk o.l. kan man lage en sidemal ved hjelp av Beaver Themer. I kombinasjon med å bruke Advanced Custom Fields og [field connections](https://kb.wpbeaverbuilder.com/article/388-field-connection-basics-themer), så har vi mulighet til å få til det aller meste.

# Favicon
Dette settes via *Tilpass -> Innstillinger -> Nettstedsidentitet -> Nettstedsikon*.
Bildet bør værre minst 512 x 512 piksler.

# Universell utforming (uu)
Ha __ALLTID__ uu i bakhodet når du setter opp eller lager noe. Tenk over at alt skal kunne være lestbart for noen som bruker skjermleser, bruker tastaturnavigering, svaksynte som trenger høy kontrast osv. Dette er også viktig å tenke over når man drar inn ferdige moduler (spesielt fra PowerPack). Det er ikke alle disse som blir godkjent innefor reglene til uu. [Les mer om uu her](/universell-utforming).