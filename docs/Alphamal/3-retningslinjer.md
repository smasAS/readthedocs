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

<div style="padding:55.05% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/354204953?title=0&byline=0&portrait=0" style="position:absolute;top:0;left:0;width:100%;height:100%;" frameborder="0" allow="autoplay; fullscreen" allowfullscreen></iframe></div><br>

**2. Globale innstillinger i BB**  
BeaverBuilder pluginen gir oss mulighet til å justere på globale innstillinger via "Verktøy". Ofte trenger man ikke å røre dette, men noen ganger kan det være greit å endre f.eks **maks sidebredde** og responsive **breakpoints**.

<div style="padding:55.05% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/354205783?loop=1&title=0&byline=0&portrait=0" style="position:absolute;top:0;left:0;width:100%;height:100%;" frameborder="0" allow="autoplay; fullscreen" allowfullscreen></iframe></div><br>

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

<div style="padding:54.5% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/355545316?loop=1&title=0&byline=0&portrait=0" style="position:absolute;top:0;left:0;width:100%;height:100%;" frameborder="0" allow="autoplay; fullscreen" allowfullscreen></iframe></div>br>

# Lage sidemaler
For innlegg, sider, custom post types, arkiver, søk o.l. kan man lage en sidemal ved hjelp av Beaver Themer. I kombinasjon med å bruke Advanced Custom Fields og [field connections](https://kb.wpbeaverbuilder.com/article/388-field-connection-basics-themer), så har vi mulighet til å få til det aller meste.

# Favicon
Dette settes via *Tilpass -> Innstillinger -> Nettstedsidentitet -> Nettstedsikon*.
Bildet bør værre minst 512 x 512 piksler.

# Universell utforming (uu)
Ha __ALLTID__ uu i bakhodet når du setter opp eller lager noe. Tenk over at alt skal kunne være lestbart for noen som bruker skjermleser, bruker tastaturnavigering, svaksynte som trenger høy kontrast osv. Dette er også viktig å tenke over når man drar inn ferdige moduler (spesielt fra PowerPack). Det er ikke alle disse som blir godkjent innefor reglene til uu. [Les mer om uu her](/universell-utforming).

# HTML5 markup
BB gjør det mulig å velge å wrappe rader, kolonner og moduler med HTML-elementer. Det er viktig å bruke riktige elementer for at både søkemotorer og skjermlesere skal kunne lese og forstå innholdet på nettsiden best mulig.
<div style="padding:55.05% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/362750858?title=0&byline=0&portrait=0" style="position:absolute;top:0;left:0;width:100%;height:100%;" frameborder="0" allow="autoplay; fullscreen" allowfullscreen></iframe></div><br>

## Forklaring på de mest viktigste HTML5 elementene
```<main>``` omslutter det dominerende innholdet på nettstedet, inkludert alt artikkelinnhold og andre relaterte seksjoner som utvider det sentrale temaet på siden, som f.eks. ```<article>``` og ```<section>```.

```<article>``` bør kun omslutte det viktigste innholdet på akkurat den siden du er på. Søkemotorer kan legge mer vekt på innholdet som er omsluttet av denne taggen, i tillegg til at skjermlesere kan finne ut hva som er hovedinnholdet på siden. Kan f.eks. omslutte ```<section>``` og ```<aside>```.

```<section>``` brukes for å dele opp innhold der det er natulig å det i forskjellige seksjoner. Forsiden er et sted hvor det ofte er bruk for dette. En seksjon må alltid ha sin egen overskrift med en heading-tag. Kan ligge inne i en ```<article>```.

```<aside>``` brukes for sidestilt innhold, som f.eks. innhold i en sidebar. Innholdet i en ```<àside>``` skal være relatert til det omkringliggende innholdet. Kan ligge inne i en ```<article>```.  
*Eksempel: En nyhetsartikkel har et felt hvor det står detaljer om forfatteren som har skrevet artikkelen. Dette kan legges i en ```aside```.*

```<nav>``` brukes for å markere navigasjon / menyer. Slik som hovedmenyen i ```<header>```, breadcrumbs, meny i ```<footer>``` o.l.

```<header>``` brukes hovedsaklig for header på selve nettstedet, men en ```<article>``` eller ```<section>``` kan ha sin egen ```<header>```.

```<footer>``` har SEO fordeler i forhold til at man kan definere bunntekstdelen av et nettsted, for eksempel bedriftsinformasjon og andre nyttige lenker, men kan også brukes i ```<article>``` eller ```<section>```.

### Basic oppsett med HTML5 markup
```
<header>
    <!-- Main header content -->
    <img src="logo.png" alt="Bedriftens logo" />
    <nav>
        <!-- Main navigation -->
    </nav>
</header>

<nav role="breadcrumbs">
    <!-- Breadcrumbs -->
</nav>

<main>
    <!-- Main content -->
    <article>
        <!-- The most important content to this page-->
        <header>
            <h1>The article heading1</h1>
        </header>
        <section>
            <h2>Section content</h2>
        </section>
        <section>
            <h2>Section content 2</h2>
        </section>
        <aside>
            <h3>Aside content relevant to the article content</h3>
        </aside>
        <footer>
            Footer content
        </footer>
    </article>

    <section>
        <h2>Section content not relevant to the main article content</h2>
        <aside>
            <h3>Aside content relevant to the section</h3>
        </aside>
    </section>

    <aside>
        <h2>I.e. sidebar content</h2>
    </aside>

</main>

<footer>
    <!-- Main footer content -->
    <nav>
        <!-- Footer navigation -->
    </nav>
    <aside>
        <h3>Aside content relevant to the footer content</h3>
    </aside>
</footer>
```

<script src="https://player.vimeo.com/api/player.js"></script>