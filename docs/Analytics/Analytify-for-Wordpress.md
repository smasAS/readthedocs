---
title: "Analytify for Wordpress"
date: 2017-07-26 10:16:53
---

1. Logg inn og last ned siste versjon av analytify pro fra [Analytify.io](https://analytify.io/your-account/)
2. Legg inn følgende utvidelser på Wordpress
	* Analytify
	* Analytify Pro
	* Analytify Dashboard Widget
3. Analytify > Innstillinger > Lisens
	* Skriv inn lisensnøkkel
4. Logg inn på [Google API Console](https://console.developers.google.com)
	* Ved Analycis API XX
	* Klikk på Analytify og kopier Client ID og Client secret
5. Analytify > Innstillinger > Avansert
	* Huk av "Ønsker du å bruke egne API nøkler"
	* Skriv inn Client ID
	* Skriv inn Client Secret
	* Skriv inn Redirect URL (står i teksten under)
6. Legg inn Redirect URL i [Google API Console](https://console.developers.google.com) på samme prosjekt
	* Klikk 'Save' to ganger (viktig)
7. Analytify > Innstillinger > Autentifisering
	* Autentifiser med korrekt google konto
	* Profil for innlegg: Velg riktig analytics konto
	* Profil for kontroll panel: Samme analytics konto som over
	* Hak av 'Skjul profiler' (viktig)
8. Analytify > Innstillinger > Kontrollpanel
	* Vis Analytics til følgende roller: Legg til Editor og Shop Manager (hvis Woocommerce)

![Analytify for Wordpress](../img/analytics/analytify.gif)

### Ferdig!

![Done](../img/goodjob.jpg)
