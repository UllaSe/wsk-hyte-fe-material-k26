# Responsiivinen suunnittelu, perusteet

Käydään perusasiat ensin läpi luennon kautta:

1. [Responsiivinen suunnittelu, ppt](https://docs.google.com/presentation/d/1_lgctjnQ9ktsoBKFvkcBd43cN8EuTQ6IhVtmW6ttTss/edit?usp=sharing)

<br>

Teemme tunneilla perusharjoituksia ja mediasääntöjä ihan uuteen tyhjään html pohjaan. Linkit joita käyn demon aikana läpi löytyy readme tiedostosta ja täältä: [Responsiivinen suunnittelu, LINKIT](03-linkkejä.md)

Kun olemme käyneet läpi teorian, muokkaa nyt vite projektisi sivuja responsiivisemmaksi. Kaiken ei tarvitse vielä toimia, mutta yritä korjata mahdollisimman paljon rakenteita jotka menevät pienessä koossa rikki.

### Tehtävä 1 - Responsiivinen Banner/Hero kuva

Lisää sivuillesi responsiivinen Banner/Hero kuva. Yritä tässä käyttää CSS Background ominaisuutta ja sovittaa kuva mahdollisimman mukautuvaksi alueeseen.

![image](images/desktop.png)

### Tehtävä 2 - Media Queries / Mediakyselyt

Lisää sivuillesi muutama breakpoint jossa muutat sisältöä sopimaan paremmin kyseiseen näyttökokoon. Joudut nyt katsomaan kokonaisuutta "content first" ajattelutavalla. Tee breakpointit niihin kohtiin, missä sisältö menee rikki tai tarvii korjailua.

- [Media Queries](https://www.w3schools.com/css/css_rwd_mediaqueries.asp)

Varmista että sisältösi mukautuu pieniin kokoihin. Tarkista että kuvat skaalaantuvat ja fontit mukautuvat sisällön mukaan. Varmista ettei sivu mene "rikki" missään vaiheessa.

Responsiivista navigaatiota (esim. burger menu) ei tarvitse vielä tehdä, mutta voit toteuttaa sen jos haluat. Varmista kuitenkin että navigaatio pienenee, menee vertikaalisesti tms. eikä mene rikki.

![image](images/mobile.png)

# Testijulkaisu verkkolevylle

Julkaise reponsiivinen sivusi alla olevien vite ohjeiden mukaan ja siirrä dist kansion sisältö verkkolevyllesi. Testaa että kaikki toimii kuten pitää.

#### Publishing the website created with Vite

1. Stop the dev server (_ctrl-c_) if running
1. [Build](https://vitejs.dev/guide/build) the application `npm run build`
   - If you have more html files than just `index.html`, you need to add them to [configuration](https://vitejs.dev/guide/build#multi-page-app). Create a file called `vite.config.js` into your project's root folder:

   ```js
   // vite.config.js
   import { dirname, resolve } from 'node:path';
   import { fileURLToPath } from 'node:url';
   import { defineConfig } from 'vite';

   const __dirname = dirname(fileURLToPath(import.meta.url));

   export default defineConfig({
   	build: {
   		rollupOptions: {
   			input: {
   				main: resolve(__dirname, 'index.html'),
   				test: resolve(__dirname, 'test.html'),
   				nested: resolve(__dirname, 'bmi/index.html'),
   			},
   		},
   	},
   	// Public base path could be set here too:
   	//base: '/~ullamu/hyte/',
   	base: './',
   });
   ```

1. Copy all contents of `dist/` folder to the web server's public folder
   <br>
