# Todo -lista

Simppeli todo -lista appi, joka on rakennettu reactilla. 
Tämä sovellus on tehty pitkälti oheisen tutorialin mukaan: 

https://www.youtube.com/watch?v=E1E08i2UJGI

Sovellukseen on tehty lisäksi Jest -yksikkötestit sekä github actions putki, joka ajaa testit ja buildaa sovelluksen.

## GitHub Actions

Github actions workflowia voidaan kokeilla valmiilla ohjelmalla, jonka tämä repositorio sisältää. 

Tämän demo-ohjelman alkuperäinen repositorio löytyy osoitteesta: https://github.com/Jualhalo/todoLista. 

Kloonaa tämä tehtävä omalle koneellesi haluamaasi hakemistoon. Poista package-lock.json -tiedosto.

## Työjono, Workflow

Projekti sisältää jo valmiin workflow tiedoston, joka löytyy .github/workflows -polun takaa. Workflowssa on työ, joka käynnistyy main haaran push-eventin yhteydessä. Kun pushaat projektin repositorioosi, pitäisi workflowin käynnistyä automaattisesti. Pääset seuraamaan workflowin toimintaa ja tuloksia repositoriostasi Actions-välilehdeltä. Näkymässä on listattu kaikki workflowt. Jos jokin niistä on käynnissä, sen vierellä on keltainen merkki. Klikkaamalla workflow:ta se laajentuu ja pääset näkemään kaikki sen sisältämät työt. Työtä klikattaessa sekin laajentuu ja näet listan kaikista työn askeleista (steps). Tässä näkymässä näet myös kaikki onnistuneet/epäonnistuneet vaiheet, sekä sen vaiheen jossa workflow on kyseisellä hetkellä menossa, edelleen keltaisella merkillä merkattuna.

Mikäli workflow ei suoriutunut onnistuneesti, työnäkymässä on punaisella merkillä merkattuna vaihe jossa workflow epäonnistui. Esimerkiksi jos projektissa olevista yksikkötesteistä yksi tai useampi epäonnistui, se näkyy työnäkymässä kohdassa Run npm test. Epäonnistuneen vaiheen voi laajentaa, jolloin siinä näkyy mitkä testit onnistuivat ja mitkä epäonnistuivat. Jos jokin vaihe epäonnistui, mukana on myös error-viesti, joka viittaa epäonnistumisen syyhyn. Tällöin koodiin tulisi tehdä korjauksia, jotta kaikki testit menevät läpi. Tee tarvittavat korjaukset koodiin ja commitoi.

Testaus ja buildaus -työn yhteydessä on myös huomio noden 12-version deprekoitumisesta. Päivitä YAML-tiedostoa siten, että vaihdat setup-node -actionisin versioon 3 ja noden versioksi 20. Päivitä myös devdependency  testing-library/react" versioon 15.0.6", Commitoi.

## Testit ja koodin debuggaus

Kun olet tehnyt kummatkin muutokset, pushaa ne githubiin. Tällöin workflowin pitäisi jälleen käynnistyä automaattisesti. Mikäli kaikki vaiheet onnistuivat, workflowin viereen tulee vihreä ok-merkki.

Tutki ajettavaa testiä, ja katso virheilmoitusta. **Korjaa** virheilmoituksen mukaisesti virheellinen koodi. Tee uudestaan **git push**





