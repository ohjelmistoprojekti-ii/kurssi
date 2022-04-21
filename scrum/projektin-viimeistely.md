# Projektin viimeistely

Onnistuneen projektin tärkeä vaihe on projektin dokumentointi, stabilointi ja luovutus. 

Luovutuskelpoinen projekti on siis stabiloitu ja dokumentoitu siten, että myös projektin ulkopuolinen taho pystyy hyödyntämään sitä helposti. Näissä opensource-henkisissä projekteissa käytämme projektin dokumentoimiseen GitHub-repositiorioon kirjoitettavaa **readme.md**-tiedostoa.

Projekti tulee myös stabiloida niin, että siinä ei ole ohjelman käyttöä estäviä virheitä, ja että tunnetut virheet on dokumentoitu esimerkiksi [GitHub-repositorioon issueina](https://help.github.com/en/github/managing-your-work-on-github/creating-an-issue).

Projektin luovutuksen yhteydessä on syytä myös käydä läpi vähintään tyypillisimmät tietoturvaongelmat, kuten repositorioon vahingossa päätyneet API-avaimet ja mahdollisesti suojaamattomat tai heikosti suojatut tietokannat.

## Dokumentointi

Kurssin puitteissa suosittelemme dokumentoimaan projektinne vähintään [markdown-muotoisen readme-tiedoston avulla](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes). Mikäli dokumentaatiostanne tulee kattava, voitte harkita readme-tiedoston lisäksi myös [**GitHubin wikiä**](https://docs.github.com/en/communities/documenting-your-project-with-wikis/about-wikis), [**GitHub Pages**](https://docs.github.com/en/pages) -sivustoa tai PowerPoint-kalvosettiä, joka voi olla mukana repositoriossanne.

Voitte halutessanne ottaa pohjaksi esimerkiksi [tämän readme.md-templaten](https://github.com/othneildrew/Best-README-Template). Tärkeintä readme-tiedostossa on tarjota ainakin projektin yleiskuvaus ja yleistason tekninen arkkitehtuuri sekä asennusohjeet. Lisäksi käytetyt teknologia ja kirjastot olisi hyvä esitellä, linkittää niihin liittyvät perustutoriaalit ja tarjota mieluusti myös muutama koodiesimerkki oleellisten kohtien käyttämisestä koodissa. Lisätkää readme-tiedostoon myös kuvaukset mahdollisista automaatioista (esim. GitHub actions).

Jatkokehitysajatukset on hyvä dokumentoida [GitHub-issueiden](https://help.github.com/en/github/managing-your-work-on-github/creating-an-issue) kautta ja viitata niihin readme.md-tiedostossa kuten edellä mainitussa [templatessa on tehty](https://github.com/othneildrew/Best-README-Template/issues?q=).

Lisäksi olisi hienoa löytää projektistanne joku timanttisin ydin, josta saattaisi olla eniten hyötyä ulkopuolisille ja tarjota se osa selkeästi käytettävän rajapinnan (API) kautta ulos. Tämä rajapinta voi olla toki mahdollisesti REST:iä, jos tämä ydin on luonteeltaan verkkopalvelu. Se voi olla myös dokumentoituja funktioita ja luokkia, jotka oikein käytettyinä tarjoavat ulkopuolisille kehittäjille jotain kiinnostavaa. Voit tutustua esimerkiksi [täällä](https://github.com/mitogh/react-native-image-placeholder) siihen, miten React Native Image Placeholder -paketti on dokumentoitu muita kehittäjiä ajatellen.

Tässä lisäksi esimerkkinä erään [aiemman vuoden projektin dokumentaatio](https://github.com/Myyyra/StashHunters) tällä kurssilla.


## Tietoturva

Projektin viimeistelyn ja luovutuksen yhteydessä on syytä varmistaa että siihen ei ole jäänyt ilmeisiä huolimattomuudesta tai puutteellisesta konfiguroinnista johtuvia tietoturvahaavoittuvuuksia.

Tyypillisiä konfigurointivirheitä ovat esimerkiksi heikot salasanat tai [täysin suojaamattomat tietokannat](https://snyk.io/blog/mongodb-hack-and-secure-defaults/), jotka ovat helppoja kohteita väärinkäyttäjille. Toinen tyypillinen virhe on lisätä yksityisiä API-avaimia versionhallintaan osana lähdekoodia, tai commitoida vahingossa ympäristömuuttujia sisältäviä .env-tiedostoja.

Mikäli olette projektin aikana valinneet esim. tietokannan tai ylläpitokäyttäjien salasanoiksi heikkoja salasanoja, ne on tässä vaiheessa syytä vaihtaa vahvemmiksi. Mikäli käytössänne on eri tuotteiden oletussalasanoja, niiden vaihtaminen on erityisen tärkeää.

Mikäli versionhallintaan on päätynyt salaista tietoa, kuten API-avaimia, suosittelemme lukemaan artikkelin [Removing sensitive data from a repository](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/removing-sensitive-data-from-a-repository). Lisäksi on tärkeää poistaa kaikki paljastuneet salaisuudet käytöstä.

Mikäli projektissanne on käytössä **MongoDB**, lukekaa esimerkiksi MongoDB:n artikkeli [How to Avoid a Malicious Attack That Ransoms Your Data](https://www.mongodb.com/blog/post/how-to-avoid-a-malicious-attack-that-ransoms-your-data).

**Firebase**:n kohdalla lukekaa artikkeli [Fix insecure rules](https://firebase.google.com/docs/firestore/security/insecure-rules) ja varmistakaa, että kukin käyttäjä voi muokata vain omaa dataansa, ja että esimerkiksi tunnistamattomat käyttäjät eivät voi lukea koko tietokannan sisältöä. Virheelliset käyttäjäoikeudet voivat johtaa esimerkiksi siihen, että kuka vain voi ladata koko tietokannan sisällön yksinkertaisesti käymällä tietokantanne osoitteessa `https://tietokanta.firebaseio.com/data.json`.

Huomioikaa oman projektinne arkkitehtuuri ja pohtikaa yhdessä, mitkä ovat projektinne potentiaalisia riskitekijöitä, ja miten voitte minimoida riskejänne. On toivottavaa, että tietoturvaa on huomioitu projektin aikana esimerkiksi [SQL-](https://owasp.org/www-community/attacks/SQL_Injection) ja [XSS-](https://owasp.org/www-community/attacks/xss/)injektioiden osalta, mutta myös näiden suhteen on hyvä varmistaa, että vahinkoja ei ole päässyt tapahtumaan. Tietoturvan arvioinnin osalta voi olla hyödyllistä käydä esimerkiksi [OWASP Top Ten](https://owasp.org/www-project-top-ten/) -lista läpi, ja arvioida eri tyyppisten haavoittuvuuksien merkitystä omassa ohjelmistossa.
