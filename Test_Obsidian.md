
---
# Opis po polsku kilku podstawowych znaków formatujących w plikach *.md

---

Ogólnie jest proto. Jeden słowa są **bold** inne słowa *italic* w pliku. Można też wprowadzić [link to Google!](http://google.com) prawdziwy i działający!
##Nagłówki

---

# To jest nagłówek h1
## To jest nagłówek h2
###### To jest nagłówek h6

---
## Format textu

---
*Ten text będzie italic*
_Ten text także będzie italic_

**Ten text będzie bold**
__Ten text także będzie bold__

_Możesz też **kombinować** z nimi_

---
## Listy
---

### Nieuporządkowane
* Element 1
* Element 2
  * Element 2a
  * Element 2b
---
### Uporządkowane
1. Element 1
    1. Element 1a
        1. Element 1a1
        1. Element 1a2
    1. Elemnt 2b
1. Element 2
1. Element 3
   1. Element 3a
   1. Element 3b
1. Element 4
---
## Obrazy
![GitHub Logo](./images/T.png)
Format:![Alt Text](https://cdn.pixabay.com/photo/2016/07/02/16/36/pictogram-boxing-1493254_960_720.png)

---
## Linki
http://github.com - bezpośredni!
[GitHub-pośrdeni](http://github.com)

[Link do innego pliku md](MarkFiles/test.md)

[Drzewo Dokumenty](MarkFiles/tree.md)

[Drzewo TXT](MarkFiles/tree1.txt)

---

## Bloki

Jak powiedział Natanek:

> Jeśli na głowie jawi się żel
> to wiedz że ktoś się toba intesuje

---

## Kod w linii

Myżlę że powinieneś użyć
`<jakiś adres>` tego elementu zamiast.

---

## Podświetlanie kodu

```javascript
function fancyAlert(arg) {
  if(arg) {
    $.facebox({div:'#foo'})
  }
}
```
lub inaczej - 4 spacje przed -  nie działa:
    function fancyAlert(arg) {
      if(arg) {
        $.facebox({div:'#foo'})
      }
    }

Przykład Pythona
```python
def foo():
    if not bar:
        return True
```
CPP
```cpp
for (i=0, i<10, i++)
    {
        k:=4;
        k++;
    };
```
Ruby
```ruby
require 'redcarpet'
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html
```
Można zobaczyć wspierane na GitHubie języki [Tutaj](https://github.com/github/linguist/blob/master/lib/linguist/languages.yml)

---
## Lista zadań
- [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> supported
- [x] składnia wymaga jakijkolwiek listy (nie lub uporządkowanej)
- [x] to jest wykonany element
- [ ] to jest element niewykonany
- [ ] \(Optional)

---
## Emoji

@toma :+1: kody  :smile: :weary:
[lista Emoji do wklejenia](http://emoji-cheat-sheet.com/)

---
## Tabele

Pierwsz kolumna | Druga kolumna
-|-
coś 1| coś 2
coś 3| coś 4
### Wyrównanie

| Left-aligned | Center-aligned | Right-aligned |
| :---         |     :---:      |          ---: |
| git status   | git status     | git status    |
| git diff     | git diff       | git diff      |
### Znaki specjalne
| Nazwa     | Znak |
| ---      | ---       |
| Backtick | `         |
| Pipe     | \|        |

---
## Przekreślenie

~~jakieś~~

---
## Równania matematyczne
$\text{S}_1(N) = \sum_{p=1}^N \text{E}(p)$

$\int_{n=1}^{\infty}P\left ( x^{n} \right ) \text{dx}$

$\lim_{x\to\infty}4x^{a-1}$

$\mathcal{W}(A,f) = (T,\bar{f})$

$\inference{ \Gamma \vdash x_0 : T_0 \enspace \Gamma \vdash x_1 : T_1 \thinspace ... \thinspace \Gamma \vdash x_n : T_n \enspace \Gamma \vdash x_n : T_{n+1} \enspace }{ \Gamma \vdash {\bf match} \enspace x_0 : T_0 \enspace : \sqcap _{1\geq n \geq x+1} T_n }[MatchExpression]$

Fajny edytor internetowy jak by się zapmniało [Tutaj](https://www.codecogs.com/latex/eqneditor.php)

---
##Wzory chemiczne
$$v=u+at$$
H2O  $$\ce{H2O}$$

Ca2+(aq)+2OH−(aq)↽−−⇀Ca(OH)2(s) $\ce{Ca^2+(aq) + 2 OH-(aq) <=> Ca(OH)2(s)}$

A−→−−−catalystB $\ce{A ->[catalyst] B}$
3.4×10−8 $\pu{3.4E-8}$
8.314 JK−1mol−1 $\pu{8.314 J K-1 mol-1}$
Keq $K_\mathrm{eq}$
pKa $\mathrm{p}K_\mathrm{a}$
ΔrG∘ $\Delta_\mathrm{r} G^\circ$
E=E∘−RTzFlnQ $\displaystyle{E = E^\circ - \frac{R T}{z F} \ln{Q}}$

(2367) $\displaystyle{\left(\frac{\frac{2}{3}}{\frac{6}{7}}\right)}$

KMn+7O4 $\ce{K\overset{+7}{Mn}O4}$

(∂U∂T)V=CV $\left(\frac{\partial U}{\partial T}\right)_V = C_{V}$

(∂U∂T)V=CV $\displaystyle{\left(\frac{\partial U}{\partial T}\right)_V} = C_{V}$ 

(∂U∂T)V=CV
$$\left(\frac{\partial U}{\partial T}\right)_V = C_{V}$$

MathJax ma format \\ce{..}
$$\ce{HCl}$$
$$\ce{H2O + HCl <=> H3O+ + Cl-}$$

Expression|Markup (without $...$)|Symbol Meaning
-|-|-
$a=b$|a = b|equal
$a\ne b$|a \ne b|a is not equal to b
$a \overset{\wedge}{=}b$|a \overset{\wedge}{=}b|corresponds to
$a \approx b$|a \approx b|approximately equal
$a \simeq b$|a \simeq b|asymptotically equal
$a \sim b$|a \sim b| proportional
$a \propto b$|a \propto b| proportional(Alternate)
$a \lt b$|a \lt b|less than
$b \gt a$|b \gt a|greater than
$a \leqslant b$|a \leqslant b| less than or equal
$a \leq $|a \leq b|less than or equal(Alternate)
$b \geqslant $|b \geqslant a|greater than or equal
$b \geq a$|b \geq a| greater than or equal(Alternate)
$a \ll b$|a \ll b|much less than
$b\gg a$|b\gg a|much greater than
$\infty$|\infty|infinity symbol
$\pi$|\pi|π Symbol


---
# <center>KONIEC DOKUMENTU</center>
---