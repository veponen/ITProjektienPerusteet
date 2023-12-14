# ITProjektienPerusteet
Wysockin kirjaa käyttäen     
Millainen on tyypillinen it-projekti. 
<!-- osallistumisohjeet https://docs.github.com/en/get-started/quickstart/contributing-to-projects -->

## Arviointi
*Tentti*: Wysockin kirjasta rajoitetut teemat 50 %   
*Paritehtävä*: Kommunikointi/viestintä-materiaali 25 %    
*Projektityö*: suunnitelman teko. Versionhallinnan suunnittelu erityispiirteenä 25 %
Työkalut. 
# Oppimistavoitteet
Ymmärrät projektimaisen 1) **työskentelyn periaatteet ja luonteenpiirteet**. Opit 2) **suunnittelemaan** ja dokumentoimaan **IT-projekteja**. Opit käyttämään *3) projektinhallintasovellusta projektin etenemisen seurantaan ja hallintaan.* 

* 1)**työskentelyn periaatteet ja luonteenpiirteet**: etätyö, ryhmätyö ja laadukas [kommunikointi/vuorovaikutus](./kommunikointi/README.md), näitä [tukevat työkalut](./toolChain/README.md).
* 2)**Suunnittelemaan ja dokumentoimaan it-projekteja**: projektityypin päättely, vaatimusten määrittelytyö, vaatimuspuu, tehtäväpuu, muu tarvittava dokumentaatio ja siihen liittyvät seurantaa/hallintaa (alla) tukevat työkalut (kuten VSCode, DrawIO) ja notaatiot (kuten Markdown, UML käyttötapaus)
* 3)**etenemisen seuranta ja hallinta**: ymmärretään vähän laajemmin tässä. [kanban, versionhallinta (git-branching)](./seurantaHallinta/README.md), burndown chart. Perinteisissä projekteissa (infrapuolella) ms-projectin kaltaiset gantt-chart esitykset.  

- [Projektin määritelmä ja käsitteet](#projektin-määritelmä-ja-käsitteet)
- [Projektityypit ja **hallintamenetelmät**](#projektityypit-ja-hallintamenetelmät)
- [Projektin **organisointi**](#projektin-organisointi)
- [Projektin resursointi](#projektin-resursointi)
- [Projektisuunnitelma](#projektisuunnitelma)
- [Projektin **hallinta**](#projektin-hallinta)
- [Projektin **riskienhallinta**](#projektin-riskienhallinta)
- [Projektin päättäminen](#projektin-päättäminen)
- [Projektinhallintasovellukset ja niiden käyttö](#projektinhallintasovellukset-ja-niiden-käyttö)

# Arviointikriteerit
TODO: avainasiat näistä linkitettävä tuonne oppimistavoitteisiin tai niistä tänne.      
Tyydyttävä 1      
Suunnittelet ja dokumentoit IT projektin. Projektin dokumentointi sekä **työkalujen ja menetelmien** hyödyntäminen on puutteellista.      
Tyydyttävä 2      
Suunnittelet ja dokumentoit IT projektin. Dokumentaatiosta on tunnistettavissa yrityksiä *ymmärtää* tehtyjä ratkaisuja **teorioiden ja toimintamallien** avulla. **Työkalujen ja menetelmien** hyödyntäminen on osittain puutteellista.       
Hyvä 3 (HUOM toimintamallit kuitenkin mukana)     
Suunnittelet ja dokumentoit IT projektin. Dokumentaatiossa kuvataan toteutusta **teorioiden ja käsitteiden** avulla. **Työkalujen ja menetelmien** *asiantuntevaan hyödyntämiseen on pyritty*.      
Hyvä 4 (HUOM: parhaat käytänteet + käytänteet =>toimintamallit)       
Suunnittelet ja dokumentoit IT projektin. Pyrit *parhaiden käytänteiden* hyödyntämiseen. Dokumentaatiossa on *käytetty **teoriaa ja käsitteitä** selittämässä* tehtyjä toimenpiteitä sekä tukemassa *esitettyjä väitteitä*. **Työkalujen ja menetelmien** hyödyntäminen on *asiantuntevaa*.        
Kiitettävä 5     
Suunnittelet ja dokumentoit IT projektin *parhaiden käytänteiden* mukaisesti. Dokumentaatiossa *selitetään ja perustellaan* tehtyjä toimenpiteitä **teorioiden, toimintamallien** ja **käsitteiden** avulla. Myös **vaihtoehtoisia** toteutuskelpoisia menettelytapoja on pohdittu. **Työkalujen ja menetelmien** hyödyntäminen on asiantuntevaa ja monipuolista.
<!-- 
## lyhennelmä arviointikriteereistä arvioinnin helpottamiseksi
* 1-2 projektin dokumentointi, työkalut ja menetelmät.
* 2 + teoriat ja toimintamallit
* 3 + käytetään dokumentaatiossa teoriaa ja käsitteitä
* 4 + pyrit parhaisiin käytänteisiin. 
* 5 + käytetty parhaita käytänteitä
-->  
# arviontikriteereistä poimitut teemat
1. [suunnittelu ja dokumentointi](#suunnittelu-ja-dokumentointi)
2. [teoriat ja käsitteet (toimintamallit)](#teoriat-ja-käsitteet-toimintamallit)
3. [työkalut ja menetelmät](#työkalut-ja-menetelmät)

# kommunikoinnin tärkeyden perustelut
Kaikki aiheet on syytä käsitellä/ajatella niin että painotetaan kommunikointia/interaktiota. Perustelut: 
1. 1)Wysocki: 80 %  tuotekehitysprojekteista on APM. APM projekteissa ja Extreme-projekteissa kommunikoinnin merkitys korostuu. 
2. 1)Wysocki: APM ja Extreme projektin epäonnistumisen todennäköisyys kasvaa selvästi jos projektin jäsenet eivät työskentele samassa tilassa. Teknologia auttaa, mutta onko se sama asia kuin oikeasti kasvotusten oleminen?
Epäonnistumisen Riskiä voidaan kuitenkin pienentää: "Openness and honesty are critical success factors.s359-360?", kuinka saadaan aikaan? <!-- chatgpt kysymys: how to forward Openness and honesty in complex project with distributed team? [hyvä vastaus](./opennesAndHonesty.md) josta voi edetä. -->
3. Agile manifesto https://agilemanifesto.org/
4. XP käytännöt: http://www.extremeprogramming.org/values.html

 
# Teemojen tarkempi käsittely 

## Projektin määritelmä ja käsitteet
Wysocki ykkösosa, project triangle, Ch 2 "what is project management"

## Projektityypit ja **hallintamenetelmät**
Wysockin nelikenttä ja sen alakohdat. Ch 2, fig 2.9 valinta
Perinteinen ja Agile
## Projektin **organisointi**
Wysockin nelikenttä ja sen alakohdat. Ch 2, fig 2.9 valinta
projektityypeittäin: perinteinen vs agile: projektipäällikön vs tiimin vastuut
RBS ja WBS

## Projektin resursointi
Vysocki: ihannetilanne vs. se mitä saadaan. 
Pohdintatehtävä: mitä se vaikuttaa projektityypin valintaan

## Projektisuunnitelma
PRojektin suunittelu: RBS ja WBS työskentely, harjoitukset. vertaisarvioinnit?
## Projektin **hallinta**
Wysocki: TODO katso missä. Kommunikointi ja sen suunnittelu. Raportointi. Agilet menetelmät. 
Kanban, versionhallinnan kytkentä kanban-tauluun. Burndown chart. 
tarkemmin  [työkaluista](#työkalut-ja-menetelmät)
## Projektin **riskienhallinta**

## Projektin päättäminen
hyväksymistestaus joka speksattu jo aloitettaessa. 
prosessi tähän.
## Projektinhallintasovellukset ja niiden käyttö 
Kanban, versionhallinta, burndown chart, gantt. 
tarkemmin  [työkaluista](#työkalut-ja-menetelmät)
# osaamistavoitteista kaivetut pääteemat
## suunnittelu ja dokumentointi
Wysockin kirjasta dokumenttipohjat ja järjestys
UML-opas: UC, uc-kuvaus, deployment kaavio.
RBS ja WBS puurakenteet ja WBS gant-kaavio. 
Projektin tai aliprojektin tyypin määrittely-palaverimuistio.
**Wysocki:n mukaan toiminta järjestyksessä (kuvadioista):**
* fig 6.1 project scoping process
    * COS-conditions of satisfaction määrittelydokumentti (fig 6.2) 
    * vaatimusmäärittely
    * POS project overview statement kirjoitus

## teoriat ja käsitteet (toimintamallit)
Wysockin kirja pääasiallinen teoreettinen lähde tällä kurssilla. 
IT-projektit on tietointensiivistä asiantuntijatyötä. 
Wysocki: hajautettu projektiryhmä riski, riskin mitigointi ja kommunikoinnin vaikutus siihen - toimintamalli, henkilökohtainen toiminta!

## työkalut ja menetelmät
IT-projektien työkalut ja menetelmät eivät ole pelkästään projektijohdon työkaluja. 
### seuranta ja suunnittelu
Kanban board ja gant chart tärkeimmät. 
Burndown chart
Markdown dokumentit
### Versionhallinta - seuranta
Tehtävien käytännön tekemisen seuranta. tehtävät linkitetään versionhallinnan kirjauksiin/vienteihin joko käsin tai automaattisesti (commit). Projektityöntekijät käyttävät päivittäin. Projektin johto seuraa.
ns. hajautettu versionhallinta GIT on tärkein. Hyvä opas [git-käyttöön Haaga-helian amk-sta](https://github.com/mruonavaara/git101#14-Github-Students-pack)

### kommunikoinnin ja työn tuki
Sähköposti, chat, editorin yhteis- ja parityöskentelyn tuki: word ja vscode. Obsidian-esittely
Työkaluja tärkeämpää on miten niitä käytetään: asiallinen kommunikointi. 
 <!--TODO: työnäyte josta pisteet vscode-tehtävä yhdessä opettajan kanssa pienissä ryhmissä, samalla versionhallinnan käyttöä.

 **Käydään tarkemmin vscode** -->

# Projektityypin valinta
Määritellään goal. 
Lähdetään kartoittamaan vaatimuksia
* arvoidaan vaatimusten täydellisyyden astetta
* arvioidaan omaa ymmärrystä aihesta eli vaatimuksista
    * vaatimukset ja oma ymmärrys vaikuttavat toisiinsa
* Mitä vähemmän ymmärrystä sitä agilempi PMLC malli
    * Myös käytettävissä olevan tiimin ymmärrystä arvioidaan.
* Mitä vähemmän kokemusta työstä ylipäätään => TPM PMLC malli

Arvioitavat kokemuksen lajit
* kokemus projektin toimialasta eli SME, subject matter expertize
* Kokemus käytetystä teknologiasta: ohjelmointi, testaus, työkalut
* Tiimin kokemus yhdessä toimimisesta, kuinka tuttuja tiimin jäsenet. 
* kokemus tehtävästä työstä yleensä: ohjelmointityöstä, konfigurointityöstä, testaustyöstä, eli roolin mukaisesta työstä. 


