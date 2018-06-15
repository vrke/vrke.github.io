# Informatika Biztonság

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

## Támadások kategorizálása

- Aktivitás szerint: Aktív (egy fájl letörlése), Passzív (lehallgatás)
- Forrás szerint: Külső támadás (hacker), Belső támadás (dolgozó)
- Célpont szerint: Hardver, Szoftver, Adat, Kommunikációs csatorna

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
     - hjf
- Üzletmenet folytonosság (business continuity)
- MTBF (Mean Time Between Failure) Meghibásodások között eltelt átlag idő
- MTTR (Mean Time To Repair) Javítás átlagos időtartama
- Hiba Megelőzés
  1. Minőségi alkatrészek
  2. beszerzés politika
  3. Hibákat előre jelezzük (Jelzés esetén csere -> tervezhető -> hiba megelőzés)

## Scanning

Letapogatás. Olyan tevékenység ami során azonosítjuk a hosztokat/portokat/szolgáltatásokat a hálózaton.

### Network scan

### Port scan

### Vulnerability scan

## Fontos szarok

- Tcp 3utas kézfogás SYN SYNACK ACK
- Wiretrapping  „A lehallgatás az a folyamat, amikor egy harmadik fél  telefon  vagy számítógép  hálózati  forgalom megfigyelést végez.
- Magas rendelkezésre állás : Olyan rendszer, amelynek felépítést úgy tervezték, hogy a meghibásodások mértékének csökkentésével minimalizálják a szolgáltatás kimaradásának idejét.
  1. HA % = (T müködés/ T üzem) * 100
  2. HA % = [(T üz - SZUM üz \* T kihagy) / T üz] \* 100
