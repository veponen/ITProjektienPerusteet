# Ohjelmistostartupin työkaluketju-projekti
1. project goal/projektin tavoite vysocki sivut 178-180 mukaisesti: ei jargonia. liiketoimintalähtöinen.     
   versio 1. kehitetään ja/tai konfiguroidaan skaalautuva ohjelmistotuotteen kehitysympäristö.     
   versio 2. Kehitetään/valitaan ja konfiguroidaan ohjelmointia varten tuotekehitysympäristö jota voi laajentaa helposti (skaalautuvaa)
2. (5 p.) Vaatimuksien kartoitus (RBS): Vähintään 5 kappaletta joista väh. 1 ylimmällä tasolla.
   Lukuohje: (prio x) tarkoittaa prioriteettia x (P:) tarkoittaa priorisoinnin perustelua
```
   1. Työaikasuunnitelman teko
     1.1 RBS vaatimusten hallinnan automatisointi (priorisointi, uusien vaatimusten käsittely scope bank)
     1.2 WBS työtehtävien suunnittelun automatisointi
     1.3 Työmäärän arvioinnin automatisointi
   3. (prio 2) toteutuneen työn seuranta (P: työtovereiden ja johdon tarve tietää missä mennään) 
   4. Graafinen dokumentaatio oltava mahdollista.
   5. (prio 3) Tietomallin teon automatisointi ER-kaavio
   6. projektitehtävien vaatimusten ja henkilöstön osaamisen kohtaaminen automaattiseksi.
     6.1 työntekijöiden tehtävähistorian automaattinen seuranta.
         6.1.1 teknologia- ja
         6.1.2 tuoteosajärjestelmätasolla
         6.1.3 tiimitasolla (kuka on tehnyt kenenkin kanssa töitä?)
  7.  Automaattinen koodista vaatimukseen jäljitettävyys
     7.1 Testaus - feature - koodi - jäljitettävyys
     7.2 (prio 1) muutokset missä tahansa jäljitettävyysketjun osassa: vaikutuksien jäljitys automaattiseksi.
      (P: helpottaa vian etsintää ja muutosten vaikutusten näkemistä)
(seuraavaa vaatimusta ei asiakasorganisaatiolle voi ottaa mukaan)
8. vaatimustenmäärittelyn pohjalle annettua dokumenttia pitää pystyä kommentoimaan niin, että pystytään käymään keskustelua.

```
3. (5 p.)Projektin luokitus ja sen perustelu,
Projektin henkilökunta kokenutta. Tiedetään että hyvin moni tämän projektin osajärjestelmistä on valmiina.
Ne pitää vain konfiguroida "yhteen". Se on epävarmaa miten konfigurointi saadaan tehdyksi.
On vaatimuksia jotka ovat epäselviä projektin alussa. => agile. Goal on selvä.
valitaan Scrum jonka sisällä soveltuvin osin käytetään prototyping-mallia. reunaehto: Tiimi on max 4 henkeä samassa huoneessa. Siksi ei pidetä virallista dailyä, mutta scrum master pyrkii seuraamaan pysyykö tiimi tietoisena toistensa tekemisestä.

4. (2 p.) RBS perusteella tarvittavan tiedon kartoitus: mistä/mitä tietoa kerätään.

* 7.2 (prio 1) muutokset missä tahansa jäljitettävyysketjun osassa: vaikutuksien jäljitys automaattiseksi.
   * vaatimusdata
   * Tehtävädata
   * tiedot toteutetuista artefakteista.
   * yllämainittujen väliset linkit
     
* 3. (prio 2) toteutuneen työn seuranta
   * tehtävät
      * tehdyt tunnit
      * suunnitellut tunnit
  * speksi
  * vaatimus
  * työntekijä
    
* Vaatimusten yhdistetty tietomalli
   * vaatimus
   * tehtävä
   * artefakti
   * työntekijä
  
* SANASTO:
   * Artefakti: valmis suunnitteludokumentti, valmiiksi koodattu ohjelman osa, testaus-speksi, testiraportti
   * Speksi: spesifikaatio eli suunnitteludokumentti


5. (2 p.) RBS perusteella Karkea tietojärjestelmän osien kartoitus.
* jäljitettävyys-moduli: Seuraa artefaktien, vaatimusten ja tehtävien muutoksia ja "liputtaa" katselmoitavat asiat.
* Vaatimusten määrittely-moduli: vaatimusten tietojen kirjaukseen
* Tehtävä-moduli: tehtävien kirjaaminen (kanban toteutukset: github, gitlab, jira...)
* Työntekijä-moduli: työntekijän tietojen kirjaukseen
* spesifikaatio-moduli: (jira)

 ```
VILLIT MUISTIINPANOT
"Liikkennevalo" toimintaa muistuttava järjestelmä: kun hierarkiassa ylempänä olevaa (tai alempana?) komponenttia muutetaan, on sytytettävä punainen valo siihen linkitettyihin komponentteihin. Valon voi muuttaa vihreäksi vasta kun linkitetty komponentti on tarkastettu. 
 
SANASTO: 
komponentti: vaatimus, tehtävä, suunnitteludokumentti, valmis koodi, kerättävä tieto. 
 ```
6. (2 p.) Tehtävien kartoitus (WBS) tietojärjestelmän osien ja tarvittavan tiedon (edelliset kohdat) avulla.
* Suunnittelu/speksaus
  * Käyttöliittymät/frontend/UI/UX
     * vaatimusmäärittelymodulin UI 
  * Backend
    * Vaatimusten 7.2 ja 3. mukaisen tietokannan suunnittelu
  * tiedonhaku
     * tutki mitä "remoteja" on käytettävissä
     * tutki gitlab rajapinnat (eli miten sieltä saa tietoa ulos. Riittääkö git-rajapinta?)
        * tehtävätietojen osalta
        * työntekijöiden osalta
     * Spesifikaatioon tarkoitettujen modulien kartoitus.
* Toteutus
   * Jäljitettävyysmodulin tarkempi kuvaus/alustava tarvespeksi asiakkaan kanssa
   * Jäljitettävyysmodulin käyttöliittymä-prototyyppi
   * Vaatimusmäärittelymodulin UI toteutus
   * Vaatimusmäärittelymodulin backend toteutus
   * 
4. Testaus
   * vaatimusmäärittelymodulin testaus
   * ...
7. (5 p.) versionhallinnan haarojen (branch) ja toiminnan suunnittelu.
Tähän kuvausta mitä git-brancheja tarvitaan ja miksi
Tämän demoprojektin osalta: valitut viisi toteutustason vaatimusta.
Branchit      
* 7.2 (prio 1) muutokset missä tahansa jäljitettävyysketjun osassa (branchin nimi: jaljitettavyysKetju)
* 3. (prio 2) toteutuneen työn seuranta (branchin nimi: duuniSeuranta)
