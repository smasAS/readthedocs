--- 
title: Ekstra funksjonalitet
---

# Legge til webfonter
Om man skal bruke en annen webfont enn Google Fonts (som er default i BB), så finnes det en måte å få lagt inn dette ved hjelp av vår egen plugin Alphamal Settings. Det er viktig at det gjøres på den måten, slik at fonten blir synlig alle steder hvor man kan velge fonter i BB.

1. Gå til *Alphamal settings -> Fonter*.
2. Trykk knappen "Legg til fontpakke".
3. Fyll ut feltene. Det kan legges inn flere fonter per fontpakke.
4. Husk å trykk knappen "Oppdater" for å lagre endringene.

<div style="padding:54.5% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/354201624?loop=1&portrait=0" style="position:absolute;top:0;left:0;width:100%;height:100%;" frameborder="0" allow="autoplay; fullscreen" allowfullscreen></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

---

# Legge til bildestørrelser
Å legge til egendefinerte bildestørrelser gjøres ved hjelp av vår egen plugin Alphamal Settings. Det er viktig at det gjøres på den måten, slik at bildestørrelsen blir synlig alle steder hvor man kan velge det i BB.

1. Gå til _Alphamal settings -> Bilder_.
2. Trykk knappen "Legg til bildestørrelse" og legg inn ønsket navn, bredde, høyde og om det skal croppes elle ikke. Gjentra prosessen om du skal lage flere.
3. Husk å trykk knappen "Oppdater" for å lagre endringene.
4. Bygg thumbnails på nytt for at endringen skal tre i kraft. Gjøres via _Verktøy -> Rebuild thumbnails_

<div style="padding:54.5% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/354200307?loop=1&portrait=0" style="position:absolute;top:0;left:0;width:100%;height:100%;" frameborder="0" allow="autoplay; fullscreen" allowfullscreen></iframe></div><script src="https://player.vimeo.com/api/player.js"></script> <br>

---

# Shortcodes

## Alphamal bg image

```
[alphamal-bg-image id="optional" class="optional" size="optional"]
```

Denne kjører ut en div med et bilde som bakgrunnsbilde. Veldig snedig å ha når man f.eks bruker BB sin innleggsmodul og velger tilpasset innleggsoppsett.

**Parametre**
- **id:** Post-ID til en annen post man vil ha bilde fra. Defaulter til fremhevet bilde på gjeldende post.
- **class:** Egendefinert klasse som man vil bruke for å style bildet. I utgangspunktet er det ingen klasse
- **size:** Navnet på en definert bildestørrelse. Defaulter til "medium"

**Eksempel på bruk**

Shortcode:
```
[alphamal-bg-image class="my-class" size="large"]
```

Resultat:
```
<div class="my-class" style="background-image:url('url-to-large-image.jpg');"></div>
```
