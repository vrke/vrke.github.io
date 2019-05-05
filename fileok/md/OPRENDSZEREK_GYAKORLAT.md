# Oprendszerek GYAKORLAT

193.225.19.239:22 putty szerver ip.

## Parancsok

- whoami
- who - kik vannak bejelentkezve
- pwd - print working directory
- man - parancsnev -manual - help
- cat
  - cat > fajl (fájl létrehozása)
  - cat fajl  (a fájl kiiratása)
- cd -  change directory
  - cd .. - feljebb menni egy könvtárral
  - cd ~ sajat munka mappa
  - cd / root
- chmod
  - chmod ugo+rwx filenev
  - chmod 740 file > user mindent | group olvas | others semmit
- ls - list;  -l (hosszú kiírás)  ls -lR filenev /rekurzivan kiiratja a mappa tartalmat hosszan
- touch filnev ->file letrehozasa.
- mkdir - make directory
- rmdir -remove directory
- rm - remove
- ln - link
- traceroute
- free -m
- cp
- mv
- sed
- grep

## elérés

- relatív
  - /ahol vagy/mappa/filenév
- Abszolút elérés
  - /gyökér/mappák/file >> /home/NÉV/mappa/mappa/file
  - ../mappa > visszalépéssel parancskiadás

## chmod filemódbitek változtatása  UGO RWX 421

- User Group Others `+ - =` Read Write eXecute  (nagybetü a kisbetü)
- [ugoa] `+ - =` [rwxXst]
- cat </etc/passwd
- chmod u+x filenév
- chmod ugo+rwx filenev
- r=4 w=2 x=1
- chmod 740 file > user mindent | group olvas | others semmit
- tehat u=7=rwx g=4=read o=0

|\\ |x  |w  |r  |wx |rw |rwx|
|---|---|---|---|---|---|---|
|o  |001|002|004|003|005|007|
|g  |010|020|040|030|050|070|
|u  |100|200|400|300|500|700|
|go |011|022|044|033|055|077|
|ug |110|220|440|330|550|770|
|ugo|111|222|444|333|555|777|

- NÉV:x:1222:1001::/home/NÉV:/bin/bash
- felhaszn:jelszo:userid:groupid

## Átirányítás

st bemenet 0 <   0>
st kimenet 1 >	 1>	
st hiba    2   	 2>

- 1>&2 melyik csatornát hova irányítunk(itt az egyest a kettesbe) a standardkimenetet atiranyitottuk es masoltuk a hiba csatornaba `cat <allatok/kutyak/pointer >allatok/pointermasolat`
- a pointer bemenetét atiranyitottuk a masolat kimenetere. `cat <allatok/kutyak/pointer <<VALAMIKARAKTERLANC`
- addig ir be a filbe ameddig el ne eri a karakterlancot amit megadtunk. `hozzafuzeshez out>> ketoldalunyilak<<input`

## VI szovegszerkeszto

- vi filenév (állomány létrehozása)
- esc normal mode utana : es lehet menteni dd(sortörlés)x(karaktertörlés)o(uj ssor beszúrása)
- ment q! kilép mentés nélkül
- beszúró mód i(insert) a(append)
- parancs mód : w(mentés) q(kilép) wq(kilép és ment)

## Pipeok / Csatornák

- more parancs ->feltördeli oldalakra tördelve a filet.
- wc filenev ->ujsor, szó, és bit számot ír ki a fileokra -m karakterhossz, -L leghosszabb sor.
- Pipeba a | karakterrel rakhatunk be
- `ls | wc -w` kiirja mennyi listázott szó van az ls parancs hatására, indirekt mód a filedarabszám megállapítására.
- `ls -l |wc -l`  kiirja a reszletes listát majd megszámolja hány sorbol áll.

## GREP

- `grep <minta> <file>` -> az adott mintát keresi az adott fileba majd vissza adja azt a sort.
- `grep -i` -> ignorolja a casesensitivity -t.
- `grep -v`
- `grep NÉV /etc/passwd | cat > sajat`  megkeres egy adott patternet a helyen majd letrehoz egy filet és átirja azt a sort.
- `grep NÉV /etc/passwd > sajat` atiranyitja a sort  amit a grep ad a sajatba.

## Filenév megdási módok

- `file?` az utlso karakter illeszkedik.
- `*file file*`az állománynév elejére/végére illeszkedik.
- `file[a123]`Filera illeszkedik megadott karakter.
- `file[A-Z]` Filera illeszkedik egy intervallum.
- `file[^A-Z]`tagadás.

## Find parancs

- Kiindulási konyvtar opciok
  - maxdepth n - mindepth n -> .
- tesztek
  - n +n -n pontosan n, nagyobb mint n, kissebb mint n.
- Access
- Create
- Modify

példa

- `find ~ -size +1000k -and -size -2000k`
  - amin (-+)n -> file legutóbbi elérése utáni eltelt idő percben.
  - mmin (+-)n ->file modositasa utan eltelt ido percben.
  - empty
- `ls -l | tail -n 5 | sort -r` utolso 5 eredményt irja ki fordított sorrendben. n helyére belehet írni a számot is.
- `head -n 3 bolygok | tail -1` a harmadik sort adja vissza.
- `ls pont* | sort -r`
- `find ~ -type d -and -name 'pict*'` forditott sorrendel vissza adja a mappakat amiben van pont
- `| uniq` ->kiszűri az ismételt sorokat.

## LINKEK

-ln mirelinkel linkneve
-ln -s mirelinel linkneve
-egrep -i -> case sensytivityt leveszi.

## AWK

- `awk 'BEGIN {for (  i = 0 ; i <= 10 ; i++) print(i)}'` kiírja a számokat 0 tol 10 ig
- hanincs begin akkor nem indul el.
- kell a kis aposztrof izé jel is [`'`] mert az határolja parancsot.
- AWK globális változók
  1. NR NUMBER OF RECORDS.  alap értelmezésként egy sor, mert a RS (record separator a sor törés(enter).
  2. NF  NUMBER OF FIELDS.   egy rekord egy mezője egy szó kb alapértelmezés szerint Field separator a space/tab.
  3. FS FIELD SEPARATOR FS= ";"
  4. RS  RECORD SEPARATOR.  RS= ";" Az alap RS="\n"  Át lehet állítani a separatort a saját kedvünkre fenti módon.
- `awk '{if (NR % 2 == 0 )  print $0}' filenév` kiiratja minden második sort a fileban
- `$0` a teljes rekordot kiiratja
- a filenév a '' on kivül kell hogy legyen
- itt begin nem működik.
- `awk 'END {print NR}' fájl`  kiírja mennyi sorból áll end helyett lehet |tail -1

## SHELL SCRIPTEK [plusz anyag lehet nem müködik a kód]

Első

>1. `touch elsocript` létrehozuk a filet
>2. `cat >> elsocript` beleirányitunk tartalmalt
>3. `#!/bin/sh` ez az "SH paracs" `sh elsocript`  el lehet majd meghívni ezt a scriptet. bővebben [ITT](https://stackoverflow.com/questions/13872048/bash-script-what-does-bin-bash-mean) ez egy hely ahol tárolva vannak a scriptek.
>4. `ls | wc -w`  kilistáz és megszámolja
>5. `ctrl +c` kilépünk
>6. `chmod 744`

Második

>1. `touch masodikscript`
>2. `cat udvozles`
>3. `#!/bin/bash`
>4. `echo -n "Hogy hívnak?"`
>5. `read nev`
>6. `echo "Üdvozlom $nev !"`
>7. `ctrl +c`
>8. `chmod 744 udvozles`  futtatási jogot kell adni mert nem müködik külömben

---

## Feladatok

- Adjon parancsot, mellyel az adott alkönyvtár összes 200 byte-nál hosszab filenevét és hosszát kilistázza,rekurzív módon (könyvtárakat nem).

- Adjon parancsot, mellyel PoSH-ben lekérdezheti a négy legutóbb írt állományt.

- Hozzon létre `$hany` változóban tárolt mennyiségű file-t `[sorszam1]_[nev]` formaban. A `[sorszam1]` induljon 0-tól, növekedjen 3-asával addig, míg a sorszám kisebb mint a `$darab`-ban megadott érték. (a `$hany` valtozo erteket mas adja meg, csak ugy, mint a `$darab` valtozo erteket is. Pl., ha `$hany==5` és `$darab==7`, akkor ezeket kell, hogy letrehozza a szkript:
  - 0_valami
  - 3_valami
  - 6_valami és itt megáll, hiába 5 darabot kellene létrehozni, de a `$darab==7`, tehát 9_valami már nem lehet.)