--- 
title: Good to know
---

# Shortcodes

## Alphamal bg image

```
[alphamal-bg-image id="optional" class="optional" size="optional"]
```

Denne kjører ut en div med et bilde som bakgrunnsbilde. Veldig snedig å ha når man f.eks bruker BB sin innleggsmodul og velger tilpasset innleggsoppsett.

Parametre
id: Post-ID til en annen post man vil ha bilde fra. Defaulter til fremhevet bilde på gjeldende post.
class: Egendefinert klasse som man vil bruke for å style bildet. I utgangspunktet er det ingen klasse
size: Navnet på en definert bildestørrelse. Defaulter til «medium»
Eksempel på bruk
Shortcode: [alphamal-bg-image class="my-class" size="large"]

Resultat:
```
<div class="my-class" style="background-image:url('url-to-large-image.jpg');"></div>
```