# Analízis 1

[Anal 1](http://ttk.pte.hu/matek/numanal/ttk_elemei/gianal/analizisgi01-02het.pdf)

## HALMAZELMÉLET

||jelmagyarázat|
|-|-|
|∩|metszet|
|∀|minden|

### Halmaz

A halmaz a közös tulajdonsággal bíró dolgok összessége/sokasága/rendszere/osztálya.
Nagybetűvel jelöljük: A,B,C KIVÉTEL> N,Z,Q,Q*,R
A halmaz elemeit kisbetűvel jelöljük: a,b,c  KIVÉTEL> x
 Egy halmaz adott ha egy dologról egyértelműen eldönthető hogy:
-- Hozzátartozik a halmazhoz, elemei a halmaznak.[a eleme A (fura e betű a jele)
-- nem tartozik hozzá a halmazhoz, nem elemei a halmaznak.[b nem eleme A nak  (a jel áthúzva)
Tétel: Ha egy halmaznak *n* db eleme van akkor *2n* részhalmaza van.

### Halmazok szemléltetése

- Venn-diagrammal történik.
- Vagy a halmaz jele és az elemek felsorolása kapcsos zárójelek között vesszővel elválasztva. A = {a,b,c,d}

### Üres halmaz

Üres halmaz az a halmaz amelynek egyetlen eleme sincsen.
Jele egy áthúzott karika vagy {}

### Számhalmazok

 Azokat a halmazokat, amelyeknek elemei számok számhalmazoknak nevezzük.
|Jel|Név|kiegészítés|
|-:|:-|:-|
| N| Természetes számok|N = {0,1,2,3...}
| Z |Egész számok |Z = {...-1,0,1...}
| Q| Racionális számok |Q = {p/q (p,q eleme Z) q nem 0} Véges illetve végtelen szakaszos törtek
| Q* | Irracionális számok |O*= {Pi, gyök2, egyéb végtelen nem szakaszos törtek}
| R| Valós számok |R = {Véges vagy végtelen törtek halmaza}
| C| Komplex számok |C = {i+-1 alakú számok}

### Ábrázolások

- A valós számok halmaza és a számegyenes pontjai között kölcsönösen egyértelmű megfeleltetés létesíthető
- A halmaz elemeit számegyenesen ábrázoljuk

### Definíciók

- 2 hamaz egyenlő ha elemei megegyeznek A={a,b} B={a,b} A=B
- A halmaz a B halmaz részhalmaza ha A minden eleme eleme B-nek  A(c alatt vonal)B
- A halmaz VALÓDI részhalmaza B nek ha A minden elme eleme Bnek, de Bnek van olyan eleme ami nem eleme A nak
- A c B  //A valódi részhalmaza Bnek
- {} c A //az üreshalmaz valódi részhalmaza Anak
- Ha egy halmaznak n darab eleme van akkor 2^n darab részhalmaza van pl.: A={1,2,3,4,5} 2^5 részhalmaza van Anak.

## Műveletek halmazokkal

## Únió

   Az A és B halmaz únióján mind azon elmek halmazát értjük
 amelyek vagy A vagy B vagy mindkét halmaz eleme
   A u B  = {x | x eleme A vagy x eleme B}

### Metszet

Az A és B halmaz metszetén azon elemek halmazát értjük amelyek elemei Anak és Bnek is
  A (forditott u) B = {x| x eleme A és x eleme B}
 2 halmaz DISZJUNKT ha nincs közös elemük, azaz metszetük üreshalmaz

### Külömbség

  Az A és b halmaz külömbségén mindazon elemek halmazát értjük amelyek
eleme az A halmaz összes olyan eleme ami nem eleme Bnek

  A\B  = {x| x eleme A, x nem eleme B}

### Komplementer

Legyen A részhalmaza H nak
A halmaz komplementer halmazán azt a halmazt értjük amelynek
elemei az alaphalmaznak mindazon elemei amelynek a halmaznak nem eleme

  XXX

### Halmazok descartes féle sorozata

Legyen A ls B nem üres halmaz.
A és B elemeiből készíthető rendezett párok az olyan (a,b) alakú szimbólumok,
ahol a pár első tagja az A eleme a második tagja a B eleme.
Az A és B halmazok elemeiből készített rendezett párok halmazát
az A és B halmazok Descartes féle sorozatának nevezzük
  A x B = {a,b| a eleme A és b eleme B}
`A = {a,b}, B = {1,2}, A x B = {(a,1),(a,2),(b,1),(b,2)}`
Speciálisan: `RxR = R^2  RxRxR = R^3`

----

## KOMPLEX SZÁMOK

### Komplex számok halmaza

- Jele **C**
- Megköveteljük, hogy:
- Az x^2 +1 = 0 egyenletnek is legyen eredménye a C halmazon: x^2 = -1
- A komplex számokkal végzett műveletekre is érvényesek legyenek azok a szabályok, mint a valós számokkal végezhető műveletekre (Osztás, szorzás elvégezhető legyen és teljesüljön a kommutatív, asszociatív és diszkriminatív tulajdonság. Valamint az a+x = b és az a*x =b (a nem 0) egyenletek megoldhatók lesznek).
- A komplex számok halmaza tartalmazza a valós számok halmazát

### definíciók

1. Az *i* = sqrtf(-1) [gyök-1] számot képzetes(Imaginary) egységnek nevezzük  i^2 = -1
2. A *z* = a+b*i számot komplex számnak nevezzük ahol a,b eleme R
3. A *z* szám valós része Re(z)=a a képzetes része Im(z)=b `z = a+b*i` a komplex számnak az algebrai alakja  Minden valós szám leírható z = a+0*i Alakban R eleme C

### Ábrázolás

1. a komplex számokat komplex számsíkon -- Gauss-féle számsíkon --  ábrázoljuk. Az x-tengelyt valós, az y-tengelyt képzetes tengelynek nevezük.
2. `z = a+b*i` a komplex számnak a sík P(a;b) pontjai vagy az OP(origo, p pont) helyvektor felel meg.

### Konjugált

 `z = a + b*i` a komplex számnak a **konjugáltján** a  z = a **-** b*i a komplex számot értjük.
 Abszolút érték
 `z = a + b*i` a komplex számnak az abszolút értékén a komplex számot ábrázoló vektor hosszát értjük
`|z| = |a+b*i|= gyök(a^2+b^2)`

### Egyenlőség

: A komplex szám algebrai alakban akkor és csak akkor egyenlő ha a valós és a képzetes része is egyenlő

### Műveletek algebrai alakban

|Művelet|alap állás| = |
|-|-|-|
|Össze adás|`Z1+Z2 = (a1 + b1 \*i) + (a2 + b2*i)`|`=(a1+a2) + (b1+b2)*i`
|Kivonás|`Z1-Z2 = (a1 + b1 *i) - (a2 + b2*i)`| `=(a1-a2) + (b1-b2)*i`
|Szorzás|`Z1*Z2 = (a1 + b1 *i) * (a2 + b2*i)`| `=(a1+a2) + (b1+b2)*i`
|Osztás|`Z1/Z2 = (a1 + b1 *i) / (a2 + b2*i)`|A nevező konjugáltjával szorzunk `=(a1+a2) + (b1+b2)*i`

### Trigonometrikus alak

- A z= a+b*i alak egyértelműen jellemezhető
- a szám 0 tól való  távolságával `r = |z| (r=>0)` és
- azzal a szögértékkel (phi)  φ amellyel a valós tengely pozitív része az adott pontba mutató `φ = arg z * a`   komplex szám komplementere `0<= φ <=π`
- `z = r(cos  φ+i sin  φ)`

### Exponenciális alak

- Euler formula `e^iφ = cos  φ + i sin  φ`
- `lnx = log e x` (logaritmus naturalis egyenlo e alapu logaritmus x)
- exp alak:`z=r * e^i φ`

### Műveletek

- összeadás kivonás algebrai alakban
- Szorzás: `z1*z2 = (r1 * e^i φ1 )* (r2 * e^i φ2) = (r1*r2) * e^i (φ1+φ2) = (r1*r2)(cos(φ1+φ2)+i sin(φ1+φ2))`
- Osztás `r =/= 0  z1/z2 =  r1* e^i φ1/r2 * e^i +φ2 =r1/r2  e^i (φ1-φ2) - r1/r2 (cos(φ1-φ2)+i sin(φ1-φ2))`

### Hatványozás

: `Legyen n e eleme R nek z^n = z*z ...*z  z= r * e^iφ = r(cosφ + isinφ)`
`z^n = (r*e^iφ)^n = r^n * e^inφ`

Legyen n eleme R+ nak  z^n = z*z*z*.....*z, | z = r e^iφ = r(cos  φ+i sin  φ) | z^n = r^n e^inφ
Abszolút értéket hatványozunk, argumentumot(? φ)

### Demoire tétele

 `(cosφ + isinφ)^n = cos(n*φ) + i*sin(n*φ)`
`z^n = r*(cosφ + i*sinφ)^n = r^n (cos(n*φ) + i*sin(n*φ))`

### Egység gyökök

 `w^n`
 `= n gyök alatt r (cos (φ+k*2*pi)/n + i *sin *(φ+k*2*pi)/n`
 `= n gyök alatt r e^i(φ+k*pi)/n`
 `w3 = 1 -> w3 = 1 cos0 + i sin0)`
 `k=0  w0 = 1*(cos (0+0*2*pi)/3 + i *sin *(0+0*2*pi)/3 = 3 gyök alatt 1 e^i(0+0*pi)/3`
 `k=1  w1 = 1*(cos (0+1*2*pi)/3 + i *sin *(0+1*2*pi)/3 = 3 gyök alatt 1 e^i(0+1*pi)/3`
 `k=2  w2 = 1*(cos (0+2*2*pi)/3 + i *sin *(0+2*2*pi)/3 = 3 gyök alatt 1 e^i(0+2*pi)/3`

w^k = k alatti gyök r [((cos)(φ*k*2pi)/n) ((sin)*i*(φ*k*2pi)/n)

## Leképezések

|-    |Egy    |Több |
|----|------|-------|
|egyértelmű|E-e|T-e |
|többértelmű|E-t|t-T|

- Ha A halmaz minden eleméhez hozzá rendelünk egy adott utasítás szerint a B halmaz vagy t b elemet, akkor az A halmaz B halmazra való leképezéséről beszélünk

Leképezések osztályozása:

- Egyértelmű: a leképezés ha A bármely egyes eleménak egyetlen B-beli képe van továbbá, ha minden egyes kép elemnek csak egy eredetje van akkor a leképezés egy értelmű.
- Az egyértelmű leképezések függvények

## Függvények

- Egyváltozós valós függvény: Legyen A és B 2 nem üres halmaz, ha az A halmaz minden eleméhez hozzá rendeljük a B halmaz pontosan 1 elemét, akkor az A halmazon értelmezett B beli értékeket felvevő függvényt kapjuk
- Df/Rf: Az A halmazt az f függvény Értelmezési Tartományának[ÉT] nevezzük Df-el jelöljük. Azokat a B beli elemeknek a halmazát, amelyeket az A beli elemekhez rendelünk, értékkészletnek nevezzük és Rf el jelöljük.
- Ha A és B halmaz elemei is valós számok akkor egyváltozós függvényről beszélünk.
- Zérus hely  Az f függvény zérushelye az értelmezési tartományának azon elemene amelyre a függvény értéke 0( Ahol a függvény metszi az X tengelyt)

### Monotonitás

- Monoton növő egy függvény ha az értelmezési tartományának bármely 2 pontára teljesül  `x1<x2, (f)x1=<(f)x2`
- Szigorúan monoton növő egy függvény ha egy függvény ha az értelmezési tartományának bármely 2 pontára teljesül `x1<x2, (f)x1<(f)x2`
- Monoton csökkenő egy függvény ha az értelmezési tartományának bármely 2 pontára teljesül`x1<x2 (f)x1>=(f)x2`
- Szigorúan monoton csökkenő egy függvény ha az értelmezési tartományának bármely 2 pontára teljesül `x1<x2, (f)x1>(f)x2`
- nem monoton

### Korlátosság

- Az f függvény felülről korlátos ha van olyan K szám amire igaz minden x eleme Df nek f(x) <= K
- Az f függvény alulról korlátos ha van olyan k szám amire igaz minden x eleme Df nek  f(x) >= k
- Egy függvény csak akkor korlátos ha felülről és alulról is korlátos. Létezik olyan k és K szám  amire igaz hogy minden x eleme Dfnek és`k<= f(x) <= K`
- Nem korlátos függvények
    1. Csak felülről
    2. Csak alulról
    3. sem felülről sem alulról nem korlátos

### Paritás

- Az f függvény amelynek az érték tartománya az origóra szimmetrikus halmaz, ha minden x eleme Dfnek f(-x) = f(x) teljesül
- Az f függvény amelynek az érték tartománya az origóra szimmetrikus halmaz, ha minden x eleme Dfnek f(x) = -f(x) teljesül
- Se nem páros se nem páratlan

### Helyi szélső érték

 Az f függvények az x0 helyen helyi vagy lokális maximum(minimum)-a van ha x0nek van olyan környezete, hogy az ebbe eső minden olyan xre ahol f értelmezett teljesül `f(x)<f(x0) [vagy  f(x>)f(`

### Konvexitás

 Az f függvény az [a,b] intervallumon alulról konvex [konkáv] ,ha bármely ívének minden pontja az ív végpontjait összekötő húr alatt [felett] van.

### Inflexiós pont

 Azt a pontot, amelyben két különböző konvexitású görbedarab csatlakozik, inflexiós pontnak nevezzük.

### Periodocitás

 Az f függvény periodikus ,ha létezik olyan p &gt; 0 valós szám ,hoghy minden x-re ,ahol f értelmezett f(x+p)=f(x) teljesül.A legkisebb ilyen p-t az f függvény periódusnak nevezzük.

### Elemi függvények osztályozása

- Algebrai függvények
 1. racionális
 2. irracionális

- Transzcen? függvények
 1. exponenciális
 2. logaritmikus
 3. trigonometrikus
 4. ciklometrikus

### Függvények leszűkitése

Legyen az A halmaz az (f) fv Értelmezési Tartományának nem üres részhalmaza az f fv A halmazra való leszűkítése alatt azt az fvt értjük amelynek az ÉTja A és értékkészlete minden x0

### Összetett fvk leképezése

### Inverz fv

Legyen az f fgv kölcsönösen egyértelmű leképezéssel létesült fgv. Az f fgv invesz fgv-én azt az f fgv-t értjük amelynek értelmezési tartómánya az f fgv értékészlete és hozzá rendelési törvény a következő ,minden y-hoz azt a x-t rendeli ,amelyből az eredeti leképezés során az az y keletkezett azaz amelyre y=f(x).

### Elemi fv

----

## Ciklometrikus fvk

Mivel minden trigonometrikus fgv több-egyértelmű leképezéssel keletkezett ezért az inverzük nem fgv. Azonban ha ezen fgv-ek mindegyikét olyan intervallumra szűkítjuk le,amelyen  kölcsönösen egyértelmű , akkor a trigonometrikus fgv-ek inverzeiőről is beszélunk.

### sin

- f(x) = sinx Dsz = [-pi/2; pi/2] ezen az intervallumon a sin x szig mon növő ebből következik hogy e-e leképezés -> létezik és véges
- Df={x| x eleme R} t-e -> nem létezik -> Dsz = [-pi/2; pi/2] -> e-e -> létezik  Rf [-1;1] y = sin x arcisn y = arcsin (sinx) = x = inverz f(y) -> inverz f(x) = y = arcsin x Df=[-1;1] Rf = [-pi/2; pi/2]
- Hozzárendelési utasítás : arcsin azt jelenti hogy a  [-pi/2; pi/2] zért intervallumba eső zárt szöget radiánban adva menyek a sinusa =x

### cos

- f(x) = cosx Dsz = [0; pi] ezen az intervallumon a cos x szig mon csökken ebből következik hogy e-e leképezés -> létezik és véges
- `Df={x| x eleme R}` t-e -> nem létezik -> Dsz = [0; pi] -> e-e -> létezik  Rf [-1;1]
- `y = cos x`
- `arcisn y = arccos (cosx)` = x = inverz f(y) -> inverz f(x) = y = arccos x Df=[-1;1] Rf = [-pi/2; pi/2]
- Hozzárendelési utasítás : arccos azt jelenti hogy a  [0; pi] zért intervallumba eső zárt szöget radiánban adva menyek a cosinusa =x

### tan

### ctg

### fv azonosság

f=g -> Df = Dg és f(x) = g(x) minden x eleme Dfnek és a hozzárendelési utasítások megegyeznek

### megadható

- egyenlettel
  1. implicit alak
  2. explicit alak
- integralvonalanként változó képlettel
- grafikonnal

### Függvény konstans szorosa

: Ha f függvény differenciálható x0ban és c tetszőleges valós szám akkor a c*f függvény is differenciálható x0ban és (c*f)'(x0)=c*f'(x0)
Bizonyítás: feltétel  (differenciahányados)=f'(x0) létezik és véges

### Függvény összege

minden x null  eleme D(f+g)  (f+g)(x0) = f(x0)+g(x0)

### Függvények szorzata

Az f és g fgv-ek szorzata az az f*g fgv amelyre D f*g = D f ∩ D g és ∀ x 0 D f*g (f*g)(x 0 )
=f(x 0 )*g(x 0 ).

### Függvények  Hányadosa

Az f és g fgv-ek hányadosán aztz az f/g fgv-t értjük amelyre D f / g = D f ∩ D g \{ x D g ;g(x 0 )=0 }
helyen (f/g)(x 0 )=f(x 0 )/g(x 0 ).

### szorzat

Az a c = f(x) ami ÉT megegyezik a f(x) étéjével  ésrtékei minden x0 elem D(c és f) helyen c*f(x)(x0) c eleme R

### 2fv összege

Minden x0 eleme D(f+g) helyen (f+g)(x0) = f(x0) + g(x0)

### polinomok

(racionális egész fgv-ek)
A Pn R → R Pn=a 0 + a 1 x + a 2 x 2 + . . . + a n x n fgv-t edfokaválós együttható polinom fgv-nek
nevezzük .a i R, i=0,1,2...n ; a n ≠0.

### 2 fv szorzata

### 2fv osztása

### racionális törtfüggvények

olyan hányados függvény amelynek a számlálója és nevezője is egy polinom függvény.

### Összetett függvény

### Inverz függvény

### Polinomok

----

## Számsorozatok

: FOGALMA: Ha ∀ pozitív egész számhoz hozzárendelünk egy-egy valós számot ,szám sorozat kapunk.

### megadási módja

: A sorozatoknak vÉgtelen sok eleme van és ezeket különféle módon adhatjuk meg.
a.A sorozatot megadhatjuk az általános elem képletével, vagyis az n változó függvényeként
felírt képlettel, formulával. (Pl a n = 2*n)
b. . A sorozatot megadhatjuk rekurzív módon. Ez azt jelenti, hogy néhány elemet megadunk,
a további elemeket pedig az előttük lévők segítségével definiáljuk.(Pl a n = a n-1 + a n-2 )

### sorozatok szemléltetése

1. Sikbeli koordinata rendszerben az ( n,a n ) pontokkal
2. Szám egyenesen csak a sorozat tagjaival.

## *Vizsgálati szempontok*

### monotonitás

- Monoton növő egy függvény ha minden an re teljesül  `an+1>=an`
- Szigorúan monoton növő egy függvény ha egy függvény ha az értelmezési tartományának bármely 2 pontára teljesül `x1<x2, (f)x1<(f)x2`
- Monoton csökkenő egy függvény ha az értelmezési tartományának bármely 2 pontára teljesül`x1<x2 (f)x1>=(f)x2`
- Szigorúan monoton csökkenő egy függvény ha az értelmezési tartományának bármely 2 pontára teljesül `x1<x2, (f)x1>(f)x2`
- nem monoton

### korlátosság

----

### Határérték

határ érték szempontjából egy sorozat két fajta lehet, Konvergens vagy divergens.

----

## Határérték(sorozatok)

### Konvergens (összetartó) sorozatok

1. Az an sorozat konvergens és határéeréke A szám ha minden epszilon sugaru környzetéből a sorozatnak csak véges számű tagja marad ki.
2. Az an sorozat konvergens és határéeréke A szám a minden epszilon kissebb mint nulla  számhoz tartozó N(epszilon) küszöbszám vagy küszöb index ha n>N(e) akkor |an-A|<epszilon teljesül Jelölés Lim n tart végtelenig dn = A !KÉP!
- Ha egy sorozat konvergens akkor korlátos. **Fordítva nem igaz!** A korlátosság a konvergencia szükséges de nem elégséges feltétele
- ha egy sorozat korlátos és monoton akkor konvergens. **Fordítva nem igaz!** A korlátosság és a monotonitás a konvergencia elégséges de nem szükséges  feltétele

### Divergens (nem konvergens sorozat)

Tágabbb értelemben van határértékük:
 \+ (pozitív) végtelenbe divergál
 \- (negatív) végtelenbe divergál

### Nevezetes határértékek

lim n-végtelen 1/n = 0
lim n-végtelen q^n 0ha |q|<1 1ha q=1  egyébként divergens -> végtelen q>1 korlátos q=-1 széttartó divergens q<-1
lim n-végtelen (1+(1/n))^n = e -> általánosan (1+(k/n)) = e^k és ő konvergens
lim n-végtelen n gyök alatt a = 1  a eleme R+

### Függvények határéerékének műveleti tulajdonságai

## konvergens sorozatok műveleti tulajdonságai

### Rendőrszabály

limn→∞
an
: ha az an sorozat konvergens és határértéke A szám a bn sorozat konvergens és határértéke a szám minden nre ihaz hogy an<=cn<=bn akkor cn sorozat is konvergens és határértéke A szám

### Egyváltozós valős függvények határértéke

### Végtelenben vett határértéke

### függvények határértékének műveleti tuzlajdonságai

### Függvények folytonossága

## Intervallumbeli folytonosság

- Az f függvény folytonos az ]a;b[ nyilt intervallumon  ha az intervallum minden pontjában folytonos
- Az f függvény folytonos a [a;b] tárt intervallumon ha az ]a;b[ nyílt intervallumon folytonos és az a helyen jobbrol a b helyen balról folytonos
- Az f fv az x0 helyen barról/jobbról folytonos ha
1. x0 helyen értelmezve van (x0 eleme Df nek)
2. x0 helyen van bal/jobboldai határértéke
3. x0 helyen a bal/jobboldalo határértéke megegyezik a helyettesítési értékkel
- Ha az f függvény Értelmezési tartományának minden pontjában folytonos akkor az f folytonos függvény
- A polinomok, racionális törtfüggvények, exponenciális, logaritmus és trigonometrikus függvények **folytonos** függgvények.

### Műveletek folytonos függvényekkel

- Ha az f és g folytonos x0 helyen akkor az f+g, f*g, f/g (ha g =/= 0) függvények is folytonosak x0 helyen
- ha a g belsőfüggvény folytonos x0ban és a külsö f függvény is folytonos a g(x0) ban  akkor f(x) kör g folytonos x0 ban.
- Ha fx egy-egy értelmű függvény folytonos x0ban akkor F(y) inverz függvény is folytonos az y0 helyen

## Deriválás

### **Az érintő**

- Egy görbe P0 pontbeli érintője az  e egyenes, ha minden p0 hoz konvergáló Pn pontsorozathoz tartozó P0Pn szelősorozat határhelyzete ugyan az az e egyenes.
- Ha az f függvény Értelmezési tartományának minden pontjában differenciálható akkor az f függvényt differenciálható vagy deriválható függvénynek nevezzük.
- az f függvény differenciálható ]a;b[ nyílt intervallumon ha au intervallum minden pontján differenciálható.

### differencia hányados

### differenciál hányados

### derivált

### differenciálhatóság és folytonosság kapcsolata

----

## Differenciálhatóság műveleti tulajdonságai

### c*f

### f+g

### f*g

### f/g

### fkörg

### inverz

----

### elemi függvények deriválta

### algebrai

### logaritmikus

### trigonometrikus

## Magasabb rendű deriváltak

### differenciálszámítás azonosságai

### érintő egyenlete

### L'hospital[LOPITÁL] szabály

----

## Függvény vizsgálat

### fv menetének vizsgálata derivált segítségével

### szélsőérték és derivált kapcsolata

Ha az ]a;b[ intervallumon differenciálható f függvénynek szélsőértéke van -> f'(x0)=0
Geometriai jelentése

### szélsőérték

Szélsőérték létezésének elégséges feltétele

- Az x0 helyen és és annak valamely környezetében differenciálható f függgvénynek az x0 helyen akkor van szélsőértéke ha f'(x0)=0 és az f függgvény az x0 helyen előjelet változó
 1. Ha f'(x0)=0 és az f' függgvény x0 helyen + -> - helyi maximuma van
 2. Ha f'(x0)=0 és az f' függgvény x0 helyen - -> + helyi minimuma van
- Az x0 helyen és és annak valamely környezetében kétszer differenciálható f'(x0) = 0 és f''(x0) = 0 akkor az f függgvény az x0 helyen lokális szélsőértéke van
 1. Ha f'(x0)=0 és az f''(x0)<0  helyi maximuma van
 2. Ha f'(x0)=0 és az f''(x0)<0  helyi  minimuma van
- Az f'(x0)=0 szükséges de nem elégséges feltétele hogy az ]a;b[ intervallumon differenciálható f függgvénynek az x0 eleme ]a;b[ helyen szélsőértéke van
