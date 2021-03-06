# Technikai tudnivalók az Alkalmazások fejlesztése tárgy beadandóiról

## A dokumentáció elhelyezése

### Github

A beadandót egy Github kódtárban (repository) kell tárolni. Ennek lépései:

1. Új kódtár létrehozása
2. Kódtár klónozása
    1. Helyi munka esetén: `git clone https://...`
    2. Cloud9 esetén: új workspace létrehozásakor meg lehet adni a kódtár elérhetőségét
3. Kód írása
4. Változások stage-elése: `git add .`
5. Változások mentése: `git commit`
6. Változások feltöltése: `git push` vagy `git push origin master`

A dokumentációt a Github kódtár `README.md` állományába kell megírni, ez jelenik majd meg a kódtár főoldalán.

### Markdown és GFM

A dokumentációt GFM-ben (Github Flavoured Markdown) formátumban kell megírni. Segítséget ehhez az alábbi linkeken lehet találni:

- [Összefoglaló a markdown formátumról a Github oldalán](https://help.github.com/articles/markdown-basics/)
- [Másik lényegretörő összefoglaló](http://www.web-crunch.com/resources/lowdown-markdown/)
- [Leírás a GFM-ről](https://help.github.com/articles/github-flavored-markdown/)

### Képek elhelyezése

A dokumentációnak képeket is tartalmaznia kell. Ehhez a képeket feltöltjük egy könyvtárba (pl. `docs/images`) és a dokumentációból [relatív útvonalként hivatkozunk rá](https://help.github.com/articles/relative-links-in-readmes/):

```
![Kép felirata](docs/images/database.png)
```

Az előző kódrészlet eredménye:

![Kép felirata](docs/images/database.png)


## A dokumentáció szerkezete

A dokumentáció felépítésével kapcsolatos elvárások alapvetően megfelelnek az előzménytárgyban megfogalmazott elvárásoknak, de ki is egészülnek a tárgy webes jellegének megfelelően. A következő segédanyagok használhatók ehhez:

- [Az előzménytárgy dokumentációval kapcsolatos elvárásai](http://webprogramozas.inf.elte.hu/alkfejl/A_dokumentacio_felepitese.pdf)
- [A gyakorlatokon tervezéssel kapcsolatban elhangzott diák](http://webprogramozas.inf.elte.hu/alkfejl/03.html#/4)
- [Webes alkalmazások tervezése, tervezési eszközök](http://ade.web.elte.hu/wabp/lecke2_lap1.html)
- [További hallgatói jegyzetek a különböző UML diagramokkal kapcsolatban](http://webprogramozas.inf.elte.hu/alkfejl/dok_uml_hallgatoi_anyagok.zip)

A diagramok elkészítéséhez bármilyen eszköz használható. Néhány ajánlat:

- [nomnoml](http://nomnoml.com/): sokféle diagramtípus
- [js-sequence-diagrams](https://bramp.github.io/js-sequence-diagrams/): szekvenciadiagramok
- [Lumzy](http://lumzy.com/app/): webes mockupkészítő eszköz
- [LayoutIt](http://www.layoutit.com/build): designtervekhez
- [Bootswatch](http://bootswatch.com/): designtervekhez

A dokumentáció a következő részeket tartalmazza:

- Követelményanalízis
- Tervezés
- Implementáció
- Tesztelés
- Felhasználói dokumentáció


### Követelményanalízis

A követelmény feltárás során felmérik és összegyűjtik a megrendelt szoftverrel szemben támasztott felhasználói követelményeket, elemzik az alkalmazási szakterületet. Részei:

1. Követelmények összegyűjtése: a nyújtandó szolgáltatások ismertetése rövid, szöveges leírásként, sokszor felsorolásként jelenik meg.
    1. Funkcionális elvárások
    2. Nem funkcionális követelmények
2. Szakterületi fogalomjegyzék: ha vannak speciális fogalmak, akkor ezeket itt lehet összegyűjteni és magyarázni.
3. Használatieset-modell
    1. Szerepkörök: lista rövid leírással
    2. Használati eset diagramok: a szerepkörök és az elérhető funkiók kapcsolatát jelenítik meg, ha kell, akkor esetenként rövid magyarázó szöveggel.
    3. Folyamatok pontos menete: legalább 1 folyamat kifejtése.


### Tervezés

1. Architektúra terv
    1. komponensdiagram (nem kell)
    2. Oldaltérkép
    3. Végpontok
2. Felhasználóifelület-modell
    1. Oldalvázlatok
    2. Designterv (nem kell, elég a végső megvalósítás kinézete)
3. Osztálymodell
    1. Adatmodell
    2. Adatbázisterv
    3. Állapotdiagram
4. Dinamikus működés
    1. Szekvenciadiagram (nem kell)

### Implementáció

1. Fejlesztői környezet bemutatása
2. Könyvtárstruktúrában lévő mappák funkciójának bemutatása

### Tesztelés

Tesztesetek felsorolása: milyen eseteket próbált végig a hallgató. (egyelőre nem kell)

### Felhasználói dokumentáció

1. A futtatáshoz ajánlott hardver-, szoftver konfiguráció
2. Telepítés lépései: hogyan kerül a Githubról a célgépre a program, hogyan kell elindítani
3. A program használata

