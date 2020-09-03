[tutorial](https://product.hubspot.com/blog/git-and-github-tutorial-for-beginners)  

`git init` - alustus, jos aloittaa uuden repon (repository/arkisto). Tehdään hakemiston sisällä. Tarvitsee tehdä alussa vain kerran aloittaessa projektin. Jos kloonaa projektin esim. githubista `git clone` avulla, ei tarvitse tätä tehdä.  

`git clone <url to .git repository>` - alustus, jos lataa repon esimerkiksi githubista. Esim `git clone https://github.com/khlsvr/katalogit.git`  

uusien tiedostojen lisääminen hakemistoon tai aikaisempien muokkaaminen tapahtuu normaalisti miten tekee muutoinkin tietokonetta käytettäessä.  

`git status` - tarkastele huomaako git uudet tiedostot  

`git add <filename>` - uusien hakemistoon lisättyjen tiedostojen lisääminen itse projektiin. Ja esim. yhden hakemiston kaikki tiedostot `git add hakemisto/* 

`git rm <filename>` - tiedostojen poisto.  

`git status` - tarkastele taas, tiedostot nyt lisätty  

`git commit -m "Your message about the commit"` - ajaa päivityksen ja tekee muutokset gittiin  

### githubin kanssa työskentely  

`git remote add origin https://github.com/khlsvr/mynewrepository.git` - asetetaan "originille" osoite. Tuohon asetetaan sen repon osoite (näkee mm. github.comissa repon sivuilta). Tarvitsee tehä kerran.  

`git remote -v` - näyttää mikä osoite on asetettu originiksi.  

`git push -u origin master` - työnnetään muutokset githubiin. Master on pääversio projektista. Projektista voi irroitaa erilisiä versioita, jolloin työnnöt saatetaan suorittaa eri paikkoihin.  

`git pull origin master` - vedä githubista muutokset omalle koneelle (sen masteriin).   

`git log` - listaa commit-historiaa  

`git config -l` - tsekkaa username ja tietoja

## Esimerkkitapauksia:  

### Uuden satkukuvan lisääminen:  

1. Tarkista, että omalla koneellasi oleva repo on ajan tasalla. Mene repon juurihakemistoon ja aja `git pull origin master` tai git-ohjelmalla valitsemalla hakemistossa "pull".
2. lataa ja tallenna kuva discordista repon hakemistoon oikealla nimellä.
3. "lisää" kuva ajamalla `git add <kuvatiedoston nimi>` tai git-ohjelmalla valitsemalla "add".
4. Aja muutokset `git commit -m "x kuvaa lisätty" tai git-ohjelmalla commitin avulla.
5. Työnnä muutokset githubiin ajamalla `git push -u origin master` tai git-ohjelmalla valitsemalla "push".
6. Voit käydä nettiselaimella tarkistamassa githubin sivujen kautta löytyykö lisäämäsi kuva oikeasta paikasta.


