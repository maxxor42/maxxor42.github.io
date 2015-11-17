---
layout: post
title:  "Svar på frågor"
date:   2015-11-17 12:00:00
comments: true
categories: answers
---

För den här sidan har jag samlat includes och variabler samlade på `_main.scss`. Därifrån har jag använt Jekylls include-funktion för att inkludera andra scss-filer och däred skapa endast en css-fil. Jag har skapat separata sass-filer för varje enskild sidtyp, där jag samlat css specifik för dem. 

### What do you think of pre-compiling your CSS?

CSS-skrivande blir effektivare genom pre-compiling med SASS/SCSS. CSS-kod är ett trubbigt verktyg, så fort en sida är någorlunda komplex blir koden ofta oöverskådlig och svårläst. Med SCSS får en tillgång till fler verktyg och tekniker, som gör att en kan skriva mer komplex och överskådlig text.

Det går även att dela upp koden i separata sass-dokument, för att sedan lägga ihop dem till ett enskilt css-dokument i samband med compiling, för att undvika onödigt många requests till servern.

Det finns två nackdelar med att inte skriva CSS direkt. Dels behöver en compila koden för att göra ändringar, vilket innebär att även små förändringar kräver lite mer jobb. Den som vill läsa koden behöver tillgång till o-compilade cass-filer för att se hur css-en är skriven, det compilade css-dokumentet är inte läsbart av människor. 

### What do you think of static site generators?
SSI's är bra för mindre projekt där en behöver få upp en hemsida snabbt och enkelt, och där det inte är många inblandade i projektet. Eftersom inga databaser och CMS-er är inblandade i produktionen kräver de färre server-inställningar och mindre underhåll. Sidorna är även relativt säkra, eftersom det som finns på servern bara är sttiska filer finns inget lätthackat.

### What is robots.txt and how have you configure it for your site?
I robots.txt kan en förklara för sökmotorernas spindlar vad på webbplatsen som de kan inkludera i sin sökdatabas, och vad de bör låta bli att indexera.

På den här webbplatsen har spindlarna ska bortse från hela sajten, eftesom jag bara har gjor den för den här kursen och inte tänkt använda den som egen, riktig hemsida (än).

### What is humans.txt and how have you configure it for your site?
I humans.txt kan en skriva credits till de som arbetat med en webbplats. Sidan riktar sig främst till professionella inom webbproduktion, och innehåller information om skribenter, kodare, designers, samt om vilken software och teknik som används vid produktionen.

### How did you implements comments to blog posts
Jag använde disqus för att inkludera comment-funktionalitet i bloggposterna. Jag skapade ett konto och slängde in koden i en egen html-include. Jag har även gjort det möjligt att, i markdown-filen för de olika inläggen, ange ifall en vill eller inte vill att de enskilda posterna ska ha kommentatorsfält.

### What is Open Graph and how do you make use of it?
Open graph är en standard för att ange vad i en webbsida som är viktigast vid delning i sociala nätverk. Med OG går det att styra vad som dyker upp på facebooks wall eller i en Twitter-post när någon delar en bloggpost eller en webbsida.

Jag har lagt till og-kod för alla sidor på webbplatsen. OG-koden är dels webbadressen till sidorna, dels rubriken för sidan. Jag har egentligen inte använt några bilder på sajten, men har lagt till en bild på en söt hund för att testa att allt fungerar som det ska.
