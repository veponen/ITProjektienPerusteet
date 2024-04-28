# Perusteet it-projekteissa
Tähän perusteet. kaiken it-järjestelmien konfigurointiin, suunnitteluun, dokumentointiin ja tekemiseen liittyvän perus-kuvio. 
Tuosta pitää tehdä suomenkielinen versio: 
https://medium.com/semantixbr/how-to-get-more-productive-projects-using-agile-and-git-f48be9aad1c2

# Kanban käyttö
Erilaisia graafisia työkaluja on, ja teollisuudessa käytetään lähinnä Jiraa. Myös githubissa ja gitlabissa on kanban-työkaluja. Niistä ei saa riittävän helposti tapahtumalokeja. **Tämän puutteen takia** opintojaksoilla käytetään merkkipohjaista ratkaisua suoraan projektin reposistoryssa. [Käytetään todo.md nimeä ja aina samaa sisäistä rakennetta](./TODO.md), sen voi kopioida omaan projektiin. Tuota päivitetaan remoteen joka kerran kun sitä muutetaan, jotta muut projektin jäsenet saavat tiedon tilanteesta. Toki sitä voi päivittää myös suoraan githubissa.
Mallia ja lisätietoja voi katsoa myös [täältä](https://github.com/todomd/todo.md) ja [täältä](https://github.com/todomd/todo.md/blob/master/TODO.md)


Testaamaton graafinen git pohjainen [kanban taulu](https://marketplace.visualstudio.com/items?itemName=gordonlarrigan.vscode-kanbn) joka näyttää hyvin lupaavalta. 

# Edistyneempiä asioita
Yhteistyön teon työkalut. Eräs mahdollisuus:
* VSCode, Git, [Github](./github.md), DrawIO (DrawIO korvikkeet: PlantUML, UMLet ) JA Live Share
* Näillä pystyt tekemään pari- ja ryhmätöitä aika-paikka riippumattomasti. 
Vaihe 1: Asenna VSCode
## Draw-IO
* Asenna Draw.io Integration (Henning Dieterichs) plugin, tai UMLet (the umlet team) tai PlantUML (Jebbs).
    * tietenkin kaikkien tiimiläisten pitää käyttää samaa kaavionpiirtotyökalua. Suositan Draw.io-ta, siinä on eniten valmiita symboleja (more-symbols-nappi).
    * Huom: Draw.io-ta ei välttämättä pysty käyttämään "Live Share"-tilassa
* Luo tiedosto jonka tarkenteena on drawio, esimerkiksi: esimerkki.drawio
    * kun klikkaat tiedostoa VSCodessa, drawio-editori aukeaa automaattisesti. 

## MS Live Share
* Asenna Live Share (Microsoft), yhteisiä dokumentointi/koodaus-sessiota varten     
* Käyttö:     
    * sinun ohjeesi: Sovi yhteinen aika työparin kanssa, tee sillä hetkellä linkki, lähetä se linkki vaikka teams chatilla.
    * työparisi ohje, 
        * vaihtoehto 1: avaa linkki selaimeen klikkaamalla sitä. VSCode-käyttöliittymä avautuu. 
        * vaihtoehto 2: Kopioi linkki, mene VSCodessa live-share toimintoon, paina Join-nappia ja pasteta(liimaa) linkki esiin tulevaan osoite-laatikkoon.
    * Nyt toimii samaan tyyliin kuin word tai googledocs dokumentin yhteiseditointi
        * Lisäksi on kaikki koodaukseen liittyvät ominaisuudet mukana. 
        * kaikki muutokset tapahtuvat "hostin" koneella, ja hänen on huolehdittava muutosten viennistä "remoteen"
* Lisäksi ääniyhteyttä varten on käytettävä joko teamsia tai jotain muuta. 

## remote-tilin luominen ja käyttö: github
TODO laita nämä yleisohjeisiin kurssitemplateen. 
Tehtävät tallenteet: git asennus, github remote tilin luonti, github repositoryn kloonaus: olette saanut osoitteen. 
SSH-avainten teko
SSH-avaimen asennus githubiin omalle tilille
TODO
GIT tilin valmistelu omalla koneella: aseta gituser ja gitemail 
    Configure your Git username/email
    Open the command line.
    Set your username: git config --global user.name "FIRST_NAME LAST_NAME"
    Set your email address: git config --global user.email "MY_NAME@example.com"

## Git-peruskäyttö
### yhden kerran git clone
git clone <osoite-jossa-remote-on>
### peruskäyttö 
Seuraavia asioita tehdään jatkuvasti, kerrotussa järjestyksessä
editoit joitakin tiedostoja
lisäät ne "staging" alueelle: **git add** <tiedoston nimi kansiopolkuineen>
Teet niistä yhden muutoksen, kommitin: **git commit** -m"kuvaava nimi kommitille" 
haet muiden mahdollisesti tekemät muutokset remotesta: **git pull**
viet omat muutoksesi remoteen: **git push**


## Git (merge) conflict 
* tapahtuu kun teet "git fetch rebase" tai "git pull" ja käy huono tuuri.
* Joskus git ei osaa päätellä samaan paikkaan "yhtäaikaa" tehdyistä muutoksista että kumpi on oikea. 
* Tätä tilannetta kutsutaan nimellä "Git conflict" tai merge conflict. Ja kyllä siitä selviää. 
    * sattuu harvemmin, haluan osallistua niiden korjaukseen jos vain suinkin on aikaa, oppiakseni. **Tässä auttaa paljon VSCoden käyttö** (miten? arvaappa) 
* Selviytymistrategia 0. 
    * noudata gitin ohjeita konfliktin ratkaisussa 
* Selviytymis-strategia "kun mikään ei tunnu toimivan v. 1": 
    1. palaa aikaan ennen konfliktia, 
    2. ota oma konfliktin aiheuttanut tiedostosi talteen toiseen hakemistoon, 
    3. poista git-hakemistossa sen tiedoston muutokset, tee git pull tai fetch rebase uudestaan. 
    4. vertaa omaa ja gitistä tullutta tiedostoa, tee muutokset käsin uudestaan git-versioon, tee uusi kommitti + git push. 
* Selvitymis-strategia "kun mikään ei tunnu toimivan v. 2" (Nato code "Toni K")
    * omat muutokset talteen
    * Kloonaa repo uudestaan
    * tee uuteen klooniin muutokset
    * jatka töitä sillä pohjalla. 