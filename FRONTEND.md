# Javascript tematika

## 1. JavaScript `(ECMAScript, ES6)` alapok
> [!NOTE]
> Az `ES6` után több új szabvány is megkjelent, mégis, azért emeljük ki pont ezt a verziót, és nem valamelyik későbbit, mert ez volt a "nagy" vízválasztó, melyben nem csupán náhány függvénnyel, vagy osztályal bővült a Javascript, hanem olyan radikális változásokat hozott, mint a változók hatáskörének kibővítése vagy az OOP nagy átalakulása.

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
>Ebben a részben elsajáítjuk a programozás alapjait. Ha ezt megérted, akkor a többi programnyelvvel is boldogulni fogsz, hiszen a logikája minden programozási nyelvnek hasonló. Természetesen ezeken az órákon bemutatjuk a JavaScript programozás sajátosságait is.

- Típusok, változó, állandok
    - #### Típusok csoportosítása:
        - Primitívek - (egyszerű típusok) melyek egyszerre csak egy adat tárolására alkalmasak
            - Szám - `Number`
                - Ide tartozik a `NaN` érték is, ami a Not a Number rövidítése. Tehát ez nem egy típus, hanem, egy érték.
            - Szöveg - `String`
            - Logikai - `Boolean`
                - lehetséges értékei, a `true` és a `false`
            - undefined - `undefined`
                - Egyetlen értéket vehet fel, és ez az `undefined`
        - Összetett Adattípusok, melyek egyszerre több adat tárolására alaklmasak
            - Az Object, mint adattípus
               - Array azaz Tömb: Fontos mehjegyezni, hogy Javascriptben, a tömb számára nincs külön adattípus. Az az Object-ből van származtatva, ám a gyakorlatban, úgy használjuk, mintha külön típus lenne.

- Operátorok - Melyek műveleteket hajtanak végre, az operandusaik közt, és visszatérnek a művelet eredményével.

    - Az Operátorokat csoportosíthatjuk operandusaik száma szerint:
        - Egy operandusú `unary` 
        - Két operandusú `binary`
        - Három operandusú `thernary`
Vagy 

    - Az általa elvégzett művelet típusa szerint:
        - Aritmetikai műveletek végző operátorok
        - Hozzárendelő vagy értékadó operátorok
        - Összehasonlító operátorok
        - Logikai operátorok
        - Léptető operátorok

- Típuskonverzió - Gyakran van szükség arra, hogy egy változó értékét valami más típusú értékké alakítsuk át. Páldául, amikor egy szám szövegként van definiálva, ekkor ezt a szöveget, ami számot tartalmaz, át kell alakítani, számmá. Ez az átalakítás a típuskonverzió.
- A `Math` object - A Math tartalmazza, a komplekszebb matematikai műveletek elvégzéséhez szükséges függvényeket, mint például a trigonometriai függvényeket, krekítéseket, vagy a gyökvonást és a konstans matematikai értékek is itt vannak tárolva, mint a PI érték. (Amolyan tudományos számológépként lehet használni)

* ####  Vezérlési szerkezetek
    * `function` - Függvények - Amelyek nem mások, mint programba írt programok, melyeket akárhányszor fel tudunk használni (futtatni) a programunkon belül. 
       * `arrow function` - nyílfüggvény, rövidített függvény. `ES6 szintaxis`
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
    
* #### Változók hatásköre
- Sztringműveletek
    - Stringkezelő függvények
- Reguláris kifejezések

- Tömbműveletek:
    - Tömbkezelő függvények
    - A tömbök magasabb rendű függvényei
- #### A Spread syntax, avagy a `...` (másoló) operátor:
    - mely segítségével tömböket és objectecet tudunk ki és be csomagolni. Többek közt, lehetővé teszi két változó, harmadik változó ígénybevétele nélküli felcserélését.
- Halmaz műveletek:
    - A Set Object
- Műveletek Object adattípussal
- #### Referencia típusok:
    - Ebben a fejezetben újra csoportosítjuk az adattípusokat. Hiszen nem csak értékük alapján lehet őket csoportosítani, hanem egy adott típus, hozzárendelésben való működése alapján is. 
- A `Date` object, avagy dátumok a Javascriptben
- Az `Intl` - Internationalization API: A Javascript multikultija :) Amely lehetővé teszi a számok, dátumok és szövegek formázását, a világ különböző nyelvi és kulturális szabályai (úgynevezett locales) szerint. Ahelyett, hogy külső könyvtárakat (például a régi Moment.js-t) használnál, az Intl segítségével natívan, gyorsan és memória-hatékonyan kezelheted a honosítást.

## 3. `DOM` (Document Object Modell) 
#### Javascript alkalmazása front-enden

> Ebben a részben gyakorlatban alkalmazzuk azt, amit elméletben már megalapoztunk Hasznos, vagy szórakoztató mini-alkalmazásokat készítünk a weboldalunkra.

> [!WARNING]
> Ebben a fejezetben, már szükség lesz az eddigi ismereteinkre.

- `DOM` (Document Object Model)
    - DOM szerkezet
    - Csomópontok (Node)
        - Text
        - HtmlElement
    - a `document` object
    - DOM műveletek - HTML elemek manipulálása, Javascript segítségével
        - a children és a childnode
            - köztük levő különbség
        - DOM kezelő függvények
            - egy HTML elem elérése
                - Hagyományos módszerrel, mint pl a `.getElementById`
                - Modern módszer, avagy a `.querySelector` és a `.querySelectorAll`, melyek segítségével egy CSS selector alapján tudunk eg vagy akár több elemt kiválasztani.
                  >[!NOTE] Többek közt ez az `ES6` újítás ásta alá a `jQuery` létjogosultságát, mert most már nem szükséges a jQuery használata a CSS selectorok alapján történő HTML elemek kiválasztásához.
            - a `document` object-en keresztül elérhető függvények
            - Egy Text, vagy HTMLElement csomóponton keresztül elérhető függvények
        - A DOM, egy HTML elemre vonatkozó fontosabb attribútumai
            - Ahol külömbséget teszünk a pusztán csomópont, és HTML csomópont viszonyítási pontok közt
            - Stíluslap (style) kezelése
        - Attribútumok kezelése
        - Saját attríbútumok kezelése:
            - A `dataset` 
    - Eseménykezelés - mely keretén belül lehetőségünk van lekezelni, a HTML oldalon végbeneő eseményeket, mint az oldalbetöltés, egy billentyű lenyomása, vagy az egérkattintás.
        - Két fajta eseménykezelés létezik:
            - Attribútum típusú eseménykezelés
            - EventTarget-en keresztül való eseménykezelés
    - A `Document fragment` - A fragmentekkel lehetőség nyílik, a memóriába dinamukusan, önálló struktúrák létrehozására, melyek roppant hatékonnyá, és gyorsá teszik a DOM manipulációt, hiszen, amíg a fragment-ben dolgozunk, a böngésző nem számolja/nem rajzolja újra a teljes HTML dokumentumunk tartalmát, minden kis apró változtatásra, ami plusz erőforrást emészt fel. És ha már kész a struktúra a megjelenítésre, csak akkor adjuk hozzá a fragmentet a dokumentumhoz.
        - gyakorlati megvalósítás `template` element-en keresztül: például amikor egy webshop termékkártyáját hozzuk létre. A memóriába rakjuk össze, és, amikor teljesen kész van, hozzáaadjuk a dokumentumunkhoz.

## 4. Struktúrális programozás
### Tervezési minták
> Ahhoz, hogy a `3.` fejezetben elkezdett projekteket tovább tudjuk fejleszteni, szükségünk van arra a tudásra, melynek segítségével a kódjainkat, bizonyos modellek alapján rendszerezni, `strukturálni` tudjuk.

- Függvénytárak
    - Vezérlők készítése
- `Closure` - Zárványok, Függvénygyárak: Olyan függvények, melyek "emlékeznek" környezetükre, A zárványon (ami szintén függvény) belül létrehozott változókra, ami kiemelten nagy adatbiztonságot jelent. A zárvány praméterihez, és a zárványon belül létrehozott változókhoz, csak a "Closure" által publikált függvényeken keresztül férhetünk hozzá.
- `Module Pattern` - A moduláris programozás - mely segítségével lehetőségünk nyílik, a kódunk egyes részeit a többitől elkülöníteni, és függetleníteni. Ezzel lehetőségünk nyílik az egyes mechanizmusok szétválasztására, ami a kód átláthatóságát, karbantarthatóságát, és továbbfejleszthetőségét segíti elő. Nem utolsó sorban, egy modul nemcsak átláthatóságot, továbbfejleszthetőséget, és karbantarthatóságot biztosít, hanem mobilitást is, hiszen a modulok, projktről, projekre hordozhatóak, ami egy újabb fejlesztés produktivitását biztosítja.

    Itt beszélni fogunk:
    - Hagyomásnyos függvény alapu modulokról
        - A felefedő modul modell
    - `ES6 modules` - A `module` mód - Aminek segítségével, Javascript állományok publikus interfészeit tudjuk egymásba ágyazni.
        - `export`
        - `import`
    > Érdekesség: Voltaképpen minden modul egy `Closure` :) Csak egy kicsit más megközelítésben. 

## 5. A `document.cookie` - Sütik kezelése
- Mik azok a sütik?
- Mire használhatjuk a sütiket? (Mire valóak egyáltalán)
#### Egy komplett `cookie` modul építése
> A `cookie` modul építése közben, átismételjük, és gyakoroljuk a modulos programozást, miközben megtapasztaljuk azok előnyeit, és nagyszerűségét, egy hasznos gyakoralti példa keretén belül.
#### A `localStorage`
- külömbségek, a `document.cookie`-val szemben

## 6. `Form Validation` - Űrlapok ellenőrzése
>[!NOTE]
> Ebben a fejezetben, Egy összetett, gyakorlati, és a mindennapi programozásban, igen hasznos példán keresztül nézzük meg, mindazt, amit eddig tanultuk.

> Az eddigiekben Javascript nélkül elküldtük a kitöltött űrlapot vagy kérdőívet, és majd kiderült, hogy az jó, vagy hiba van benne. Viszont a böngészőben futó Javascript segítségével, szabályokat határozhatunk meg a felhasználó számára, és csak ezen szabályok mentén tesszük számára lehetővé az űrlap elküldését.
> Ilyen szabályok például: helyes email formátum, karakterszámra vonatkozó megkötések, bizonyos mezők kötelező kitöltése, stb.

## 7. Programozási Paradigmák
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

## 8. `AJAX` - Asynchron Javascript And XML
### Adatok lekérése más szerveren lévő adatbázisból.

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
    - A `JSON` függvényei:
        - `parse` - mely segítségével a szövegként érkezett JSON adatstruktúrát használható formára hozzuk.
        - `stringify` - mely segítségével szöveggé alakítjuk a JSON-t. Ebben a formában tudjuk tartósan tárolni, vagy akár egy kérésben a szerver felé továbbítani.
- a `Promise` - Mint igéret, melyet 2 forgatókönyv jellemez.
    - Mi történjen akkor, ha az ígéretet sikerült teljesíteni
    - Mi történjen akkor, ha az ígéret nem teljesült.
- A `Fetch` API - Ami egy `Promise` alapú kérés kezdeményezését teszi lehetővé.

# 9. `Optimalizálás`
Ebben a fejezetben bepillantunk a javascript futtató környezetébe, abba a mechanizmusban, ahogy a Javascript sorba állítja az épp futásra váró proceszeket. Mivel a Javascript egy szálon fut, előfordulhat, hogy beragad egy-egy hoszabban tartó függvény, vagy ciklus, amit egy helyes optimalizálással, ki tudunk küszöbölni.

- `EventLoop` - ez a mechanizmus felel, azért, hogy a futásra várakozó proceszek, sorban le is fussanak.
- Optimalizálás `EventLoop` segítségével

# 10. `PWA - Progressive Web Application`
* A `PWA` nem más, mint olyan böbgészőben futtatható `HTML+CSS+Javascript` alkalmazások, melyeket eszközünkre (PC, Laptop, Tablet, Telefon,...) telepíthetünk. Az így telepített alkalmazások offline is elérhetőek lesznek, mint bármilyen más telepített alkalmazás az eszközünkön.

***
* Rekurzív függvények

***
# 11. `Frontend Vizsga`

>[!NOTE]    
> * Vizsga: 2,5 órás gyakorlati vizsga a végén
>
> * Beadandó: időpontfoglaló rendszer
>   - pontos leírást a kurzus végén ad az oktató
>   - elkészítésére általában 3 hét áll rendelkezésre
>   - választható nyelv: JavaScript vagy TypeScript
>
> * Tanfolyam közben: órai tesztek
>
> * Folytatás: a 14. hét után TypeScript modul, melynek végén külön vizsga van
