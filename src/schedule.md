# Ütemezés

Az órák csütörtökönként a BA.F.07-ben vannak (távoktatásban, MS Teams-en), neptun szerint 08:00-10:35 között előadás és 10:45-11:30 között gyakorlat. (Ezek aránya valamint közte a szünet az aktuális előadásanyag és az igények szerint módosulhat). A „gyakorlat” nem labor, hanem sokkal inkább konzultáció!

|hét |dátum      |előadás                    |gyakorlat                                                               |
|---:|:---------:|:-------------------------:|:----------------------------------------------------------------------:|
|  1.|  09. 08.  | Bevezető, áttekintés      | feladat és a munkafolyamat átfogó ismertetése, avalonia tutorial       |
|  2.|  09. 15.  | Napi munka, verziókezelők | git, GitHub, IDE ismertetés, warmup feladat ismertetése                |
|  3.|  09. 22.  | Software Architecture I.  | csapatsorsolás, Sprint Planning, Task Definition Workshop              |
|  4.|  09. 29.  | Software Architecture II. | konzultáció (design dokumentumok bemutatása)                           |
|  5.|  10. 06.  | Agile, SCRUM, Kanban      | konzultáció                                                            |
|  6.|  10. 13.  | Verification & validation | konzultáció                                                            |
|  7.|  10. 20.  | Continuous Integration    | nálunk hogy működik (handout, AutomatedCar), konzultáció               |
|  8.|**10. 27.**| **1. demo**               | retrospektív, Sprint Planning, Task Definition Workshop                |
|  9.|  11. 03.  | Review culture            | konzultáció                                                            |
| 10.|  11. 10.  | Legacy code               | konzultáció                                                            |
| 11.|  11. 17.  | ASPICE in nutshell        | konzultáció                                                            |
| 13.|  11. 24.  | Guest presentation        | konzultáció                                                            |
| 12.|**12. 01.**| Összefoglalás, **2. demo**| retrospektív, tárgy feedback                                           |
| 14.|**12. 08.**| **Zárthelyi dolgozat**    |                                                                        |


## Házi feladatok

Határidő (hét)| feladat
---|--------
2  | [Avalonia Tutorial teljesítése](https://docs.avaloniaui.net/tutorials/todo-list-app)
3  | Warmup feladat
4  | design dokumentumok bemutatása (statikus és dinamikus)


## Gantt diagram

<div class="mermaid">
    gantt
    dateFormat  YYYY-MM-DD
    axisFormat  %m-%d
    title 2022/23 tanév I.félév
    Bemutatkozás :milestone, 2022-09-08, 1d
    section Avalonia
        Avalonia-tutorial: active, avalonia-tutorial, 2022-09-08, 1w
    section Warm-up
        Warm-up :active, warmup, 2022-09-15, 1w
    Csapat sorsolás :milestone, after warmup, 1d
    section Sprint 1
        Sprint 1 :active, sprint1, after warmup, 5w
    Demo 1 :milestone, after sprint1, 1d
    section Sprint 2
        Sprint 2 :active, sprint2, after sprint1, 5w
    Demo 2 :milestone, after sprint2, 1d
    Zárthelyi :milestone, 2022-12-08, 1d
    click sprint1 href "./sprint_1.html"
    click sprint2 href "./sprint_2.html"
</div>


<!--
# Házi feladat - 1. hét

1. GitHub fiók létrehozása
    * ha még nincs
2. 11 JDK telepítése, mivel a szoftvert Java nyelven kell elkészíteni
    * ha nincs fönt
3. Fejlesztőkörnyezet telepítése és beállítása
    * IntelliJ IDEA az ajánlott és támogatott eszköz
4. Git és GitHub oktatóanyagok elolvasása
    * ha vannak hiányosságok
    * az órán nincs idő szájbarágósan git használatot oktatni, erre vannak interaktív oktatófelületek
    * ez mindenkinek egyéni felelőssége, ám ha konkrét kérdések merülnek fel, akkor ezekre természetesen kitérünk
5. Git repó klónozása
6. Kód futtatása a futtató- és a fejlesztőkörnyezet beállításainak tesztelése céljából
7. A jegyzet és az abban taglalt segédanyagok megismerése
8. Az elkészítendő szoftver átgondolása (lásd readme), statikus és dinamikus modell elkészítése komponens szinten
    * Ennek terjedelme (az órái példa alapján): egy absztrakciós szint a négyfelé bontás (kb. user story szint), és egy az ez alatti egyel, minden komponens még egy kibontása, kb. egyenrangú komponensek létrehozására - osztály szintre nem mennék le, még ha a végén ezekből akár osztály is lesz. Szóval kettő struktúra, kettő dinamikus viselkedést leíró diagram, egy magasabb és egy alacsonyabb absztrakciós szinten. Hogy konkrétan hány building block, azt mindenkinek "érzésre" kell megállapítania, ezért szubjektív az architektúra.
    * Ez egy egyéni feladat, hiszen még nincsenek csapatok. Az elkészítéshez javasolt eszközök: MS Visio, https://www.draw.io/.
    * Az elkészült diagramoknak a következő órán bemutatható állapotban kell lenniük.
-->



# Demók

A félév során a csapatok két alkalommal prezentálják az elvégzett munkát. A „demók” az _elkészült_ szoftver megrendelőnek való bemutatását szimulálják. Nem a kódra vagyunk kíváncsiak, hanem működés közben szeretnénk látni, hogy a szoftver teljesíti feladatban foglalt követelményeket.
A bemutatás során, a `master` branchre befogadott kódot vesszük figyelembe, minden egyéb _„nem készült el határidőre”_, azaz értékelhetetlen.

[Bővebben...](demo.md)


# Zárthelyi

Ismert, Moodle-ös teszt, 50 kérdéssel, erre 70 perc áll majd a rendelkezésre. Minden kérdéshez 4 válaszlehetőség, amelyek közül pontosan egy a helyes. (Vannak „az alábbiak közül melyik NEM helyes” felépítésű kérdések is.) A rendelkezésre álló idő alatt kérdéseket tetszőleges alkalommal felül lehet vizsgálni, módosítani a teszt „lezárása” után azonnal kiértékelésre is kerül.


# Jegy kialakítása

1. gyakorlati jegy (sprintek átlaga) × 0.7 + ZH jegy × 0.3

2. Ha nincs gyakorlati teljesítmény, akkor a félév elégtelen, függetlenül attól, hogy a ZH hogy sikerült.
3. Mivel a sprintekre csapatok kapnak jegyet, mindenki kitölt egy csapattárs értékelő kérdőívet arról, hogy a csapaton belüli munka miképpen oszlott meg.

A ZH százalék jegyre számítását az alábbi intervallumokkal végezzük:

tól | ig | jegy
-- | --- | --
 0 |  49 | 1
50 |  59 | 2
60 |  69 | 3
70 |  79 | 4
80 | 100 | 5
