# Data Structures and Algorithms with JavaScript

## Előszó

### Miért tanulmányozzuk az adatstruktúrákat és az algoritmusokat?

Nicklaus Wirth - Algorithms + Data Structures = Programs (Prentice-Hall)

Minden számítógép programnak szüksége van valamilyen típusú adatstruktúrára, hogy a program kezelje azokat az adatokat, amiket manipulál, egy vagy több algoritmussal, hogy az adatokat átfordítsa a bejövő formátumról, kimenő formátumra.

## Tömb

A leggyakoribb adatstruktúra aszámítógép programozásban.

### JavaScript tömb definiálása

> Tömb: elemek lineáris gyűjteménye, ahol az elemek index-elve vannak.

A JavaScript tömbök gyakorlatilag speciális típusú objektumok, az indexek integer típusú számok. Amikor integer típust használ indexekhez, belűl átkonvertálódnak string típussá. Mivel csak objektumok a JavaScript tömbök, nem annyira hatékonyak más programozási nyelvekhez képest.

### Tömbök használata

A tömbök a JavaScript-ben nagyon rugalmasak.

#### Tömb létrehozása

```JavaScript
const numbers = [] ;
print(numbers.length); // 0

// Más módon
const numbers = [1,2,3,4,5];
print(numbers.length); // 5

// Más módon
const numbers = new Array();
print(numbers.length); // 0

// Más módon
const numbers = new Array(1,2,3,4,5);
print(numbers.length); // 5

//
const numbers = new Array(10);
print(numbers.length); // 10

// Nem kell minden elemének a tömbnek ugyanolyan típusúnak lenni.
const objects = [1, "Joe", true, null];

// A tömb valóban tömb? - isArray()
const number = 3;
const arr = [7,4,1974];

print(Array.isArray(number)); // false
print(Array.isArray(arr)); // true
```

* [JavaScript: The Good Parts by Douglas Crockford](http://shop.oreilly.com/product/9780596517748.do)
* [JavaScript: The Definitive Guide, 6th Edition](http://shop.oreilly.com/product/9780596805531.do)
