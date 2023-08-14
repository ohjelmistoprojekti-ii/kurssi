# Ohjelmistoprojekti 2, toteutus SOF007AS3A-3001

Tämä Git-repositorio sisältää Ohjelmistoprojekti 2 -kurssin dokumentaation ja tiedostot.

## Kurssin sisältö

Opintojaksolla opiskelijat suunnittelevat ohjelmiston oikeaan tarpeeseen. Opiskelijat:

1. Organisoivat oman ryhmänsä toiminnan.
1. Tutustuvat tarpeeseen, joka voidaan ratkaista ohjelmistolla.
1. Määrittelevät ja suunnittelevat ratkaisun tuotantoiteraatio kerrallaan.
1. Toteuttavat ja esittelevät tuotantokelpoisia ratkaisuversioita.
1. Julkaisevat ohjelmistoratkaisun.

Kurssin suoritettuaan opiskelija ymmärtää ongelman ratkaisemiseen tarvittavia ohjelmistokehittäjän taitoja. Hän kykenee ymmärtämään ja kuvaamaan tarpeita ja ehdottamaan niihin soveltuvia ohjelmistoratkaisuja. Hän osaa itsenäisesti lisätä osaamistaan aiemmin tuntemattomista teknologioista. Hän oppii arvioimaan ja valitsemaan avoimen maailman ongelmanratkaisuun soveltuvia teknologioita ja menetelmiä. Hän osaa ottaa vastuun jostakin toteutettavan ratkaisun osa-alueesta. Hän osaa jakaa hankkimaansa osaamista muille tiiminsä jäsenille. Opiskelija osaa tiimin jäsenenä toteuttaa tuotantokelpoisen ohjelmistoratkaisun ongelmaan.

Kurssin arviointi perustuu ryhmätyöskentelyyn, ryhmän lopullisen tuloksen tarkoituksenmukaiseen toimivuuteen sekä kurssin lopuksi yksilötyönä tehtävään esseeseen, jossa arvioidaan omaa ja ryhmän toimintaa.

Ohjelmistokehityksen teknologioita -kurssi toimii osin tämän kurssin teknisenä tukikurssina. Suosittelemme hyödyntämään kyseisellä kurssilla käsiteltyjä aiheita, kuten testausta ja jatkuvaa integraatiota, tämän kurssin projektissa.

Kurssin lopputulokset julkaistaan lähtökohtaisesti avoimella lisenssillä.

Katso myös:

* [opintojaksokuvaus](https://opinto-opas.haaga-helia.fi/course_unit/SOF007AS3A)
* [Scrum guides](https://scrumguides.org/)
* [Readme Driven Development](https://tom.preston-werner.com/2010/08/23/readme-driven-development.html)


## 📑 Aiemmin hankitun osaamisen tunnistaminen (AHOT)

Jos olet hankkinut tämän opintojakson mukaisen osaamisen työsi kautta, voit osoittaa osaamisesi tavanomaisen osallistumisen sijasta AHOT-menettelyllä. Osaamisen tunnistamiseksi ilmoittaudu tälle kurssille normaalisti, ja ole yhteydessä kurssin opettajiin AHOT-järjestelyjen osalta **viimeistään kurssin ensimmäisen viikon aikana**.

Tarkemmat ohjeet AHOT-käytäntöjen suhteen löydät [erilliseltä sivulta](./ahot.md).


# 📅 Kurssin aikataulu *(syksy 2023)*

Kurssista järjestetään keväällä 2023 kaksi toteutusta. Toteutuksen **SOF007AS3A-3001** yhteiset tapaamiset järjestetään viikoittain seuraavasti:

* 1\. ja 2\. periodi

    * Itsenäinen opiskeluaika **maanantaisin klo 14-16.45 luokassa 5006**.
    * Yhteiset tapaamiset **keskiviikkoisin klo 14-16.45 luokassa 5006**.


Itsenäisillä opiskelukerroilla opettajat eivät ole pääsääntöisesti tavoitettavissa.

Kurssille varattuina ajankohtina työskennellään projektin parissa scrum-kehyksen mukaisesti. Tavoitteenamme on työskennellä kolmen viikon sprinteissä, joita  mahtuu kurssille 4 kappaletta. Intensiivi- ja lomaviikkoja ei huomioida osana sprinttien kestoa.

Kunkin tiimin sprintin aloitukset ja katselmoinnit pyritään järjestämään toistuvasti samoina viikonpäivinä ja kellonaikoina, jolloin sprinttien pituudet pysyvät tasaisina.

Kurssin laajuus on 10 opintopistettä, [eli noin 270 tuntia](https://www.haaga-helia.fi/fi/ects-jarjestelma-ja-tutkintotodistuksen-liite-eli-diploma-supplement). Kevään aikana viikoittaiseksi työmääräksi tulee noin 17 tuntia. Tulet siis työskentelemään merkittävässä määrin myös yhteisten tapaamisten ulkopuolella.



## Sprint 0: Projektien käynnistys *(21.8.-3.9.)*

### 📅 23.8. tiimien muodostaminen

Kurssin [käytäntöjen ja tavoitteiden](./aloitustunti.md) käsittely.

[Esimerkkejä avoimen rajapinnan tarjoavista palveluista](avoimet-rajapinnat.md)

**Tehtävä**: avoimen datan lähteisiin ja avoimen lähdekoodin projekteihin tutustuminen.

* Jakautuminen tiimeihin. Tiimin tavoitekoko on 5 henkilöä.
* [Palvelujen kehittämisen menetelmät (haaga-helia.fi)](https://www.haaga-helia.fi/fi/tool-factory-menetelmat-palvelujen-kehittamiseen)

&nbsp;


### 📅 30.8. "define sprint"

Vision määrittelyn ja toteutettavan palvelun suunnittelun kick-off

[Double Diamond -menetelmä (www.thoughtworks.com)](https://www.thoughtworks.com/insights/blog/double-diamond)

* GitHub project -palvelun nopea intro
    * YouTube: [Plan and track projects closer to your code #DemoDays](https://youtu.be/SI1ra-XHWHM)
    * GitHub blog: [How we’re using projects to build projects](https://github.blog/2022-05-16-how-were-using-projects-to-build-projects/)
* Esimerkki määrittelydokumentista ja käyttäjätarinoista: [Form Autofill for Firefox Desktop](https://docs.google.com/document/d/1j31lNkc_OFNNoxKmOJX5LWrbLn5zD19ngwsQtq_edVc/edit)
* Projektin laajuuden estimointi: karkea arviointi käytössä olevasta ajasta ja odotetuista tuloksista

**Tehtävä**: define-vaiheen tulosten raportointi opettajille sunnuntai-iltaan mennessä. User storyjen tai taskien valinta ensimmäiselle sprintille. Scrum boardin jakaminen opettajille.

&nbsp;


## Sprint 1 *(4.-24.9.)*

Sprint 1:llä tiimit aloittavat itsenäisen työskentelyn projektin toteuttamisen parissa. Koko kurssin yhteisiä tilaisuuksia ei järjestetä, mutta ohjausta on saatavilla Teamsissa ja kampuksella lukujärjestyksen mukaisesti. Sprintti päättyy tiimikohtaisiin katselmointeihin.

&nbsp;


### 📅 6.9. Sprint 1:n käynnistys

Tiimit aloittavat itsenäisen työskentelyn projektien parissa. Opettajat tutustuvat tiimien backlogeihin ja keskustelevat/antavat palautetta suunnitelmista pääsääntöisesti Teams-kanavilla.

&nbsp;


### 📅 13.9.

Sprint 1 jatkuu. Tiimit työskentelevät itsenäisesti projektien parissa ja hyödyntävät opettajien ohjausta kutsumalla opettajat mukaan tiimin tapaamisiin.

&nbsp;


### 📅 20.9. Sprint 1 katselmoinnit

Kukin tiimi esittelee **sprintin tulokset** ja **ensimmäisen version dokumentaatiostaan** (readme). Tiimit pitävät itsenäisesti retrospektiivit, joiden perusteella työtapoja kehitetään seuraavaa sprinttiä varten.

Tällä sprintillä esiteltävä versio voi hyvin olla paikallisesti ajossa kehittäjällä, eli sen ei tarvitse toimia esimerkiksi pilviympäristössä tai fyysisellä mobiililaitteella.

**Sprint 2 planning**

Katselmointien jälkeen tiimit valitsevat käyttäjätarinat sprintille 2 ja tekevät niihin tarvittavat tarkennukset ja määrittelyt.

&nbsp;


## Sprint 2 *(25.9.-15.10.)*

### 📅 27.9. Sprint 2:n käynnistys

Tiimit työskentelevät itsenäisesti projektien parissa ja hyödyntävät ohjausta kutsumalla opettajat mukaan tiimin tapaamisiin.

&nbsp;


### 📅 4.10.

Sprint 2 työskentely jatkuu. Opettajat nimeävät jokaiselle tiimille **vertaisryhmän**, jotka **katselmoivat toistensa lähdekoodit** ja antavat palautetta demoissa.

Vertaisryhmät toimittavat toisilleen katselmointipyynnöt, jossa ovat rajanneet omasta projektistaan katselmoitavan osan.

[Koodin katselmoinnin ohjeistus](scrum/koodin-katselmointi.md).

&nbsp;


### 📅 11.10. Sprint 2 katselmoinnit

Kukin tiimi esittelee sprintin tulokset opettajille ja vertaisryhmille. **Mahdollisuuksien mukaan sovelluksen tulisi olla ajossa tuotantoympäristöä vastaavassa ympäristössä**, tai tuotantoympäristön tulisi olla vähintään valittu perustellusti. Tuotantoympäristö voi tarkoittaa esimerkiksi pilvipalvelua tai fyysistä mobiililaitetta.

**Vertaisryhmät** toimittavat toisilleen katselmointiraportit lähdekoodin katselmointien tuloksista.

Tiimit pitävät itsenäisesti retrospektiivit, joiden perusteella työtapoja kehitetään seuraavaa sprinttiä varten.

**Sprint 3 planning**

Katselmointien jälkeen tiimit valitsevat käyttäjätarinat sprintille 3 ja tekevät niihin tarvittavat tarkennukset ja määrittelyt.

&nbsp;


## Kurssin puolivälin itsearvioinnit

Kurssin ensimmäisen itsearvioinnin kirjoittaminen ja oman oppimisen pohdinta. Tarkemmat ohjeet ja aikataulun löydät kurssin Teams-kanavalta projektien loppuvaiheessa.

&nbsp;


## 16.-22.3. Intensiiviviikko

Ei kurssin yhteisiä tapaamisia.

&nbsp;


## Sprint 3 *(23.10.-12.11.)*

### 📅 25.10. Sprint 3:n käynnistys

Tiimit työskentelevät itsenäisesti projektien parissa ja hyödyntävät ohjausta kutsumalla opettajat mukaan tiimin tapaamisiin.

&nbsp;


### 📅 1.11.

Tiimit työskentelevät itsenäisesti projektien parissa ja hyödyntävät ohjausta kutsumalla opettajat mukaan tiimin tapaamisiin.

Vertaisryhmät toimittavat toisilleen katselmointipyynnöt, jossa ovat rajanneet omasta projektistaan katselmoitavan osan.

&nbsp;


### 📅 8.11. Sprint 3 katselmoinnit

Kukin tiimi esittelee sprintin tulokset opettajille ja vertaisryhmille.

**Vertaisryhmät** toimittavat toisilleen katselmointiraportit lähdekoodin katselmointien tuloksista.

Tiimit pitävät itsenäisesti retrospektiivit, joiden perusteella työtapoja kehitetään seuraavaa sprinttiä varten.

&nbsp;


## Sprint 4 *(13.11-3.12.)*

Tiimit pyrkivät viimeisessä sprintissä stabiloimaan projektinsa, eli he keskittyvät erityisesti toimintavarmuuden takaamiseen uusien ominaisuuksien jäädessä pienemmälle painoarvolle.

Sprintin tavoitteena on projektien lähdekoodien julkaisu, sekä sovellusten mahdollinen julkaisu sovelluskaupassa, npm:ssä tai web-palvelimella.

&nbsp;


### 📅 15.12. Sprint 4:n käynnistys

Tiimit työskentelevät itsenäisesti projektien parissa ja hyödyntävät ohjausta kutsumalla opettajat mukaan tiimin tapaamisiin.

&nbsp;


### 📅 22.12.

Tiimit työskentelevät itsenäisesti projektien parissa ja hyödyntävät ohjausta kutsumalla opettajat mukaan tiimin tapaamisiin.

Vertaisryhmät toimittavat toisilleen katselmointipyynnöt, jossa ovat rajanneet omasta projektistaan katselmoitavan osan. Viimeisessä sprintissä ei vertaiskatselmoida koodia, vaan projektin "yleisilmettä" painottuen erityisesti Git-repostitorioon ja dokumentaatioon.

[Ohjeita projektin viimeistelyyn (dokumentointi, stabilointi ja tietoturva).](scrum/projektin-viimeistely.md)

&nbsp;


### 📅 29.12. Projektien loppudemot

Sprint 4 päättyy kurssin loppudemoihin, joissa kukin tiimi esittelee tuloksiaan muille.

Muistakaa myös dokumentoida projektinne mahdolliset tunnettut puutteet ja bugit ([GitHub issueina](https://help.github.com/en/github/managing-your-work-on-github/creating-an-issue)).


&nbsp;


## Itse- ja vertaisarvioinnit

Kurssin itse- ja vertaisarviointien kirjoittaminen ja oman oppimisen pohdinta. Tarkemmat ohjeet ja aikataulun löydät kurssin Teams-kanavalta projektien loppuvaiheessa.

&nbsp;


------

Tämän sivuston ovat kehittäneet Teemu Havulinna ja Ismo Harjunmaa. Materiaali pohjautuu suuresti Ohto Rainion kurssimateriaaleihin.
