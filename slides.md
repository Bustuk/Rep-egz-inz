---
# try also 'default' to start simple
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://source.unsplash.com/collection/94734566/1920x1080
# apply any windi css classes to the current slide
class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
# some information about the slides, markdown enabled
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# persist drawings in exports and build
drawings:
  persist: false
download: true
---

# Indukcja Matematyczna

Presentation slides for developers

---

# Czym jest indukcja matematyczna?

 - ## Indukcja niezupełna
 - ## Indukcja zupełna
---

# Definicja
Zasada indukcji matematycznej

<br>

#### Niech $T(n)$ oznacza formę zdaniową zmiennej n określoną w dziedzinie $N$

Jeżeli:
1. istnieje taka liczba naturalna $n_0$. że $T(n_0)$ jest zdaniem prawdziwym
2. dla każdej liczby naturalnej $n >= n_0$ prawdziwa jest implikacja $T(n) => T(n+1)$

to $T(n)$ jest zdaniem prawdziwym dla każdej liczby naturalnej $n => n_0$.


---

# Definicja 
na chłopski rozum 

<br>

Mam posortowany rząd elementów.

Wiem że cos się dzieje dla pierwszego elementu

Wiem że element kolejny zachowuje się tak samo jak element poprzedni

Stąd wiem że dane zachowanie występuje dla każdego elementu


---

# Przykład
Udowodnić, że dla każdej liczby naturalnej $n>=3$ spełniona jest nierówność
$2^n>2n$

Nierówność jest tu formą zdaniową $T(n), n0 = 3$.

1. Dla $n = 3$ nierówność jest prawdziwa, ponieważ $23 = 8 > 2 \cdot 3 = 6$. $T(3)$ jest więc zdaniem prawdziwym.

2. Załóżmy, że nierówność jest prawdziwa dla liczby naturalnej $n >= 3$. Mnożąc tę nierówność obustronnie przez 2 dostajemy $2 \cdot 2n > 2 \cdot 2n$, czyli $2n+1 > 2n + 2n$. Ponieważ dla każdego $n => 3$ mamy $2n > 2$, więc $2n + 2n > 2n + 2 = 2(n + 1)$. Stąd ostatecznie

$2^{n+1} > 2(n + 1)$.

---

# LaTeX

LaTeX is supported out-of-box powered by [KaTeX](https://katex.org/).

<br>

Inline $\sqrt{3x-1}+(1+x)^2$

Block
$$
\begin{array}{c}

\nabla \times \vec{\mathbf{B}} -\, \frac1c\, \frac{\partial\vec{\mathbf{E}}}{\partial t} &
= \frac{4\pi}{c}\vec{\mathbf{j}}    \nabla \cdot \vec{\mathbf{E}} & = 4 \pi \rho \\

\nabla \times \vec{\mathbf{E}}\, +\, \frac1c\, \frac{\partial\vec{\mathbf{B}}}{\partial t} & = \vec{\mathbf{0}} \\

\nabla \cdot \vec{\mathbf{B}} & = 0

\end{array}
$$

<br>

[Learn more](https://sli.dev/guide/syntax#latex)

---

# Źródła

 - http://www.math.uni.wroc.pl/~preisner/dyd/2016_3lo/files/3LO_lista03.pdf
 - http://www.math.us.edu.pl/~pgladki/faq/node67.html

Łukasz Wołodkiewicz

