# Infóbizt

## 2018 tavasz kérdések amik már voltak

- Beugrók
  - 2.3 / 4.(7) /
  - (PP 2018 Május 27 Facebook)
 Volt két beugró a kötelező kérdésekből.
 Kritikus szekció-kölcsönös kizárás, Szál-processzus.
Volt Bélády anomália,
Round Robin ütemezés
RAID tömbök
lapozási technikák
hogyan jön létre holtpont
holtpont megelőzési módszerek
Kernel és user szálak közötti különbség. Memóriatöredezettség.

## Beugrók

1. Oprendszer és a kernel foglamla
2. Processzus és a szál foglama
3. Kritikus szekció és a kölcsönös kizárás
4. Rendszerhívások és megszakítások
5. Szemafor
6. Ütemezés, preemtív és nem preemtív
7. Külső Belső töredezettség.
8. Relokációs követelmény a memória kezelés szempontjából
9. MMU és mi a fő feladata
10. Virtuális Tárkezelés és Laphiba
11. Laptábla TLB
12. Karakteres És blokkos eszközök közötti különbség
13. RAID
14. DMA
15. Filerendszer Fogalma

## Kérdések

- multiprogramozás (1.előadás)
- hol kell egy adatnak és egy utasításnak elhelyezkednie, h végre hajtaható  legyen
- egyszerű cpu modell, rajz,működése (1.előadás)
- absztrakt gép (1.előadás)
- milyen processzor információkat kell nyilvántartani, hol mik ezek (1.előadás)
- IO fejlődés lépései, kapcsolodó feladatok 
- versenyhelyzet elkerülésének 4 feltétele (1.előadás)
- blokkkonzisztencia ellenőrzés, használat, hiba, javítás (10-11.előadás)
- vergődéskialakulása, grafik (7.előadás)
- Felhasználói és Kernel szintű szálak ütemezése
- SJF
- Programozott I/O
- Rendszerhívás lépései
- Hardveres megoldások processzusok kommunikációja során
- Hogyan működik a DMA vezérelt i/o rajzzal együtt
- Mi a különbség processzus és szál ütemezése között?
- A három állapotú processzus modell szerint milyen három fő állapotban lehet egy processzus és milyen átmenetek lehetnek a processzusok között? Írja le őket röviden!
- sleep-wake(alvás-ébredés): példa rá és megmagyarázni
- Ütemező algoritmusok
- Memória algoritmusok
- Mutex leírása
- Átbocsátó képesség ütemezés során
- Round Rubin ütemezés
- mik azok a monitorok
- Processzus táblázat milyen információt tárol? Milyen 3 csoportba osztható
- Mi az az éhezés?
- Rajzolja le a memória hierarchiát
- Milyen módszereket ismer az adott fájlhoz tartozó lemezblokkok nyilvántartására?
- Mi az a DMA. Magyarázza el és rajzolja le a működését.
- RAID0 RAID1 előnyei és hátrányai.
- Versenyhelyzet kialakulásra egy példa.
- Multilevel Queues.
- Round robin algoritmus.
- Bankáralgoritmus
- i csomópont

## Téma szerint a kérdések

- Holtpont
    1. Mi az a holtpont adjon példát
    2. Erőforrás számozás miben segíthet  a holtpontoknál?
    3. a holtpont kialakulásának 4 szükséges feltétele (soroljon fel 2-t)
    4. Milyen stratégiákat ismer a holtpont  megelőzésére?
- UNIX
    1. Unix ütemezése.
    2. Processzor állapotok unix alatt, processzorátmenetek
    3. Értékelje a unix prioritásos ütemezését
- Lap és Keret
    1. Mi a laptábla, hol használatos?
    2. Lapméret és keret közötti összefüggés
- Memória foglalás
    1. First Fit
    2. Next-fit memóriafoglalás.
    3. Írja le hogy mit jelent a Quick-Fit memóriafoglalási algoritmus? Előnyök, hátrányok
    4. worst-fit memóriafoglalási stratégia előnyei és hátrányai
    5. quick fit
    6. Fontos egyéb
- Lemezfej ütemező Algoritmus
    1. FIFO(first in first out)
    2. SSTF shortest seek time first
    3. c-scan(lemezfej ütemező algoritmus)(9.előadás)
    4. ELEVATOR, lift algoritmus
- Ütemezés
    1. algoritmusok
        - FCFS
        - Round Robin
        - SJF
- Egyéb
    1. Éhező filozófusok probléma(Dijkstra)
    2. Belady anomália
