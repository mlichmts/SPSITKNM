# Systémová analýza projektu

## Názov projektu (+ meno riešiteľa)
- **Názov projektu**: MotoTrack Slovakia – databáza motokrosových a enduro tratí
- **Meno riešiteľa**: [Meno študenta]
- **Login**: [Login]

---

## Seznam kapitol - částí projektu
1. Úvod
2. Dôvod a okolnosti zavedenia riešenia
3. Popis projektu (slovné zadanie, popis od zákazníka)
4. Analýza požiadaviek
5. Systémové požiadavky (FURPS)
6. Kritické situácie
7. Hranice systému
8. Kontext prostredia
9. Charakteristika aktérov
10. Use Case diagram
11. Scenáre (Implementácia Use Case)
12. Sekvenčný diagram
13. Triedny diagram
14. Záver

---

## 1. Úvod

Projekt je zameraný na vytvorenie webovej aplikácie pre motokrosových, enduro a countrycross jazdcov na Slovensku. Aplikácia bude slúžiť ako prehľadné miesto, kde používateľ nájde informácie o tratiach, ich lokalite a obtiažnosti, a zároveň aktuálne oznámenia o pripravovaných pretekoch.

Hlavnou myšlienkou projektu je spojiť informácie o rôznych typoch motocyklových tratí do jedného systému. Používateľ si bude môcť vyhľadať vhodnú trať podľa typu, lokality alebo obtiažnosti. Administrátor bude môcť pridávať a upravovať trate a zverejňovať oznámenia o pretekoch.

---

## 2. Dôvod a okolnosti zavedenia riešenia

Informácie o motokrosových, enduro a countrycross tratiach sú často rozdelené medzi rôzne webové stránky, sociálne siete, kluby a skupiny. Jazdec tak môže mať problém rýchlo zistiť, kde sa konkrétna trať nachádza, aký typ trate ponúka a aká je jej obtiažnosť.

Zavedenie jednotného systému umožní sústrediť tieto informácie na jedno miesto. Používateľ bude mať jednoduchý prehľad o tratiach na Slovensku a zároveň bude môcť sledovať oznámenia o pripravovaných pretekoch.

Cieľom systému je najmä:
- vytvoriť databázu motokrosových, enduro a countrycross tratí,
- umožniť vyhľadávanie a filtrovanie tratí,
- zobrazovať obtiažnosť jednotlivých tratí,
- poskytovať základné informácie o lokalite trate,
- zobrazovať oznámenia o pretekoch,
- umožniť administrátorom pridávať a upravovať obsah.

---

## 3. Popis projektu (slovné zadanie, popis od zákazníka)

Cieľom projektu je vytvoriť prehľadnú webovú aplikáciu pre jazdcov a fanúšikov motokrosu a endura. Systém bude obsahovať databázu tratí nachádzajúcich sa na Slovensku.

Každá trať bude mať svoje základné údaje, napríklad:
- názov trate,
- lokalitu,
- typ trate – **enduro, cross alebo countrycross**,
- stupeň obtiažnosti,
- stručný popis,
- prípadne ďalšie informácie podľa administrátora.

Súčasťou systému bude aj sekcia **Oznámenia o pretekoch**. Administrátor bude môcť vytvoriť oznámenie, ktoré bude obsahovať napríklad názov pretekov, dátum, miesto konania, typ pretekov a ďalšie informácie.

Bežný používateľ bude môcť:
- prezerať zoznam tratí,
- filtrovať trate podľa typu a obtiažnosti,
- zobraziť detail trate,
- prezerať aktuálne oznámenia o pretekoch.

Administrátor bude mať navyše možnosť:
- pridávať trate,
- upravovať trate,
- mazať trate,
- pridávať oznámenia o pretekoch,
- upravovať oznámenia,
- mazať oznámenia.

---

## 4. Analýza požiadaviek

### Funkčné požiadavky

**FR1 – Zobrazenie tratí**
- Systém zobrazí zoznam dostupných tratí.
- Pri každej trati sa zobrazí názov, typ a obtiažnosť.

**FR2 – Vyhľadávanie a filtrovanie**
- Používateľ môže vyhľadávať trať podľa názvu alebo lokality.
- Používateľ môže filtrovať trate podľa typu.
- Používateľ môže filtrovať trate podľa obtiažnosti.

**FR3 – Detail trate**
- Systém zobrazí detail vybranej trate.
- Detail obsahuje základné informácie o trati a jej lokalite.

**FR4 – Oznámenia o pretekoch**
- Systém zobrazí zoznam aktuálnych oznámení.
- Používateľ môže otvoriť detail konkrétneho oznámenia.

**FR5 – Správa tratí administrátorom**
- Administrátor môže vytvoriť novú trať.
- Administrátor môže existujúcu trať upraviť.
- Administrátor môže trať odstrániť.

**FR6 – Správa oznámení administrátorom**
- Administrátor môže vytvoriť nové oznámenie o pretekoch.
- Administrátor môže oznámenie upraviť.
- Administrátor môže oznámenie odstrániť.

### Nefunkčné požiadavky

- Aplikácia má byť jednoduchá na používanie.
- Obsah má byť prehľadný aj na mobilnom zariadení.
- Systém má reagovať na používateľské požiadavky v krátkom čase.
- Údaje uložené v databáze musia byť konzistentné.
- Administrátorské funkcie musia byť dostupné iba oprávnenému používateľovi.

---

## 5. Systémové požiadavky (FURPS)

### 1. Funkčnosť (Functionality – F)

- Zobrazenie databázy motokrosových, enduro a countrycross tratí.
- Vyhľadávanie a filtrovanie tratí.
- Zobrazenie obtiažnosti trate.
- Zobrazenie detailných informácií o trati.
- Zobrazenie oznámení o pripravovaných pretekoch.
- Správa tratí administrátorom.
- Správa oznámení administrátorom.

### 2. Vhodnosť k použitiu (Usability – U)

- Jednoduché a intuitívne používateľské rozhranie.
- Prehľadné rozdelenie tratí podľa typu.
- Jednoduché filtrovanie podľa obtiažnosti.
- Použiteľnosť na počítači aj mobilnom zariadení.

### 3. Spoľahlivosť (Reliability – R)

- Systém má správne zobrazovať uložené údaje.
- Pri chybe databázy alebo servera má systém používateľa informovať o probléme.
- Úprava alebo odstránenie údajov má byť vykonaná konzistentne.

### 4. Výkon (Performance – P)

- Zoznam tratí sa má načítať bez zbytočného oneskorenia.
- Filtrovanie a vyhľadávanie má byť dostatočne rýchle.
- Systém má zvládnuť bežný počet používateľov bez výrazného spomalenia.

### 5. Schopnosť údržby (Supportability – S)

- Jednoduché pridávanie nových tratí a typov údajov.
- Jednoduchá úprava oznámení.
- Možnosť rozšíriť systém o ďalšie funkcie v budúcnosti.
- Zdrojový kód má byť organizovaný tak, aby sa dal ďalej upravovať.

---

## 6. Kritické situácie

### 1. Systémové

- **Výpadok servera:** Používateľ sa nebude môcť dostať k databáze tratí a oznámeniam.
- **Výpadok databázy:** Systém nebude schopný načítať alebo uložiť údaje.
- **Strata údajov:** Pri poškodení databázy môže dôjsť k strate informácií o tratiach alebo pretekoch.

### 2. Aplikačné

- **Neplatné údaje:** Administrátor sa pokúsi vytvoriť trať bez povinných údajov.
- **Chyba pri ukladaní:** Údaje sa nepodarí uložiť do databázy.
- **Neoprávnený prístup:** Bežný používateľ sa pokúsi použiť administrátorské funkcie.
- **Neexistujúca trať:** Používateľ otvorí odkaz na trať, ktorá bola odstránená.

Systém by mal v týchto prípadoch zobraziť zrozumiteľné chybové hlásenie a podľa možnosti používateľovi umožniť pokračovať v aplikácii.

---

## 7. Hranice systému

### 1. Ideálny scenár

Používateľ otvorí aplikáciu, vyhľadá požadovanú lokalitu alebo typ trate, vyfiltruje požadovanú obtiažnosť a zobrazí detail vybranej trate. Zároveň môže skontrolovať aktuálne oznámenia o pretekoch.

### 2. Hranične riešiteľný scenár

Používateľ hľadá trať, ktorá sa v databáze nenachádza. Systém zobrazí informáciu, že požadovaná trať nebola nájdená.

### 3. Situácie, ktoré systém nezvládne

Systém nebude schopný poskytovať informácie, ktoré nie sú uložené v databáze alebo ktoré neboli pridané administrátorom. Nebude tiež zodpovedať za aktuálny stav trate, ak tieto informácie administrátor nezmení.

---

## 8. Kontext prostredia

Systém bude implementovaný ako webová aplikácia dostupná prostredníctvom internetového prehliadača. Bude pracovať s databázou, v ktorej budú uložené informácie o tratiach a oznámeniach.

Používateľ bude systém používať prostredníctvom:
- počítača,
- notebooku,
- tabletu,
- mobilného telefónu.

Systém bude závisieť najmä od:
- webového servera,
- databázového systému,
- internetového pripojenia,
- webového prehliadača.

---

## 9. Charakteristika aktérov

### Bežný používateľ / jazdec

Používateľ, ktorý chce nájsť vhodnú motokrosovú, enduro alebo countrycross trať alebo získať informácie o pripravovaných pretekoch.

**Môže:**
- prezerať trate,
- vyhľadávať trate,
- filtrovať trate,
- zobrazovať detaily tratí,
- prezerať oznámenia o pretekoch.

### Administrátor

Používateľ s rozšírenými oprávneniami, ktorý sa stará o obsah systému.

**Môže:**
- pridávať trate,
- upravovať trate,
- mazať trate,
- pridávať oznámenia,
- upravovať oznámenia,
- mazať oznámenia.

### Prostredie

- Webový prehliadač.
- Webový server.
- Databáza.

---

## 10. Use Case diagram



---

## 11. Scenáre (Implementácia Use Case)

### 1. Vyhľadanie a zobrazenie trate

- **Názov:** Vyhľadanie enduro trate podľa lokality
- **Kontext:** Jazdec chce nájsť enduro trať v požadovanej lokalite.
- **Level zanoření Use Case:** Hlavný scenár
- **Aktéri:** Bežný používateľ
- **Stakeholdeři a zájmové osoby:** Jazdci, návštevníci tratí
- **Vstupné podmienky:** Systém obsahuje databázu tratí.
- **Výstupné podmienky:** Zobrazí sa zoznam zodpovedajúcich tratí.
- **Minimálny výstup:** Zobrazenie názvu a typu trate.
- **Ideálny výstup:** Zobrazenie všetkých relevantných informácií o vybranej trati.

**Hlavný scénár:**
1. Používateľ otvorí stránku s traťami.
2. Do vyhľadávania zadá názov alebo lokalitu.
3. Systém vyhľadá zodpovedajúce trate.
4. Systém zobrazí výsledky.
5. Používateľ vyberie konkrétnu trať.
6. Systém zobrazí detail trate vrátane typu a obtiažnosti.

**Rozšírenie:**
- Ak sa žiadna trať nenájde, systém zobrazí informáciu „Trať nebola nájdená“.

---

### 2. Filtrovanie tratí podľa obtiažnosti

- **Názov:** Výber trate podľa obtiažnosti
- **Kontext:** Jazdec chce nájsť trať zodpovedajúcu jeho úrovni.
- **Level zanoření Use Case:** Hlavný scenár
- **Aktéri:** Bežný používateľ
- **Vstupné podmienky:** V databáze sa nachádzajú trate s definovanou obtiažnosťou.
- **Výstupné podmienky:** Systém zobrazí iba trate zodpovedajúce zvolenému filtru.

**Hlavný scénár:**
1. Používateľ otvorí zoznam tratí.
2. Vyberie požadovaný stupeň obtiažnosti.
3. Systém aplikuje filter.
4. Systém zobrazí zodpovedajúce trate.

**Rozšírenie:**
- Ak neexistuje žiadna trať s vybranou obtiažnosťou, systém zobrazí prázdny výsledok.

---

### 3. Zobrazenie oznámenia o pretekoch

- **Názov:** Zobrazenie informácií o pripravovaných pretekoch
- **Kontext:** Jazdec chce získať informácie o pripravovanom podujatí.
- **Level zanoření Use Case:** Hlavný scenár
- **Aktéri:** Bežný používateľ
- **Vstupné podmienky:** V systéme existuje oznámenie.
- **Výstupné podmienky:** Používateľ vidí podrobnosti o pretekoch.

**Hlavný scénár:**
1. Používateľ otvorí sekciu Oznámenia.
2. Systém zobrazí zoznam oznámení.
3. Používateľ vyberie konkrétne preteky.
4. Systém zobrazí detail oznámenia.
5. Používateľ si prečíta dátum, miesto a ďalšie informácie.

**Rozšírenie:**
- Ak oznámenie už nie je dostupné, systém zobrazí informáciu, že oznámenie nebolo nájdené.

---

### 4. Pridanie trate administrátorom

- **Názov:** Pridanie novej trate
- **Kontext:** Administrátor chce pridať novú trať do databázy.
- **Level zanoření Use Case:** Hlavný scenár
- **Aktéri:** Administrátor
- **Vstupné podmienky:** Administrátor je prihlásený.
- **Výstupné podmienky:** Nová trať je uložená v databáze.

**Hlavný scénár:**
1. Administrátor sa prihlási.
2. Otvorí administráciu tratí.
3. Vyberie možnosť „Pridať trať“.
4. Vyplní názov, lokalitu, typ a obtiažnosť trate.
5. Doplní popis a ďalšie údaje.
6. Potvrdí uloženie.
7. Systém skontroluje údaje.
8. Systém uloží trať do databázy.
9. Nová trať sa zobrazí v zozname.

**Rozšírenie:**
- Ak chýba povinný údaj, systém trať neuloží a zobrazí upozornenie.

---

### 5. Pridanie oznámenia o pretekoch

- **Názov:** Vytvorenie oznámenia o pretekoch
- **Kontext:** Administrátor chce informovať používateľov o pripravovaných pretekoch.
- **Level zanoření Use Case:** Hlavný scenár
- **Aktéri:** Administrátor
- **Vstupné podmienky:** Administrátor je prihlásený.
- **Výstupné podmienky:** Oznámenie je uložené a zobrazené používateľom.

**Hlavný scénár:**
1. Administrátor sa prihlási.
2. Otvorí administráciu oznámení.
3. Vyberie možnosť „Pridať oznámenie“.
4. Zadá názov pretekov.
5. Zadá dátum a miesto konania.
6. Vyberie typ pretekov.
7. Doplní podrobnosti.
8. Potvrdí uloženie.
9. Systém skontroluje údaje.
10. Systém uloží oznámenie.
11. Oznámenie sa zobrazí v sekcii pre používateľov.

**Rozšírenie:**
- Ak administrátor nezadá povinné údaje, systém oznámenie neuloží.

---

## 12. Sekvenčný diagram

Sekvenčný diagram môže znázorňovať proces vyhľadania trate.

**Účastníci:**
- Používateľ
- Webové rozhranie
- Aplikačný server
- Databáza

**Postup:**
1. Používateľ zadá názov alebo lokalitu trate.
2. Webové rozhranie odošle požiadavku aplikačnému serveru.
3. Aplikačný server odošle dotaz do databázy.
4. Databáza vyhľadá zodpovedajúce trate.
5. Databáza odošle výsledky serveru.
6. Server odošle výsledky webovému rozhraniu.
7. Webové rozhranie zobrazí výsledky používateľovi.
8. Používateľ môže vybrať konkrétnu trať.
9. Systém následne zobrazí jej detail.

---

## 13. Triedny diagram

Triedny diagram môže obsahovať najmä tieto triedy:

### User
- `id`
- `meno`
- `email`
- `heslo`
- `rola`

**Metódy:**
- `login()`
- `logout()`

### Track
- `id`
- `nazov`
- `lokalita`
- `typ`
- `obtiaznost`
- `popis`

**Metódy:**
- `createTrack()`
- `updateTrack()`
- `deleteTrack()`

### RaceAnnouncement
- `id`
- `nazov`
- `datum`
- `miesto`
- `typPretekov`
- `popis`

**Metódy:**
- `createAnnouncement()`
- `updateAnnouncement()`
- `deleteAnnouncement()`

### Database
- údaje o používateľoch
- údaje o tratiach
- údaje o oznámeniach

**Vzťahy:**
- `User` môže spravovať viac objektov `Track`.
- `User` môže spravovať viac objektov `RaceAnnouncement`.
- `Track` predstavuje jednu trať v databáze.
- `RaceAnnouncement` predstavuje jedno oznámenie o pretekoch.
- `Database` uchováva používateľov, trate a oznámenia.

---

## 14. Záver

Navrhovaný systém MotoTrack Slovakia má za cieľ vytvoriť jednotné miesto pre informácie o motokrosových, enduro a countrycross tratiach na Slovensku a o pripravovaných pretekoch.

Systém umožní používateľom jednoduchšie vyhľadávať trate podľa typu, lokality a obtiažnosti a zobrazovať ich základné informácie. Administrátor bude môcť obsah systému priebežne aktualizovať a pridávať nové trate a oznámenia o pretekoch.

Návrh je vytvorený tak, aby sa dal v budúcnosti rozšíriť napríklad o mapové zobrazenie tratí, fotografie, hodnotenie tratí, registráciu používateľov, komentáre alebo podrobnejšie informácie o pretekoch.
