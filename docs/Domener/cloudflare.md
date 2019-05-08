---
title: "Cloudflare"
date: 2017-07-26 10:16:53
---
1. [Cloudflare for Wordpress](#01-Cloudflare-for-wordpress)

### 01: Cloudflare for Wordpress

1. Logg inn på riktig install på [wpengine](https://my.wpengine.com/)
2. Under Domains, legg inn riktig
  2.1 Domain og sett det som primary
  2.2 Sett opp redirect til det nye domenet fra det gamle
3. Logg inn på [cloudflare](https://www.cloudflare.com/) med riktig konto
  3.1 Klikk på 'Add site' og legg skriv inn riktig domene
  3.2 Legg inn cname fra install på [wpengine](https://my.wpengine.com/)
  3.3 Legg inn 'www' som cname som peker til domenet
  3.4 Velg gratis betalingsplan
  3.5 Noter ned nameservers
4. Logg inn på [domeneshop](https://www.domeneshop.no/login) og velg riktig domene
  4.1 Legg inn nameserver fra cloudflare under navnetjenere
5. Klikk på 'Recheck Nameservers' på [cloudflare](https://www.cloudflare.com/)



![Cloudflare](../img/domener/dns-cloudflare-01.gif)

### Ferdig!

![Done](../img/goodjob.jpg)

