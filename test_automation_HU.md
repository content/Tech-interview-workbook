# Tesztautomatizálási kérdések

## Tesztelési alapok (ISTQB-hez kapcsolódó)
<img src="https://www.mindsmapped.com/wp-content/uploads/2016/06/ISTQB.jpg" alt="image" width="300" height="220">

#### ✅ Mi a tesztelés célja? Mi nem az?
A tesztelés célja annak ellenőrzése, hogy a szoftver megfelel-e a meghatározott követelményeknek, és helyesen működik-e. Nem az a célja, hogy javitsa a szoftver minőségét vagy kijavitsa a hibákat.

#### ✅ Mik a tesztelési alapelvek?
1. A hibák korai felfedezése elve
2. Teljes lefedettség elve
3. Prioritás elve
4. Reprodukálhatóság elve
5. Környezetfüggetlenség elve
6. Tesztelési erőforrások optimalizálásának elve
7. Tesztelés dokumentálásának elve

#### ✅ Mi az egységtesztelés (unit testing)? Ki felelős az egységtesztek írásáért?
Az egységtesztelés (unit testing) olyan tesztelési módszer, amelyben az egyes egységeket (általában függvényeket vagy osztályokat) izoláltan teszteljük, hogy meggyőződjünk a helyes működésükről. Az egységteszteket általában a fejlesztők irják, mivel ezek a tesztek a kód minőségének és funkcionalitásának biztositására szolgálnak. A fejlesztők felelősek az egységtesztek irásáért és futtatásáért.

#### ✅ Mik a tesztszintek, és mi a különbség köztük?

##### Tesztszintek:
1. Egységtesztelés (unit testing)
2. Komponenstesztelés (component testing)
3. Integrációs tesztelés (integration testing)
4. Rendszertesztelés (system testing)
5. Elfogadási tesztelés (acceptance testing)

##### Különbségek:
- Az egységtesztelés az egyes egységeket izoláltan teszteli, mig a komponenstesztelés az egységek csoportjait teszteli.
- Az integrációs tesztelés a különböző egységek vagy komponensek együttműködését teszteli.
- A rendszertesztelés teljes rendszert tesztel, mig az elfogadási tesztelés azt ellenőrzi, hogy a rendszer megfelel-e a felhasználói követelményeknek.


#### ✅ Mi a különbség a verifikáció és a validáció között?
Verifikáció a folyamat, amely során ellenőrizzük, hogy a szoftver megfelel-e a specifikációknak és helyesen lett-e implementálva. Validáció viszont azt jelenti, hogy ellenőrizzük, hogy a szoftver valóban azt a funkcionalitást nyújtja, amit a felhasználók elvárnak tőle.

#### ✅ Mik a tesztelési típusok, és mi a különbség köztük?
##### Tesztelési tipusok és különbségeik:

1. Fekete doboz tesztelés:
    - A kód bázist nem ismerjük, csak a bemeneteket és kimeneteket vizsgáljuk.
    
2. Fehér doboz tesztelés:
    - A kód bázist is ismerjük, a kód struktúráját és logikáját is teszteljük.
    
3. Szürke doboz tesztelés:
    - Kombinálja a fekete és fehér doboz tesztelés jellemzőit, részben ismerjük a belső működést.

4. Regressziós tesztelés:
    - A korábban működő funkcionalitásokat teszteljük újra a változások után.

5. Füsttesztelés:
    - Gyors, felületes teszt, amely az alapvető funkcionalitások működését ellenőrzi.

6. Újratesztelés:
    - Korábban hibásnak talált részek újraellenőrzése a javitások után.

#### ✅ Mi a különbség a fehér doboz, szürke doboz és fekete doboz tesztelés között?

##### Fehér doboz tesztelés:
- Ismert a kód bázis, a kód struktúráját és logikáját is teszteljük.

##### Szürke doboz tesztelés:
- Kombinálja a fekete és fehér doboz tesztelés jellemzőit, részben ismerjük a belső működést.

##### Fekete doboz tesztelés:
- Nem ismerjük a kód bázist, csak a bemeneteket és kimeneteket vizsgáljuk.


#### ✅ Mi a különbség a felhasználói elfogadási teszt (UAT) és a rendszerteszt között?
- **Felhasználói elfogadási teszt (UAT):**
  - A felhasználók végzik el, akik a szoftvert valódi környezetben használják.
  - Célja, hogy ellenőrizze, hogy a szoftver megfelel-e a felhasználói igényeknek és elvárásoknak.
  - Általában a fejlesztés végén, a rendszer teljes funkcionalitásának ellenőrzésekor történik.

- **Rendszerteszt:**
  - Tesztelők vagy tesztcsapat végzi.
  - Célja, hogy ellenőrizze a rendszer teljesitményét, megbizhatóságát, skálázhatóságát stb.
  - Általában a fejlesztés közben és a fejlesztés végén is történik, hogy biztositsa a rendszer megfelelő működését.

#### ✅ Sorolj fel különbségeket a regressziós tesztelés, a füsttesztelés és az újratesztelés között!

##### Újratesztelés (Re-testing)
| Jellemző               | Leirás                                            |
| ---------------------- | ------------------------------------------------- |
| **Cél**                | Ellenőrizni, hogy egy adott hibát kijavitottak-e. |
| **Fókusz**             | Egy konkrét hiba vagy hibák újbóli tesztelése.    |
| **Mikor végzik?**      | Miután egy hibát javitottak.                      |
| **Kiterjedtség**       | Csak az érintett funkciókat tesztelik újra.       |
| **Automatizálhatóság** | Gyakran manuálisan végzik.                        |

##### Füsttesztelés (Smoke Testing)
| Jellemző               | Leirás                                            |
| ---------------------- | ------------------------------------------------- |
| **Cél**                | Gyorsan ellenőrizni, hogy az alapfunkciók működnek-e (az alkalmazás „elinditható-e”). |
| **Fókusz**             | Alapvető funkciók (pl. belépés, főoldal betöltése, adatbevitel stb.).                 |
| **Mikor végzik?**      | Minden új build után, mielőtt részletesebb tesztelésre kerül sor.                     |
| **Kiterjedtség**       | Felületes, de széleskörű.                                                             |
| **Automatizálhatóság** | Gyakran automatizált.                                                                 |

#### ✅ Mi a különbség a statikus és dinamikus tesztelés között?

**Statikus tesztelés:**
- A kód vagy dokumentáció vizsgálata történik anélkül, hogy a program futtatásra kerülne.
- Célja a hibák, logikai hibák, stilusproblémák felfedezése.
- Példák: kódolási standardok ellenőrzése, kódolási konvenciók betartása, statikus kódelemző eszközök használata.

**Dinamikus tesztelés:**
- A program futtatása történik különböző bemenetekkel, hogy ellenőrizzük a funkcionalitást és a teljesitményt.
- Célja a szoftver működésének ellenőrzése, hibák felfedezése futás közben.
- Példák: egységtesztelés, integrációs tesztelés, rendszertesztelés.


### ✅ Hasonlítsd össze a V-modellt, a vízesés modellt és az Agile megközelítést a tesztelés szempontjából!

| Jellemzők                | Vizesés modell              | V-modell                            | Agile megközelités                               |
| ------------------------ | --------------------------- | ----------------------------------- | ------------------------------------------------ |
| **Fejlesztési folyamat** | Lineáris, szakaszos         | Szimmetrikus (V alakú), lineáris    | Iterativ és inkrementális                        |
| **Tesztelés kezdete**    | A fejlesztés után           | Párhuzamosan a tervezéssel          | Már a sprint elején elindul                      |
| **Tesztelés tipusa**     | Főként végső (system) teszt | Minden szinthez tartozik teszt      | Folyamatos tesztelés (TDD, automatizált tesztek) |végén	Minden szakaszhoz hozzárendelt	Sprinten belül, azonnal
| **Tesztelés időzitése**  | A fejlesztés végén          | Minden szakaszhoz hozzárendelt      | Sprinten belül, azonnal                          |
| **Tesztelők bevonása**   | Későn (végső fázisban)      | Korábban (már a tervezési fázisban) | Folyamatosan, csapattagként                      |
| **Visszacsatolás**       | Korlátozott, nehézkes       | Korlátozott, de szervezett          | Gyors és rugalmas                                |
| **Hibajavitás kezelése** | Nehézkes, költséges         | Strukturált, de nem gyors           | Gyors, iterativ                                  |
| **Dokumentáció szerepe** | Erősen dokumentált          | Nagyon részletes                    | Csak a szükséges minimum                         |

<img src="https://t4.ftcdn.net/jpg/03/90/15/65/360_F_390156585_8w1lsOyICIAOvDCU8tExXW2QwLCOFwXD.jpg" alt="image" width="550" height="400">


<img src="https://i.imgur.com/S38EBJw.png" alt="image" width="550" height="400">   <img src="https://segedletek.level14.hu/assets/img/modszertan-vizeses.svg" alt="image" width="550" height="400">


<img src="https://promanconsulting.hu/wp-content/uploads/2022/03/agilis-modszertanok-optimized.jpg" width="550" height="400">





## Reporting, Bugs
<img src="https://moolya.com/blog/wp-content/uploads/2023/05/Bug-Report.png" alt="image" width="300" height="220">

#### ✅ Milyen lépéseket követnél egy hiba megtalálásakor?
1. Hiba reprodukálása
2. Hiba dokumentálása
3. Hiba priorizálása és továbbitása
4. Hibajavitás (Fejlesztők által)
5. Újratesztelés
6. Regressziós tesztelés
    - Javitás nem okozott mellékhatásokat más funkciókban
7. Hiba lezárása

#### ✅ Beszélj a gyakori tesztjelentésekről és részleteikről!


#### ✅ Mit tartalmaz egy hibajelentés?
1. Cim, rövid leirás
2. Lépések a hiba reprodukálásához
3. Várt eredmény
4. Valós eredmény
5. Súlyosság, technikai hatás
6. Prioritás
    - Fejlesztési sorrendre utal
    - Pl.: High (azonnali javitás szükséges), Medium, Low
7. Környezeti információk
8. Mellékletek

#### ✅ Hogyan rangsorolnál egy hibát?
Egy hiba rangsorolása során két fő szempontot veszünk figyelembe: súlyosság és prioritás.
- **Súlyosság:** Ez azt mutatja meg, mennyire káros a hiba a rendszer működésére. Ezt általában a tesztelők állapítják meg.

- **Prioritás:** Ez mutatja meg, milyen gyorsan kell javítani a hibát. Ezt gyakran a projektmenedzser vagy a terméktulajdonos állapítja meg.

## Test Automation, Selenium
<img src="https://media.licdn.com/dms/image/C4D12AQE3GOyVsZazOw/article-cover_image-shrink_600_2000/0/1583830696602?e=2147483647&v=beta&t=bYHbKyhMoWsMgtEug6eSf3m0db5ZtGEl437TeS1qkfI" alt="image" width="320" height="220">

#### ✅ Melyik teszteseteket érdemes automatizálni és melyiket nem?
##### Érdemes automatizálni:

##### Nem érdemes automatizálni:
1. Egyszeriek vagy ritkán futnak
    - Pl. egyszeri migrációs ellenőrzés vagy nem kritikus funkciók

2. Gyakran változó UI-t vagy instabil környezetet tesztelnek
    - A változások miatt az automatizált tesztek gyakran „fals hibát” jeleznek

3. Erősen vizuális ellenőrzést igényelnek
    - Példa: reszponzív dizájn, elrendezés, színhelyesség
    - Ezekhez manuális vagy vizuális regresszióteszt való

4. Túl komplex, kreatív vagy intuícióalapú tesztek
    - Pl. UX/ergonómiai értékelés, „érzet” tesztelése

5. Alacsony üzleti értékű vagy gyorsabb manuálisan
    - Egyszerű hibák, beállítások ellenőrzése

#### ✅ Írj le egy jó automatizált tesztet!
Példa egy bejelentkezés rendszer tesztelésére

```py
import unittest
from selenium import webdriver
from selenium.webdriver.common.by import By

class LoginTest(unittest.TestCase):

    def setUp(self):
        self.driver = webdriver.Chrome()  # vagy pl. Firefox
        self.driver.get("https://example-webshop.hu/login")
        self.driver.implicitly_wait(10)

    def test_valid_login(self):
        driver = self.driver
        # Kitöltjük az űrlapot
        driver.find_element(By.ID, "email").send_keys("tesztfelhasznalo@example.com")
        driver.find_element(By.ID, "password").send_keys("HelyesJelszo123")
        driver.find_element(By.ID, "login-button").click()

        # Ellenőrzés: sikeres bejelentkezés után megjelenik a profilnév
        welcome_text = driver.find_element(By.ID, "welcome-message").text
        self.assertIn("Üdv", welcome_text, "A bejelentkezés nem sikerült.")

    def tearDown(self):
        self.driver.quit()

if __name__ == "__main__":
    unittest.main()

```

#### ✅ Mi a Selenium, Selenium IDE és Selenium WebDriver?
- **Selenium:** 
    - A Selenium egy tesztautomatizálási keretrendszer, amely lehetővé teszi, hogy automatizált módon vezéreljünk böngészőket (pl. Chrome, Firefox, Edge) különböző programozási nyelvekből (pl. Java, Python, C#, JavaScript).

- **Selenium IDE:** 
    - Böngészőbővítmény (Chrome és Firefox számára)
    - Kattintásalapú rögzítés: rögzíti a felhasználó tevékenységeit és automatikusan generál egy tesztet
    - Hasznos gyors tesztekhez és prototípushoz
    - Kódolás nélkül is használható
    - Korlátozott testreszabhatóság, nem jó komplex vagy dinamikus tesztekhez

- **Selenium WebDriver:**
    - Ez a Selenium legfontosabb és legtöbbet használt komponense.
    - Fejlett, kód-alapú, valós böngésző-vezérlő API

#### ✅ Hogyan lehet azonosítani a webes elemeket?
1. ID
2. Name
3. Osztály név
4. Elem név
5. Link / Részleges Link szöveg
6. XPath
7. CSS kijelölő

#### ✅ Hogyan lehet várni az elemekre, és mi lehet a probléma? Gyűjtsd össze a lehetséges hibákat és okokat!
A Selenium támogatja a várakozási stratégiákat:

##### Implicit wait (általános várakozás)
```py
    driver.implicitly_wait(10)  # másodpercben
```

##### Explicit wait (csak egy adott feltételre vár)
```py
    from selenium.webdriver.common.by import By
    from selenium.webdriver.support.ui import WebDriverWait
    from selenium.webdriver.support import expected_conditions as EC

    wait = WebDriverWait(driver, 10)
    element = wait.until(EC.visibility_of_element_located((By.ID, "email")))
```

#### Fluent wait (Testre szabható várakozás)
- Meghatározható a lekérdezés gyakorisága, és hogy milyen kivételeket ignoráljon.

#### ✅ Hasonlítsd össze a POM és a Keyword Driven Testing megközelítéseket!
| Tulajdonság               | **POM (Page Object Model)**         | **Keyword Driven Testing (KDT)**          |              |            |
| ------------------------- | ----------------------------------- | ----------------------------------------- | ------------ | ---------- |
| **Célközönség**           | Fejlesztők, teszt automatizálók     | Tesztelők, akár kód nélkül is             |              |            |
| **Tesztleírás módja**     | Kódalapú (pl. Python, Java)         | Kulcsszavak, táblázatok                   |              |            |
| **Karakterisztika**       | Objektum-orientált, strukturált     | Leíró, adatvezérelt                       |              |            |
| **Újrafelhasználhatóság** | Magas (page class-ok)               | Magas (kulcsszavak)                       |              |            |
| **Karbantarthatóság**     | Jó, ha jól strukturált              | Kihívás, ha sok kulcsszó van              |              |            |
| **Használati példa**      | `LoginPage.login_with_valid_user()` | \`OPEN\_BROWSER                           | URL`, `CLICK | loginBtn\` |
| **Bevezetési költség**    | Közepes                             | Magas (framework + kulcsszók fejlesztése) |              |            |
| **Tanulási görbe**        | Fejlesztőknek egyszerű              | Tesztelőknek is barátságos                |              |            |


#### ✅ Mi a különbség a TDD és BDD között?
| Tulajdonság    | TDD (Test-Driven Development) | BDD (Behavior-Driven Development) |
| -------------- | ----------------------------- | --------------------------------- |
| Teszt típusa   | Egységteszt                   | Funkcionális viselkedésteszt      |
| Tesztek nyelve | Kód (pl. Python, Java)        | Természetes nyelv (Gherkin)       |
| Fókusz         | Kód működése                  | Felhasználói viselkedés           |
| Résztvevők     | Fejlesztők                    | Fejlesztők, tesztelők, üzlet      |
| Teszt eszközök | pl. JUnit, NUnit, Pytest      | pl. Cucumber, SpecFlow, Behave    |
| Kommunikáció   | Technikai                     | Üzleti és technikai is értik      |
| Dokumentáció   | Kód szintű                    | Élő specifikáció                  |


#### ✅ Mi az API tesztelés és miért hasznos?
Az API tesztelés (Application Programming Interface testing) a szoftvertesztelés egyik típusa, amely során az alkalmazás háttérrétegét (API-kat) teszteljük — a felhasználói felület kihagyásával. Ez lehetővé teszi, hogy a rendszer működését korán, gyorsan és pontosan ellenőrizzük.

#### ✅ Mi az adatvezérelt tesztelés és miért hasznos?
Az adatvezérelt tesztelés (Data-Driven Testing, DDT) egy olyan tesztelési módszer, amelyben ugyanazt a tesztszkriptet futtatjuk különböző bemeneti adatokkal. A tesztadatokat általában külső forrásból (pl. Excel, CSV, adatbázis, JSON, XML) olvassuk be, és a teszt ezek alapján ismétlődik meg.

#### ✅ Mik a kihívások és ajánlott eljárások a dinamikusan betöltött webes elemekkel?
A dinamikusan betöltött webes elemek, késleltetve megjelenő gombok, listák, értesítések komoly kihívást jelentenek az automatizált tesztelésben (pl. Selenium). Ezek az elemek nem mindig elérhetők azonnal, így a szkriptek időzítési hibákat (pl. ElementNotFoundException) okozhatnak.

#### ✅ Mik a mobil tesztautomatizálás kihívásai?
A mobil tesztautomatizálás számos előnyt kínál (gyorsabb tesztelés, CI/CD támogatás), de sokkal komplexebb, mint a webes automatizálás. Ennek oka a platformfüggőség, a hardverváltozatosság, és az UI-k dinamikus viselkedése.

## Haladó témák
<img src="https://www.softwaretestinghelp.com/wp-content/qa/uploads/2020/05/DevOps-in-a-Selenium-Testing.png" alt="image" width="320" height="220">

#### ✅ Mi a különbség a CI és CD között?
A CI és CD a szoftverfejlesztésben használt automatizálási gyakorlatok, amelyek célja a gyors, megbízható és gyakori szoftverkiadás. Bár gyakran együtt említik őket, más célt szolgálnak:

| CD típus                  |   Jelentés                                                                                                |
| ------------------------- | ------------------------------------------------------------------------------------------------------- |
| **Continuous Delivery**   | A kód automatikusan eljut **tesztelt, kiadásra kész** állapotba (manuális jóváhagyás után lehet kiadni) |
| **Continuous Deployment** | A kód **teljesen automatikusan** települ a produkciós környezetbe                                       |


#### ✅ Írj le egy Continuous Delivery folyamatot!
1. Kód commit & push
2. Build
3. Automatizált tesztek futtatása
4. Build artifact mentése
5. Staging környezetbe telepítés
6. Manuális jóváhagyás (opcionális)
7. Production release (manuális lépés)


#### ✅ Hasonlítsd össze két népszerű CI rendszert, ezek közül az egyik legyen a Jenkins!
| Tulajdonság               | Jenkins                                          | GitHub Actions                                         |
| ------------------------- | ------------------------------------------------ | ------------------------------------------------------ |
| **Telepítés**             | Saját szerverre kell telepíteni, teljes kontroll | Felhőalapú, GitHub-ba integrált, nincs külön telepítés |
| **Nyílt forráskód**       | Igen, teljesen nyílt forráskódú                  | Igen, de GitHub platform részeként                     |
| **Könnyű használat**      | Kezdőknek bonyolultabb, sok konfiguráció         | Felhasználóbarát, YAML alapú workflow-k                |
| **Integráció**            | Nagy plugin-ökoszisztéma (\~1500 plugin)         | Erős GitHub és GitHub Marketplace integráció           |
| **Konfiguráció**          | Webes UI vagy Jenkinsfile (Pipeline-as-Code)     | YAML fájlok a repository-ban                           |
| **Skálázhatóság**         | Lokális vagy cloud agentekkel skálázható         | Felhő által kezelt, automatikus skálázódás             |
| **Költség**               | Ingyenes, de saját infrastruktúrát igényel       | Ingyenes nyilvános repo-hoz, privátnál fizetős         |
| **CI/CD támogatás**       | Teljeskörű, bármilyen projektben használható     | Erős GitHub-centrikus CI/CD                            |
| **Támogatott nyelvek**    | Minden nyelv, bármilyen build rendszer           | Minden nyelv, különböző runner-ekkel                   |
| **Felhasználói közösség** | Nagy, régóta működő, sok tutorial                | Gyorsan növekvő, GitHub közösségen belül               |
| **Biztonság**             | Saját felelősség a biztonság és frissítések      | GitHub kezeli, automatikus frissítések                 |
| **Fejlesztési sebesség**  | Függ a konfigurációtól és infrastruktúrától      | Gyorsan indul és fut, nincs infra karbantartás         |


#### ✅ Mi a Docker és miért hasznos?
A Docker egy nyílt forráskódú platform, amely lehetővé teszi alkalmazások konténerekbe csomagolását, szállítását és futtatását. A konténerek olyan könnyű, izolált környezetek, amelyekben az alkalmazás és annak függőségei együtt futnak, függetlenül a futtató rendszer környezetétől.