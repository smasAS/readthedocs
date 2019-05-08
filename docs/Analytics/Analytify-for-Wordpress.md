---
title: "Analytify for Wordpress"
date: 2017-07-26 10:16:53
---

1. Logg inn og last ned siste versjon av analytify pro fra [Analytify.io](https://analytify.io/your-account/)
2. Legg inn følgende utvidelser på Wordpress
  2.1 Analytify
  2.2 Analytify Pro
  2.3 Analytify Dashboard Widget
3. Analytify > Innstillinger > Lisens
  3.1 Skriv inn lisensnøkkel
4. Logg inn på [Google API Console](https://console.developers.google.com)
  4.1 Ved Analycis API XX
  4.2 Klikk på Analytify og kopier Client ID og Client secret
5. Analytify > Innstillinger > Avansert
  5.1 Huk av "Ønsker du å bruke egne API nøkler"
  5.2 Skriv inn Client ID
  5.3 Skriv inn Client Secret
  5.4 Skriv inn Redirect URL (står i teksten under)
6. Legg inn Redirect URL i [Google API Console](https://console.developers.google.com) på samme prosjekt
  6.1 Klikk 'Save' to ganger (viktig)
7. Analytify > Innstillinger > Autentifisering
  7.1 Autentifiser med korrekt google konto
  7.2 Profil for innlegg: Velg riktig analytics konto
  7.3 Profil for kontroll panel: Samme analytics konto som over
  7.4 Hak av 'Skjul profiler' (viktig)
8. Analytify > Innstillinger > Kontrollpanel
    8.1 Vis Analytics til følgende roller: Legg til Editor og Shop Manager (hvis Woocommerce)

![Analytify for Wordpress](../img/analytics/analytify.gif)

### Ferdig!

![Done](../img/goodjob.jpg)
