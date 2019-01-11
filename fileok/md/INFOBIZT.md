# Informatika Biztonság

## Definíciók

- **Az információs társadalom** (information society) elmélete szerint a társadalomban az információ előállítása, elosztása, terjesztése, használata és kezelése jelentős gazdasági, politikai és kulturális tevékenység.Ezen  társadalom  sajátossága  az információ-technológia (IT) központi szerepe a termelésben, a gazdaságban és általában a társadalomban

## CIA háromszög triad

- Confidentiality ▫ Bizalmasság
- Integrity ▫ Sértetlenség
- Availability ▫ Rendelkezésre állás Az informatikai rendszer és az abban tárolt adatok az arra jogosult személyek számára elérhetők.

## A biztonság 3 alappillére

- **Fizikai (infrastruktúra) védelem  :** fizikai térben megvalósuló fenyegetések elleni védelem, amelynek fontosabb részei a természeti csapás elleni védelem, a mechanikai védelem, az  elektronikai jelzőrendszer, az élőerős védelem, a beléptető rendszer, a megfigyelő rendszer, a tápáramellátás, a sugárzott és vezetett zavarvédelem, klimatizálás és tűzvédelem.
- **Adminisztratív (Ügyviteli) védelem:** az informatikai rendszert üzemeltető szervezetbe épített biztonsági szabályok, amelyeket az informatikai biztonsági szabályzat ír le. A fizikai védelemre épül, a biztonság egy következő lépcsőfoka.
- **Algoritmikus (logikai) védelem:** azokból az eljárásokból áll, amelyek a rendszer szolgáltatásaival egyidejűleg látja el a védelmi feladatokat. Eszközei: adatok

## Védelmi eszközök

Antivirus, Tűzfal, Kémprogram, Kriptográfia, Felhasználó azonosítás, VPN, Naplózás, Behatolás jelző(IDS, Intrusion Detection System), megelőző rendszer, Audit, Antivirus,

## Védelem

- Management plane
  - Rendszer konfiguráció (CLI, GUI)
  - Hozzáférési protokollok (TELNET, SSH)
  - Rendszer felügyelet (SNMP) Simple Network Management Protoco
- SOHO router védelme
  1. Admin jelszó!
  2. HTTPS en keresztöl konfiguráljunk, lehetőleg wifit kerülve
  3. wireless kapcsolat titkosítása
     - WPA2 használata (WEP gyenge)
     - Default SSID megváltoztatása
     - SSID Broadcast Tiltása
     - wireless macfilter
- Enterprise Router Védelme
  - Erős Jelszavak
  - AAA kialakítása
    1. Authentikáció Lokális/Centralizált TACACS+, RADIUS
    2. Authorizáció (RBAC) RoleBasedAccessControl
    3. Audit -Logolás, SNMPv3, NetworkTime Protocol
  - Titkosított Management protokolok használata: SSH
  - RouterVédelem
    1. Jelszó privilegizált mód  (console vty aux)
       - `enable password` (titkosítatlan jelszó)
       - `enable secret` (erős titkosítású jelszó)
       - `(config)#service password-encryption` Jelszavak titkosítása

## Hiba fogalmak

- Hiba lehet szofteres vagy hardveres.
  1. Meghibásodás/hibaok(fault)
  2. Hiba (Error)
  3. Hiba Jelenség(Failure)
- Hiba kezelés
  1. Hiba megelőzés(fault avoidance)
     - Minőségi alkatrészek
     - beszerzés politika
     - Hibákat előre jelezzük (Jelzés esetén csere -> tervezhető -> hiba megelőzés)
  2. Hiba rejtés(fault masking) a meghibásodást hibává fejlődéstől véd
  3. Hiba tűrés (fault tolerance)
- Üzletmenet folytonosság (business continuity)
- MTBF (Mean Time Between Failure) Meghibásodások között eltelt átlag idő
- MTTR (Mean Time To Repair) Javítás átlagos időtartama
- Hiba Megelőzés
  1. Minőségi alkatrészek
  2. beszerzés politika
  3. Hibákat előre jelezzük (Jelzés esetén csere -> tervezhető -> hiba megelőzés)

## Támadás

- lehet: Fizikai, Szociális, Elektronikus.
- eszközök : lopás ezközök tönkretétele |social engineering |Kali, Backtrack

### Támadások kategorizálása

- Aktivitás szerint: Aktív (egy fájl letörlése), Passzív (lehallgatás)
- Forrás szerint: Külső támadás (hacker), Belső támadás (dolgozó)
- Célpont szerint: Hardver, Szoftver, Adat, Kommunikációs csatorna

### Támadás folyamata

1. Előkészület (Preparaton)
2. Felderítés (Reconissance) Leg időigényesebb (95%)
3. Letapogatás (Scanning)
4. Hozzáférés szerzés (Gaining access)
5. Hozzáférés fenntartás(Maintaining access)
6. Jelentés/Nyomok eltüntetése (Report / Covering Tracks)

- 3+4 együtt a helyzet kihasználása / exploit
- a ciklus 2345 folyamatos
- Vulnerability: sérülékenység, sebezhetőség
- Exploit:  programkód, amely kihasználja a  sebezhetőséget
- Payload:  a hozzáférésen keresztül bejuttatott program(kód)
- **Exploitation** A felfedezett  sérülékenységek/sebezhetőségek kihasználása és kontroll megszerzése a cél felett
- **Exploit** Olyan   kód,   amely   a   távoli   rendszer sebezhetőségét   kihasználva   lehetővé   teszi payload bejuttatását a célrendszerbe
- **Payload** Olyan  kód,  amely  a  célrendszeren  futtatva lehetővé teszi a hozzáférést.
  1. Bind payload  Exploit A->V Kapcsolat A->V
  2. Reverse Payload Exploit A->V Kapcsolat A<-V
  3. VNC(Cirtual Nevtwork Computing) Gépek távoli Irányítása
  4. Meterpreter(Meta Interpreter) Commandshell, memóriában fut, lopakodó technika
- Lépések (Exploit)
  1. Exploit kiválasztása, betöltése (use exploit)
  2. Payload kiválasztása, betöltése (set payload)
  3. Opciók beállítása (set)
      - Exploit paraméterek
      - Payload paraméterek
  4. Exploit indítása (exploit)

### Külömböző támadások

- Web szerver ellen : WebsiteDefacment, Directory traversal, Űrlap szabotázs(FormTampergin), SQL injection, XSS(Crosssite sctipting), CSRF(CrossSiteRequestForgery)
- DNS felderítés
- Tracroute
- Google hacking
- Email tracking
- The harvester: Internet footprint  meghatározása
- Wiretapping (monitoring/ +injecting)
- Packet sniffing (Promiscous módban minden forgalmat)

## Scanning

Letapogatás. Olyan tevékenység ami során azonosítjuk a hosztokat/portokat/szolgáltatásokat a hálózaton.

- NETWORK SCAN
- PORT SCAN
- VULNERABILITY SCAN

## Fontos szarok

- NITS (Nemzeti Információs Társadalom Stratégia)
- Tcp 3utas kézfogás SYN SYNACK ACK
- Wiretrapping  „A lehallgatás az a folyamat, amikor egy harmadik fél  telefon  vagy számítógép  hálózati  forgalom megfigyelést végez.
- Magas rendelkezésre állás : Olyan rendszer, amelynek felépítést úgy tervezték, hogy a meghibásodások mértékének csökkentésével minimalizálják a szolgáltatás kimaradásának idejét.
  1. HA % = (T müködés/ T üzem) * 100
  2. HA % = [(T üz - SZUM üz \* T kihagy) / T üz] \* 100
