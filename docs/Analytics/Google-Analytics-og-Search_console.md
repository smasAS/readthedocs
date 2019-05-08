---
title: "Google Analytics og Search Console"
date: 2017-07-26 10:16:53
---
1. [Ny Search Console account](#ny-search-console-account)
2. [Ny Analytics property](#oppsett-av-ny-analytics-property)
3. [Innstillinger for Analytics](#innstillinger-for-analytics)

#  Ny Search Console account
1. Logg inn på [Search Console](https://www.google.com/webmasters/tools/) med hovedkonto
2. Klikk på legg til ny egenskap og skriv inn navnet på nettsiden
3. Velg last opp HTML-dokument som verifisering og last ned dokumentet
4. Last opp dokumentet over ftp til serveren
5. Verifiser domenet

![Ny Search Console account](../img/analytics/google-search-console.gif)

# Oppsett av ny Analytics property
1. Logg inn på [Analytics](https://analytics.google.com) med hovedkonto.
2. Velg riktig account og klikk på Admin.
3. Under Property klikk på dropdown menyen og 'Create new property'.
4. Legg inn rikig navn, url og tidssone

![Oppsett av ny Analytics](../img/analytics/analytics-01.gif)

# Innstillinger for Analytics
1. Admin > View > View Settings
  1.1 Huk av:       'Exclude all hits form known bots and spiders'
2. Admin > View > Custom Alerts lag en ny varsling med følgende innstillinger:
  2.1 Alert name:   'Ingen trafikk har blitt registrert det siste døgnet'
  2.2 Apply to:     'All Web Site Data'
  2.3 Period:       'Week'
  2.4 Huk av:       'Send me an email when this alert triggers'
3. Admin > Property > Tracking info > Data Collection
  3.1 Slå på:       'Enable remarketing'
  3.2 Slå på:       'Enable Advertising Report Features'
4. Admin > Property > Property Settings > Adjust Search Console
  4.1 Koble til riktig [Search Console profil](#ny-search-console-account)


![Innstillinger for Analytics](../img/analytics/analytics-02.gif)

### Ferdig!

![Done](../img/welldone.jpg)
