---
title: "Google Tag Manager"
date: 2017-07-26 10:16:53
---
1. [Ny Tag Manager Container](#ny-tag-manager-container)
2. [Oppsett Wordpress](#oppsett-wordpress)

# Ny Tag Manager Container
1. Last ned siste versjon av [GTM smartsettings](https://trello.com/c/seWOEaIH/528-lister-for-publisering) fra trello
2. Logg inn på [Tag Manager](https://tagmanager.google.com/) med hovedkonto.
3. Finn account som starter med riktig navn og klikk på 'Create Container' i menyen.
4. Klikk på Admin > Import Container og last opp siste versjon av [GTM smartsettings](https://trello.com/c/seWOEaIH/528-lister-for-publisering)
5. Velg Exsisting > 'Default workspace' og bekreft opplasting
6. Rediger variablen 'Google Analytics' og legg inn korrekt Analytics ID
7. Publiser endringene med korrekt kommentar

![Ny Tag Manager Container](../img/analytics/tag-manager-01.gif)

# Oppsett Wordpress

1. Legg inn [DuracellTomi's Google Tag Manager for WordPress](https://nb.wordpress.org/plugins/duracelltomi-google-tag-manager/) på siden

2. Innstillinger > Google Tag Manager
	* Legg inn korrekt Tag Manager ID
	* Huk av 'Custom' under container placement

3. Basic Data > Visitors
	* Huk av 'Logged in status'
	* Huk av 'Logged in user role'

![Oppsett Wordpress](../img/analytics/tag-manager-02.gif)

### Ferdig!

![Done](../img/notbad.jpg)
