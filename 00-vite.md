# Vite - asentaminen

Asennetaan ensin vite, HUOM luo tätä projektia varten **uusi tyhjä kansio** (esim. FE) erillään back-end projektista. FE ja BE elävät siis omissa projekteissaan:

### Setting up Vite for front-end (client) development

[Vite](https://vitejs.dev/guide/)

1. Create a new project with Vite in terminal

   ```sh
   # cd to your code folder
   npm create vite@latest
   # 1. type your project name
   # 2. Select a framework: -> Vanilla
   # 3. Select a variant: -> Javascript
   cd <project-name>
   npm install
   # start vite dev server
   npm run dev
   ```

1. Open the preview URL (<http://localhost:5173/>) in your browser and open developer tools (e.g. Chrome & [Chrome DevTools](https://developers.google.com/web/tools/chrome-devtools/))
1. Open the project folder in VS Code
1. To get started with a clean web app template:
   - edit or replace `index.html` file but do not remove `<script type="module" src="/main.js"></script>`
   - edit or replace `style.css` with your own styles
   - edit `main.js` file (note that the css file is imported in the js file instead of the html file `import './style.css';`). Everything else boilerplate code can be removed from the js file.
   - remove `counter.js` and image files because they are just examples

#### Publishing the website created with Vite

1. Stop the dev server (_ctrl-c_) if running
1. [Build](https://vitejs.dev/guide/build) the application `npm run build`

   - If you have more html files than just `index.html`, you need to add them to [configuration](https://vitejs.dev/guide/build#multi-page-app). Create a file called `vite.config.js` into your project's root folder:

   ```js
   // vite.config.js
   import { defineConfig } from 'vite';
   import { resolve } from 'path';


    export default defineConfig({
      base: './',
      build: {
        rollupOptions: {
          input: {
          main: resolve(**dirname, 'index.html'),
          home: resolve(**dirname, 'home.html'),
          },
        },
      },
    });
   ```

1. Copy all contents of `dist/` folder to the web server's public folder
   <br>

### Prettier

Lisää nyt projektin juureen prettier konfiguraatiotidosto, aivan kuten BE puolella.

[Prettier](https://prettier.io/)

```javascript
// .prettierrc.mjs
export default {
	semi: true,
	singleQuote: true,
	bracketSpacing: false,
	trailingComma: 'all',
};
```

# Testijulkaisu verkkolevylle

Julkaise reponsiivinen sivusi yllä olevien vite ohjeiden mukaan ja siirrä dist kansion sisältö verkkolevyllesi. Testaa että kaikki toimii kuten pitää.
