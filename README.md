# JsTematika

## 1. JavaScript `(ECMAScript, ES6)` alapok

- Mi is az a JavaScript?
- A JavaScript eredete és felhasználási lehetőségei
- JavaScript elhelyezése, importálása, betöltése egy HTML dokumentumban
### Egy kis ízelitő
- A programozás alapvető koncepciói
- A JavaScript programozás alapjai
- DOM Manipuláció
- Gyakorlás: Tartalom megjelenítése HTML oldalon JavaScript segítségével

## 2. A programozás alapjai `Javascript` nyelven
> [!NOTE]
>Ebben a részben elsajáítjuk a programozás alapjait. Ha ezt megérted, akkor a többi programnyelvvel is boldogulni fogsz, hiszen a logikája minden programnyelvek hasonló. Természetesen ezeken az órákon bemutatjuk a JavaScript programozás sajátosságait is.

- Típusok, változó, állandok
    - Primitívek - (egyszerű típusok)
        - Szám - `Number`
        - Szöveg - `String`
        - Logikai - `Boolean`
        - undefined - `undefined`
    - Összetett Adattípusok
        - Tömbök
        - Object, mint adattípus
- Operátorok
- Aritmetikai műveletek
- A `Math` object
* #### Változók hatásköre
* ####  Vezérlési szerkezetek
    * `function` - Függvények
    * `if-else` - feltételes mód
    * `switch-case` - szelekciós vezérlési szerkezet
    * #### Ciklusok - Iterációk
        - `for` - léptető ciklus
            - `for in`
            - `for of`
        - `while` - feltételes ciklus
            - `while` - elől tesztelő ciklus
            - `do while` - hátúl tesztelő ciklus
    * `try-catch-finaly` - hibakezelés, kivételkezelés
    * `arrow function` - nyílfüggvény, rövidített függvény. `ES6 szintaxis`
- Tömbműveletek
- Sztringműveletek
- Reguláris kifejezések
- A `Date` object, avagy dátumok a Javascriptben

* Rekurzív függvények

## 3. `DOM` (Document Object Modell) 
#### Javascript alkalmazása front-enden

> Ebben a részben gyakorlatban alkalmazzuk azt, amit elméletben már megalapoztunk Hasznos, vagy szórakoztató mini-alkalmazásokat készítünk a weboldalunkra, például: időpont foglalás, ár kalkulátor, sorba rendezés játék, reakció tesztelő játék, quiz játék, vagy lottó-sorsolás szimulátor.

> [!WARNING]
> Ebben a fejezetben, már szükség lesz az eddigi ismereteinkre.

- `DOM` (Document Object Model) 
    - DOM műveletek - HTML elemek manipulálása, Javascript segítségével
    - Eseménykezelés

## 4. Struktúrális programozás
> Ahhoz, hogy a `3.` fejezetben elkezdett projekteket tovább tudjuk fejleszteni, szükségünk van arra a tudásra, melynek segítségével a kódjainkat, bizonyos modellek alapján rendszerezni, `strukturálni` tudjuk.

- Függvénytárak
    - Vezérlők készítése
- `Module Pattern` - A moduláris programozás
- `ES6 modules` - A `module` mód
    - `export`
    - `import`

## 5. `Form Validation` - Űrlapok ellenőrzése
>[!NOTE]
> Ebben a fejezetben, Egy összetett, gyakorlati, és a mindennapi programozásban, igen hasznos példán keresztül nézzük meg, mindazt, amit eddig tanultuk.

> Az eddigiekben Javascript nélkül elküldtük a kitöltött űrlapot vagy kérdőívet, és majd kiderült, hogy az jó, vagy hiba van benne. Viszont a böngészőben futó Javascript segítségével, szabályokat határozhatunk meg a felhasználó számára, és csak ezen szabályok mentén tesszük számára lehetővé az űrlap elküldését.
> Ilyen szabályok például: helyes email formátum, karakterszámra vonatkozó megkötések, bizonyos mezők kötelező kitöltése, stb.

## 6. Programozási Paradigmák
### `OOP` - Objektum Orientált Programozás

> Egy olyan programozási paradigma, mely az életből vett mintákra alapszik, és ahol egy objektumnak, egyaránt vannak tulajdonságai, és funkcionalitásai is. Segítségével, egész, működési mechanizmusokat hozhatunk létre, melyeket ezután példányosíthatunk.

- Osztály szerkezete
    - Osztályok tulajdonságai és metódusai
- `function` - prototype alapú osztálydefiníció
- `class` alapú osztálydefiníció 
    - Setter és Getter függvények
    - `private` változók és függvények
    - `statikus` változók és függvények
- Osztályok származtatása - öröklődés
- Nyílfüggvények objektumokban való viselkedése, függvények objektumokhoz való tapadásának szabályai
- A `OOP` és a `DOM`
- ##### Gyakorlati példák, feladatok megvalósítása OOP-vel

## 7. `AJAX` - Asynchron Javascript And XML
### Adatok lekérése más szerveren lévő adatbázisból.

> Itt egy gyakorlati példa erejéig egy nagyobb hangszer adatbázisból kérünk le hangszer adatokat. A böngészőből kéréseket küldünk a szerver felé, amelynek válaszát utána feldolgozzuk és megjelenítjük a felhasználónak. Ez újabb oldalletöltés nélkül megy végbe, `AJAX` felhasználásával.

>[!NOTE]
> Ebben a fejezetben nemcsak a programozásban való megvalósításáról lesz szó, hanem szó esik többek közt:
> - Az URL szerkezetéről
> - A kérés szerkezetéről, mely a kérésben küldött adatok mellett, sok fejléc adat is utazik.
> - stb. ...

- Időzített scriptek - a javascript több szálon való kezelése - belépés az `AJAX` világába.
    - `setTimeout`
    - `setInterval`
- Az `XMLHttpRequest`
    - Kérések küldése távoli erőforrásra
    - Válasz fogadása és feldolgozása és megjelenítése
- `JSON` - (JavaScript Object Notation, JavaScript objektumjelölés)
    - Javascript nyelven alapuló, olvasható adastruktúra, melyet többek közt, kliens-szerver közti adatcsere megvalósítására használunk.
- a `Promise` - Mint igéret, melyet 2 forgatókönyv jellemez.
    - Mi történjen akkor, ha az ígéretet sikerült teljesíteni
    - Mi történjen akkor, ha az ígéret nem teljesült.
- A `Fetch` API - Ami egy `Promise` alapú kérés kezdeményezését teszi lehetővé.

## 8. A `document.cookie` - Sütik kezelése
- Mik azok a sütik?
- Mire használhatjuk a sütiket? (Mire valóak egyáltalán)
#### Egy komplett `cookie` modul építése
> A `cookie` modul építése közben, átismételjük, és gyakoroljuk a modulos programozást, miközben megtapasztaljuk azok előnyeit, és nagyszerűségét, egy hasznos gyakoralti példa keretén belül.
#### A `localStorage`
- külömbségek, a `document.cookie`-val szemben

***
# 9. `Frontend Vizsga`
***
# 10. `Backend`
- Javascript a `backend` szemszögéből
- `nodejs` környezet telepítése
- `Javascript` futtatása `nodejs` környezetben

### Az `npm` - Node Package Manager
- A node csomagokról úgy általában
    - `npm init` - új `node` projekt létrehozása, és inicializálása
    - `npm install` - csomagok telepítése

### A `http` package
- A `createServer` - Szerver létrehozása
- Kérések kezelés - `request`
    - a `method` attríbutum - Típusai, melyiket mikor használjuk
- Válasz küldése - `response`
#### Az `fs` (file system) package
- `.readFile` Állományok beolvasása, és tartalmuk válaszként való küldése
- `.writeFile` Állományok írása
#### Egy komplett weboldal betöltése `http` package segítségével
- válaszfejlécek létrehozása
- megfelelő `Content-Type` létrehozása, a betöltendő adat/fájl `MIME` típusának megfelelően, a válasz megfeleő kezelésének érdekében.

### az `express` package
 - `middleware` - köztes program
    - Mik azok a köztes programok
    - Köztes programopk használata, express-ben
    - Saját `middleware` definiálása és hasnzálata
- Az `express` beépített köztes programjai

- Weboldal építése `express` segítségével
- metódusfüggvények
    - kérések és válaszok kezelése metódusfüggvényekkel
    - metódusfüggvények, és a `middleware`
- Statikus weboldal betöltése `express` segítségével
    - `express.static(path) - middleware` használatával, egy statikus könyvtár kiszolgálása

## A `CRUD` API megvalósítása
> [!NOTE]
> A `CRUD` api rövidítés, a
> - `C`reate
> - `R`ead
> - `U`pdate
> - `D`elete
>
> Szavak kezdőbetűjéből tevődik össze. 

Ebben a fejezetben, ezen funkcionalitások, gyakorlati megvalósításával fogunk foglalkozni, melyekkel a kis Hangszerárúházunkat fogjuk kibővíteni.

Itt lehetőségünk nyílik:
- új hangszerek bevitelére 
- szerkesztésére, 
- és törlésére is.

## `Login` felület építése
>[!NOTE]
> A felület építése közben, az alábbi csomagokkal ismerkedhetünk meg:
> - `dotenv` - a `.env` konfigurációs fájl használatára
> - `bcrypt` - a `hash` kódok elkészítésére
> - `jsonwetoken` - a `token` alapú aláírás elkészítésére, és hitelesítésére
> - `cookie-parser` - a sütik gyors kezelésére
>

A felület rendelkezni fog egy védett oldalla, melyet csak abból a böngészőből lehet majd elérni, ahonnan bejelentkeztek, és akkor ha a böngészőben még nem járt le a `token` "szavatossága"

***
# 11. `Backend vizsga`
