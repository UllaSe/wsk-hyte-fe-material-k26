# Hyte - Web-sovelluskehitys - front-end

Ensimmäisen vuoden Ohjelmisto -kursseilla harjoiteltiin HTML/CSS peruskonsepteja itseopiskeluna. Tällä kurssilla ensin kertaamme, jonka jälkeen syvennämme HTML/CSS osaamista, sekä JS taitoja.

Kurssin lopputuotoksena rakennetaan terveyspäiväkirja-web-sovellus käyttäen tunneilla tehtyä back-end- ja front-end-sovelluksia lähtökohtana.

## Front-end, viikot 1-6

Front end osuus kurssista on rakennettu niin, että joka viikko keskitytään yhteen isoon konseptiin. Koko kurssin aikana yritämme rakentaa alla näkyvän esimerkin pohjalta mahdollisimman identtisen ja ennen kaikkea toimivan, responsiivisen sivuston hienovaraisilla animaatioilla ym. Viemme viikko viikolta kurssilla sivustoa pidemmälle ja lisäämme toiminnallisuuksia sekä vaatimuksia sen tekemiseen. Kurssin alustava viikkoaikataulu löytyy repon readme tiedostosta.

Demosivun kuvankaappaus:
![image](images/layout.jpg)

Inspiraatio tälle sivulle on saatu seuraavasta layoutista. Näytän kuitenkin sivustosta toimivan demon.

https://dribbble.com/shots/23369008-Gym-Fitness-Landing-Page

Asioita joita mm. käsittelemme tällä kurssilla ja lopullisessa sivustossa on oltava:

- HTMl, CSS ja Javacript
- REST, Fetch, Autentikaatio
- Oma sovellus, jossa Käytetty kaikkia perus asemoinnin käsitteitä
- Semanttiset elementit ja niiden oikeanlainen hyödyntäminen
- CSS Flexbox / Grid pohja sivustossa ja sen käyttö muutenkin asemoinnissa
- CSS Reset ajatus
- Hyvin mietityt CSS luokat, määrittelyt ja nimeämiset
- Responsiivisuuden eri keinot ja sen järkevä toteuttaminen
- Täysin validoitu ja puhdas koodi
- Visuaalinen suunnittelu ja sen hyödyntäminen layoutissa
- Käytettävyyden perusteet
- Modaalit, Dialogit
- Lomakkeet ja front-end validointi

Toisessa periodissa keskitymme projektin tekemiseen ja parannamme sivujen käyttökokemusta. Näistä lisää siis seuraavalla kurssilla.
<br>

# Tämän viikon fokus, kertaaminen: peruskäsitteet ja asemointi

Ensimmäisenä tehtävänä tällä viikolla on kerrata peruskäsitteitä. **Emme koske vielä flexbox/grid tyylittelyyn ensimmäisellä viikolla.** Tarkoitus onkin yrittää mimikoida jo olemassa olevaa designia ensin perinteisin keinoin. Ensimmäisellä viikolla saat siis käyttää kaikkea muuta, paitsi flexbox ja grid asemointia.

Jotta oppisimme tällä kurssilla uusia asioita, on sivuston teknologisiin ratkaisuihin tiukemmat kriteerit. Ensimmäisellä viikolla rakennamme sivustosta vain yhden osan. Lisäämme sisältöä stattisesti/dynaamisesti seuraavilla viikolla, viikko kerrallaan.

<hr>

## Viikko1 - Kertaus

Mahdollisuuksia eri html elementtien asemointiin sivuilla on monia, ja tämä onkin usein hankalimpia CSS konsepteja hallita. Perustasolla, sinulla on käytettävissä seuraavat:

- block layout / inline layout
- elementtien koon määrittely (pikselit, prosentit, sisältöön mukauttaminen)
- box-sizing (margin, padding, border)
- kelluttaminen (float)
- relatiivinen asemointi (relative positioning)
- absoluuttinen/ fiksattu asemointi (absolute / fixed / sticky positioning)
- keskittäminen (centering)

Ensimmäisenä päivänä harjoittelemme näitä asioita, löydät asemoinnin treenaamista varten, laatikko-harjoituspohjan täältä. Koodissa on mukana linkit asemoinnin eri käsitteisiin.

[Laatikkoleikki](harjoitukset/asemointi.html)

Näitä osittain korvaamaan ja helpottamaan onkin suunniteltu Flexbox ja CSS Grid käsitteet. Flex ja Grid toimivat molemmat mukavasti yhdessä, kummallakin on kuitenkin oat käyttötarkoituksensa. Näihin syvennymme kunnolla seuraavien viikkojen aikana.

### 1. TEHTÄVÄ – Palautettava viikkotehtävä

Ensimmäisellä viikolla saat käyttää siis vain perus asemointia, **ei flexbox, eikä grid asettelua**. Ensin teemme vain osan sivustosta. Aloitamme sivun about ja navigaatio-osuudesta. Huomaa, että sivujen pitää olla myös keskitetty.

Käytä sivuston esimerkkidesignia vain pohjana. Mieti oma hyvinvointiteemasi. **Käytä omia vaihtoehtoisia värejä sekä kuvia.**

![image](images/vk1.png)

## Tekniset vaatimukset

- Kirjoita HTML sekä CSS-koodi erillisiin tiedostoihin, jonka avulla luot sivustosi
- Opettele koodatessasi samalla Emmetin käyttöä
- Yhteystieto-osion takana näkyvä kuva on tehty css taustakuvana. Mikäli tämä on vielä hakusessa, käytä vain väriä.
- Saat tehtyä suorakulmaisista elementeistä ja reunuksista helposti pyöreitä/pyöristettyjä käyttämällä
  - [border-radius määrittelyä](https://www.w3schools.com/cssref/css3_pr_border-radius.asp)
  - [reunoja](https://www.w3schools.com/css/css_border.asp)
- Jos haluat käyttää varjostusta, eli Box-shadow ominaisuutta:
  - [box-shadow](https://css-tricks.com/almanac/properties/b/box-shadow/)
  - [box-shadow w3schools](https://www.w3schools.com/cssref/css3_pr_box-shadow.asp)
- Käytä ylänavigaation linkeissä pseudoluokkia ja tekstille joku muutos kun hiiren osoitin on kohdistettu linkin päälle, sekä kun sitä painetaan (ja pidetään pohjassa)
  - [CSS Pseudo-classes](https://www.w3schools.com/css/css_pseudo_classes.asp)
- Muista hyvät nimeämiskäytännöt

Navigaation tekemiseen voit käyttää valmista koodia, mutta muokkaa sitä sivuusi sopivaksi

- [Esimerkkinavigaatio](https://www.w3schools.com/css/css_navbar.asp)
- [MDN Nav Elementti](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/nav)

Lisäämme seuraavilla viikolla sivulle mm. responsivisuuden, nämä voi jättää toistaiseksi pois. Palautusohjeet löydät OMAsta.

<hr>

### HTML Validointi

Validointi, eli vahvistaminen on prosessi, jossa tarkistetaan, että prosessin kohde täyttää jotkin tietyt kriteerit. Kohde voi olla esimerkiksi tietokoneohjelma tai valmistusprosessi.

HTML validointi on käytännössä vähän samanlainen asia kun ESLintin käyttö. Kuten javascriptin, myös HTML-dokumentin kuuluu olla oikein muodostettu ja käyttökelpoinen.

Jotta kirjoittamamme koodi on standardin mukaista, on meidän ensin ymmärrettävä mitkä asiat muodostavat standardin

- HTML-koodihan on rakenteista tekstiä, joka muodostuu sisäkkäisistä ja perättäisistä elementeistä.
- Selaimet eivät näytä tunnisteita sellaisinaan vaan käsittelevät niitä teknisinä ohjeina, joiden mukaan sivun varsinainen sisältö tulee jäsentää.
- Oikeellisen dokumentin rakenne tarkastetaan dokumenttityypin mukaisesti.
- Dokumenttityyppi määrää muun muassa mitä elementtejä voi käyttää dokumentissa.
- Esim. HTML5 dokumenttityyppihän määritellään heti sivun alussa `<!DOCTYPE html>`
- Lue: https://www.w3schools.com/tags/tag_doctype.asp
- Dokumenttityyppi määrää myös mitkä elementit saavat sijaita minkäkin elementin sisällä ja mitä ominaisuuksia kuuluu millekin elementille.

World Wide Web Consortium, lyhyesti W3C on kansainvälinen yritysten ja yhteisöjen yhteenliittymä, joka ylläpitää ja kehittää WWW:n standardeja tai suosituksia kuten W3C niitä kutsuu. Uusimmat HTML standardit ja suositukset löydät täältä:

https://www.w3.org/standards/techs/html#w3c_all<br><br>

### HTML Validaattori

<img src="https://users.metropolia.fi/~ullamu/mdimages/validation.png" width="600">

Validaattori on ohjelma, joka tarkastaa koneellisesti dokumentin oikeellisuuden dokumenttityypin mukaan.
W3C Markup validaattorin löydät täältä:

https://validator.w3.org/

No miksi aina kannattaa validoida? Hyviä pointteja löydät W3Cn sivuilta seuraavasta linkistä, lue tämä läpi:

https://validator.w3.org/docs/why.html
<br><br>

### TEHTÄVÄ – Validoi HTML sivusi

Nyt kun olet lukenut HTML validoinnista, on aika myös käyttää validaattoria. Tehtävänäsi on validoida tekemäsi sivun koodi.

- Tarkista että html sivultasi löytyy dokumenttityyppi määriteltynä.
- Mene osoitteeseen: https://validator.w3.org/ ja validoi sivusi.
- Tarkista sekä korjaa mahdolliset virheet ja varoitukset:

<img src="https://users.metropolia.fi/~ullamu/mdimages/errors.png" width="600">

Tässä esimerkissä minulta puuttuu div-elementin sulku ja validaattori kehoittaa lisäämään lang=”en” attribuutin html elementille, sillä käytän sivulla englantia, enkä muita kieliä. (https://www.w3.org/International/questions/qa-lang-why) Virhe 2 korjaantuu automaattisesti sillä, että korjaan virheen kohdassa kolme, eli lisään puuttuvan div-elementin.

Korjauksen jälkeen:

<img src="https://users.metropolia.fi/~ullamu/mdimages/noerrors.png" width="600"><br><br>

## TEHTÄVÄ – Validoi myös CSS

Sama homma pätee myös CSS:n validointiin. Työkalun siihen löydät täältä:

https://jigsaw.w3.org/css-validator/

Validoi nyt sivusi CSS ja korjaa mahdolliset virheet.<br><br>
<br>
