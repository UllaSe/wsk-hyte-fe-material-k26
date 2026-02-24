## HTML5 lomakkeet ja validointi

HTML5-lomakkeet ovat osa HTML5-standardia, ja ne tarjoavat kehittyneitä tapoja luoda ja hallita interaktiivisia lomakkeita verkkosivuilla. Ne mahdollistavat käyttäjien tietojen syöttämisen ja lähettämisen palvelimelle sekä tarjoavat käytännöllisiä ominaisuuksia, kuten tietojen validointi ja selainpuolella tapahtuva tarkistus.

HTML5-lomakkeet sisältävät erilaisia lomake-elementtejä, kuten tekstikenttiä, salasanakenttiä, valintanappeja, pudotusvalikoita ja muita. Niiden avulla käyttäjät voivat syöttää erilaisia tietoja, kuten tekstiä, numeroita, päivämääriä, sähköpostiosoitteita ja muita tietotyyppejä.

[Forms](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/form)

- **Tietojen validointi:** HTML5-lomakkeet tarjoavat mahdollisuuden asettaa validointiehtoja suoraan lomakekenttiin. Esimerkiksi voit määrittää, että sähköpostiosoitteen on oltava oikean muotoinen tai että tiettyjä kenttiä ei saa jättää tyhjiksi.

[Form validation](https://developer.mozilla.org/en-US/docs/Learn/Forms/Form_validation)

- **Tyylikäs käyttöliittymä:** HTML5-lomakkeet voivat sisältää uusia käyttöliittymäelementtejä, kuten kalenterin, värivalitsimen ja aikavalitsimen. Tämä tekee lomakkeista visuaalisesti houkuttelevampia ja käyttäjäystävällisempiä.

- **Tallentaminen selaimessa:** HTML5-lomakkeet voivat tallentaa osan käyttäjän syöttämistä tiedoista selaimen muistiin väliaikaisesti. Tämä voi auttaa käyttäjiä välttämään tietojen menetyksen esimerkiksi sivun päivittämisen tai vahingossa sivulta poistumisen yhteydessä.

Lomakkeita voi tyylitellä suhteellisen helposti, tosin osa, kuten radio-button kentät ovat hieman haastteellisempia. Useimmiten tyyylittelyyn käytetään myös **:valid** ja **:invalid** pseudoluokkia.
https://www.w3schools.com/css/css_form.asp

**_Varmista että sisäänkirjatumislomakkeessasi toimii validointi, joka vastaa taustapalvelun vaatimuksia. Näin saat minimoitua käyttäjän tekemät virheet kirjaantumisessa._**
