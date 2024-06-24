# Adatkezelési tájékoztató

!> A jelenlegi verzió nem gyűjt adatokat.

Ez az adatkezelési tájékoztató magyarázza, hogy az alkalmazás milyen adatokat gyűjt, és hogyan dolgozza fel és védi ezeket az adatokat az alkalmazással kapcsolatos szolgáltatás nyújtása során.

Az összegyűjtött információk szükségesek a szolgáltatás minőségének fenntartásához és folyamatos fejlesztéséhez.

## Információgyűjtés és felhasználás

Az alkalmazás által rögzített információk 3 kategóriába sorolhatók.

### Hibanaplók

!> Az alábbi funkciók tervezettek, de még nincsenek implementálva. Jelenleg az alkalmazás nem gyűjt felhasználói adatokat.

Ezek anonimizált adatok az alkalmazásban bekövetkező elszállásokról, hibákról. Ezeket a naplókat a hibák azonosítására és javítására használjuk.

Nem tartalmaznak személyes információt.

### Követési adatok

!> Az alábbi funkciók tervezettek, de még nincsenek implementálva. Jelenleg az alkalmazás nem gyűjt felhasználói adatokat.

Az alkalmazás anonimizált felhasználási adatokat gyűjt, ebből, a felhasználói szokásokat megismeve tudjuk javítani a felhasználói élményt (UX).

Ezek az adatok a következőket tartalmazhatják:

- Látogatott képernyők, azokon végzett műveletek
- Az egyes képernyőkön eltöltött idő
- Képernyőméret, orientáció és felbontás
- Operációs rendszer és annak verziója

Az adatokat gyűjtése nem állandóan, hanem kampányszerűen történik.

Az összegyűjtött adatok nem tartalmaznak személyazonosításra alkalmas elemeket (PII), és nem kerülnek megosztásra harmadik féllel a technológiai szolgáltatókon kívül.

Egyedi azonosítót generálunk minden felhasználó számára. Ezt az azonosítót a felhasználó interakciójának követésére használjuk, mint egy munkamenet. Az azonosítót nem osztjuk meg harmadik féllel. Az azonosító nem kapcsolódik semmilyen PII-hoz. Az azonosítót nem használjuk a felhasználó követésére különböző alkalmazások vagy szolgáltatások között. Ez az azonosító minden 30 nap után megsemmisül, így az összegyűjtött adatok névtelenek maradnak. Ezután egy új véletlenszerű azonosítót generálunk.

### Felhasználói adatok

!> Az alábbi funkciók tervezettek, de még nincsenek implementálva. Jelenleg az alkalmazás nem gyűjt felhasználói adatokat.

A felhasználónak lehetősége van többek között az alábbi műveleteket végezni:
- hibás információ bejelentése
- új információk beküldése (pl. új koncertek)
- fejlesztések/új funkciók kérése
- visszajelzés küldése

Amikor ezek az információk beküldésre kerülnek, a felhasználó választhat, hogy megadja az azonosságát (OAuth/közösségi média alapú azonosítás pl.: facebook, google, stb.) vagy névtelen marad. Az azonosság megadása opcionális. Az alábbi előnyökkel jár:

- az alkalmazás értesítheti őket a kérelmükkel kapcsolatos frissítésekről
- nagyobb valószínűséggel foglalkozunk a kérelmükkel (kevésbé valószínű, hogy fennakad a spamszűrőn)
- hamarabb foglalkozunk a kérelmükkel

## Adatok megosztása harmadik féllel

A felhasználói adatokat csak a technológiai szolgáltatóinkkal (AWS, Sentry) osztjuk meg, és kizárólag működési okokból.

Az alkalmazás háttérrendszere [AWS](http://aws.amazon.com/console/). A felhasználói adatokat nem tároljuk az AWS felhőn kívül.

Hibakeresés céljából a hibák a [Sentry](https://sentry.io/) rendszerével vannak megosztva ([Adatvédelmi nyilatkozat](https://sentry.io/privacy/)).

## Biztonság

Az adatok a böngésző-kiegészítő és a háttérrendszer között HTTPS-en keresztül kerülnek elküldésre.

Az összes adat, mind tárolás, mind átvitel közben titkosítva van.

Az AWS infrastruktúráját használjuk a háttérrendszer (backend) védelmére.

## Hozzájárulás

Az alkalmazás használatával hozzájárulsz a jelen Adatvédelmi irányelvhez, és elfogadod az Általános Szerződési Feltételeit.

## Változtatások ezen az adatvédelmi irányelven

Amennyiben frissítésre kerülne az Adatvédelmi irányelv, úgy az új verzió életbelépés előtt 14 napig megtekinthető
[ezen](https://github.com/vhermecz/festime/pulls) a címen.

!> Tervbenv van, hogy a felhasználót az alkalmazáson belül is értesítsük az adatvédelmi irányelv változásairól.

# Kapcsolat

Amennyiben kérdésed vagy javaslatod lenne az adatvédelmi irányelvvel kapcsolatban, ne habozz [kapcsolatba lépni velem](https://github.com/vhermecz/festime).
