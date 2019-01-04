# Analízis

- Feladatok
  - Feladat leírás
  - Használt formula és szabályok
  - Megoldás lépések
  - Megjegyzések
- Segítségek
  - Matek : [Mateking](https://www.mateking.hu) jó forrás gyakorláshoz
    - [Differenciálhatóság (Mateking)](https://www.mateking.hu/system/files/docs/differencialhatosag.pdf)
  - Dokumentum
    - [Katex syntax](https://khan.github.io/KaTeX/function-support.html)
    - [MarkDown syntax](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
- Egyéb
  - Használt program és extension: Visual Studio Code
    - markdownlint  0.18.0 (stílus figyelő plugin hogy ne legyen kankeres a dokumentum annyira)
    - Markdown+Math 2.2.1 (Katex plugin)
  - Készítette: vrka

## Trükkök

1. $\dfrac{1}{x} = x^{-1}$
2. $\sqrt {x} = x^{\frac{1}{2}}$

## Szabályok

1. Logaritmus cucc
    - $log_a b = c$ ami nem más mint $b = c^a$
2. trignonmertikus izé
    - $sin 0 = 0$ és `cos 0 = 1`
3. deriválás
    - Lánc szabály
        - $(f\circ g)'(x_0) = (f'\circ  g)\cdot g' = f'g(x_0) \cdot g'(x_0)$
        - $(f\circ g \circ h)'(x_0) =(f'\circ g\circ h)\cdot(g'\circ h)\cdot'h= (f'gh)(x_0)\cdot(g'h)(x_0)\cdot'h(x_0)$
4. monotonitás
   - $a_{n+1} - a_n$ Egyszerű ~$\frac {n+1}{n-1}$ alakúnál lehet használni

## Feladatok

1. Határozza meg az $f= \dfrac{2}{x}$ függvény $x_0=2$ helyhez tartozó érintőjének egyenletét. Készítsen ábrát!
    - Az érintő egyenlete $y=f'(x_0)\cdot(x-x_0)+f(x_0)$ ebbe kell behelyettesíteni és a végén megkapjuk az érintő függvényét.
        1. Behelyettesítünk $x_0$ helyébe $y= f'(x_0)\cdot(x-2)+f(2)$ ebből az $f(2)$ ből pedig $\dfrac {2}{2}$ lesz
        2. Lépésben lederiváljuk a kifejezést $f'(x0)= \dfrac{2}{x} = -2 \dfrac{1}{\red x^2}$ majd ebbe $\red {behelyettesítünk}$ a következő módon az x helyére és egyszerűsítjük $-2 \dfrac{1}{\red2^2}= -\dfrac{2}{4} = -\dfrac{1}{2}$
        3. Utolsó lépésben vissza rakjuk a deriváltat oda ahol volt és megkapjuk az érintő egyenletét$\blue c(\textcolor{lime} x +\red a)+ \green b$ formátumban a következő képpen $-\blue{\dfrac{1}{2}}(\textcolor{lime} x-\red 2)+\green 2$
    - Függvény ábrázolási szabályok $\blue c(\textcolor{lime} x +\red a)+ \green b$
        1. $\red a$ x tengelyen mozgatás ellentétes irányban
        2. $\green b$ y tengelyen való mozgatás
        3. $\blue c$ nyújtás/laposítás
        4. Előjel váltás
            - $-\blue c$ invertálás y tengelyen (pl jelen esetben a x/2 fv alapból / lenne de megfordul \ irányban)
            - $-\textcolor{lime} x$ invertálás x tengelyen
    - A fenti szabályok segítségével fel kell rajzolni az alapfüggvényt (amit behelyettesítünk) majd rá az érintőt.
2. Határozza meg az $f(x)=x\cdot e^x$ függvény monotonitási intervallumait és szélsőértékeit!
    - [A példa monotonitási intervalluma](https://www.youtube.com/watch?v=7cwN7Os8tf4) egy másfajta [megoldás](https://www.youtube.com/watch?v=xaLubQigeiA&t=577s)
    - A monotonitás és szélsőértékekre segítség a megoldáshoz [itt](https://www.mateking.hu/analizis-1/fuggvenyvizsgalat-gazdasagi-feladatok/a-fuggvenyvizsgalat-lepesei)
    
3. Számítsa ki a következő határértékeket:
    - Figyelni kell mert lehet $\dfrac {0}{0}$ vagy $\dfrac{\infty}{\infty}$ alakú határ érték aminél mindenképpen a L'Hospital szabályt kell alkalmazni.
    - [Online határérték kalkulátor](https://www.symbolab.com/solver/limit-calculator/)
        - $\lim _{x\to -1\:}\left(\frac{3x-1}{x^2+2x+1}\right)$ \lim _{x\to -1\:}\left(\frac{3x-1}{x^2+2x+1}\right)
        - $\lim _{x\to 2}\left(3x+4\right)^4$ \lim _{x\to 2}\left(3x+4\right)^4
        - .
4. Deriválja az alábbi függvényeket:
    - [Derivált kalkulátor](https://www.derivative-calculator.net/)
        - (5log_3 x- root(3,x))/3^x
        - 3/root(3,x)-5/root(5,x^3)
        - (3+2x^2)^10
        - ((3x^3-4)/(2x^2+2x))^2
        - 3/x^(1/3)
    - s
