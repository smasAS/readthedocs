--- 
title: Best practice
---

# Sette generelle innstillinger

En god regel er å alltid starte med å sette globale innstillinger (farger, fonter, knapper o.l) og dette justeres på to steder:

**1. Tilpass**  
BeaverBuilder theme gir oss mange muligheter for justeringer via funksjonen "Tilpass". Det vi som regel bør endre på her er følgende ting som ligger under "Generelt": bakgrunn, uthevingsfarge, overskrifter, tekst og knapper.

<div style="padding:55.05% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/354204953?autoplay=1&loop=1&title=0&byline=0&portrait=0" style="position:absolute;top:0;left:0;width:100%;height:100%;" frameborder="0" allow="autoplay; fullscreen" allowfullscreen></iframe></div><script src="https://player.vimeo.com/api/player.js"></script> <br>

**2. Globale innstillinger i BB**  
BeaverBuilder pluginen gir oss mulighet til å justere på globale innstillinger via "Verktøy". Ofte trenger man ikke å røre dette, men noen ganger kan det være greit å endre f.eks __maks sidebredde__ og responsive __breakpoints__.

<div style="padding:55.05% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/354205783?autoplay=1&loop=1&title=0&byline=0&portrait=0" style="position:absolute;top:0;left:0;width:100%;height:100%;" frameborder="0" allow="autoplay; fullscreen" allowfullscreen></iframe></div><script src="https://player.vimeo.com/api/player.js"></script> <br>

# Endre header og footer

Dette gjør vi ved hjelp av BeaverThemer. Alphamal kommer med flere ferdige alternativer til dette.

# Egen CSS og JS

All CSS og JS som vi selv legger inn skal enten legges til via **Globale innstillinger** eller via en modul (om modulen har mulighet for å legge til dette).

# Globale elementer

Mye av det vi laget kan godt lages som **globale rader, kolonner eller moduler**.  

Har vi f.eks. en standard sidetopp, som skal se lik ut på alle sider, så bør det brukes et globalt element for å oppnå dette. På denne måten sparer vi oss mye tid om det skulle komme noen justeringer i etterkant - da trenger vi bare å gjøre justeringer __ett sted__ og ikke på absolutt alle sider hvor samme sidetoppen er brukt.

## Hvordan lage en global sidetopp

1. Start med å sette opp sidetoppen på en vanlig side ved hjelp av BB.
2. Bruk __themer connections__ for å koble til f.eks sidetittel til en tittel-modul + eventuelt fremhevet bilde som bakgrunnsbilde.
3. Lagre den aktuelle raden / kolonnen / modulen som global.
4. Nå kan du dra inn det globale elementer hvor enn du trenger å bruke det.

<div style="padding:54.5% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/355545316?autoplay=1&loop=1&title=0&byline=0&portrait=0" style="position:absolute;top:0;left:0;width:100%;height:100%;" frameborder="0" allow="autoplay; fullscreen" allowfullscreen></iframe></div><script src="https://player.vimeo.com/api/player.js"></script><br>

# Lage sidemaler
For innlegg, sider, custom post types, arkiver, søk o.l. kan man lage en sidemal ved hjelp av Beaver Themer. I kombinasjon med å bruke Advanced Custom Fields og [field connections](https://kb.wpbeaverbuilder.com/article/388-field-connection-basics-themer), så har vi mulighet til å få til det aller meste.