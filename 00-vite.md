# Vite - asentaminen

Asennetaan ensin vite, HUOM luo tätä projektia varten **uusi tyhjä kansio** (esim. FE) erillään back-end projektista. FE ja BE elävät siis omissa projekteissaan:

[Vite](https://vitejs.dev/guide/)

[Asenna Vite näiden ohjeiden mukaan](https://github.com/mattpe/hyte-web-dev/blob/main/01-tools-env.md#setting-up-front-end-client-web-development-environment-using-vite)

# Esimerkkirakenne

```
vite-project/
├─ index.html
├─ about/index.html
├─ contact/index.html
└─ src/
  ├─ main.js
  ├─ home.js
  ├─ common/
  │ └─ nav.js
  └─ css/
    └─ style.css
```

# Vite config

```js
import { dirname, resolve } from 'node:path';
import { fileURLToPath } from 'node:url';
import { defineConfig } from 'vite';

const __dirname = dirname(fileURLToPath(import.meta.url));

export default defineConfig({
	build: {
		rollupOptions: {
			input: {
				main: resolve(__dirname, 'index.html'),
				nested: resolve(__dirname, 'bmi/index.html'),
			},
		},
	},
	// Public base path could be set here too:
	//base: '/~ullamu/hyte/',
	base: './',
});
```

Polut:

```html
<li>
	<a href="./" class="selected navlink">Koti</a>
</li>
<li>
	<a href="./bmi/" class="navlink">BMI laskuri</a>
</li>

<script type="module" src="/src/js/main.js"></script>
```

# Testijulkaisu verkkolevylle

Julkaise sivusi "asenna vite" ohjeiden mukaan ja siirrä dist kansion sisältö verkkolevyllesi. Testaa että kaikki toimii kuten pitää.

Voit siirtää tiedostot kätevästi webdisk.metropolia.fi palvelun kautta. Luomme SSH avainparin tuntien aikana koulun sisäverkossa. Tarvitset sitä muiden ohjelmistojen käyttöön.
