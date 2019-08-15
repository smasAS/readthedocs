--- 
title: Good to know
---

# Shortcodes

## Alphamal bg image

```
[alphamal-bg-image id="optional" class="optional" size="optional"]
```

Denne kjører ut en div med et bilde som bakgrunnsbilde. Veldig snedig å ha når man f.eks bruker BB sin innleggsmodul og velger tilpasset innleggsoppsett.

###Parametre
- **id:** Post-ID til en annen post man vil ha bilde fra. Defaulter til fremhevet bilde på gjeldende post.
- **class:** Egendefinert klasse som man vil bruke for å style bildet. I utgangspunktet er det ingen klasse
- **size:** Navnet på en definert bildestørrelse. Defaulter til "medium"

###Eksempel på bruk
Shortcode:
```
[alphamal-bg-image class="my-class" size="large"]
```

Resultat:
```
<div class="my-class" style="background-image:url('url-to-large-image.jpg');"></div>
```

# Legge til bildestørrelser
Å legge til egendefinerte bildestørrelser gjøres ved hjelp av vår egen plugin Alphamal Settings. Det er viktig at det gjøres på den måten, slik at bildestørrelsen blir synlig alle steder hvor man kan velge det i BB.

![Hvordan legge til bildestørrelser](../img/alphamal/bilder.gif)

# Legge til webfonter
Om man skal bruke en annen webfont enn Google Fonts (som er default i BB), så finnes det en måte å få lagt inn dette ved hjelp av vår egen plugin Alphamal Settings. Det er viktig at det gjøres på den måten, slik at fonten blir synlig alle steder hvor man kan velge fonter i BB.

![Hvordan legge til fonter](../img/alphamal/fonter.gif)