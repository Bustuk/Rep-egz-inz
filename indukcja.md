---
# try also 'default' to start simple
theme: default
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: /background.jpg
# apply any windi css classes to the current slide
class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
# some information about the slides, markdown enabled
info: |
  ## Prezentacja na 
  Repetytorium do Egzaminu Dyplomowego
  1. Indukcja Matematyczna
# persist drawings in exports and build
drawings:
  persist: false
download: true
---

# Indukcja Matematyczna

---

# Czym jest indukcja?

1. w logice: wyprowadzanie wniosków ogólnych z przesłanek będących poszczególnymi przypadkami tych wniosków
2. w naukach empirycznych: metoda badawcza prowadząca do uogólnień na podstawie eksperymentów i obserwacji faktów
3. wzbudzenie prądu lub ładunku elektrycznego pod wpływem czynników elektrycznych lub magnetycznych

---

# Indukcja matematyczna

 -  Indukcja zupełna - jeśli wykorzystane w
rozumowaniu indukcyjnym zdania szczegółowe
wyczerpują wszystkie przypadki spełnienia zdania
ogólnego, będącego wnioskiem tego rozumowania
 -  Indukcja niezupełna - jeśli wykorzystane w
rozumowaniu indukcyjnym zdania szczegółowe nie
wyczerpują wszystkich przypadków 
---

# Twierdzenie
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


Mam posortowany rząd elementów.

Wiem że cos się dzieje dla pierwszego elementu

Wiem że element kolejny zachowuje się tak samo jak element poprzedni

Stąd wiem że dane zachowanie występuje dla każdego elementu


---

# Przeprowadzanie dowodów indukcyjnych

1. Określa się najmniejszą liczbę naturalną $n_0$, dla której twierdzenie ma być prawdziwe, a następnie
sprawdza się, czy rzeczywiście dane twierdzenie jest prawdziwe dla $n_0$ (metodą podstawienia liczby$n_0$  w miejsce zmiennej $n$ w twierdzeniu).
2. Krok indukcyjny
    1. Zakłada się, że twierdzenie jest prawdziwe dla ustalonego $n$ (jest to tzw. założenie 
    indukcyjne).
    2. Dowodzi się, że twierdzenie jest prawdziwe dla następnej liczby naturalnej tzn. dla $n+1$. (Dowodzimy implikacji $T(n)=>T(n+1)$, Założenie indukcyjne implikuje Tezę indukcyjną)
3. Na mocy indukcji matematycznej wnosi się, że twierdzenie jest prawdziwe dla każdej liczby 
naturalnej $n>n_0$


#### Ważne! W kroku 2.1 Nie zakładamy że dla dowolnego $n$ zachodzi twierdzenie - popularny błąd!
---

### Udowodnić, że dla każdej liczby naturalnej $n>=0$ i dowolnego $a>-1$ spełniona jest nierówność $(1+a)^n >= 1+na$ (Nierówność Bernoulliego)

1. Dla $n=0$ otrzymujemy $(1+a)^0 = 1 >= 1 + 0 \cdot a$ więc nierówność jest prawdziwa

2. Niech k będzie taką liczbą naturalną, że prawdziwa jest nierówność $(1+a)^k >= 1+ka$. (założenie indukcyjne) Udowodnimy, że zachodzi
$(1+a)^{k+1} >= 1+(k+1)a$ (teza indukcyjna)

Oznaczmy L =  $(1+a)^{k+1}$ i P = $1+ka+a$. 

Przekształćmy równoważnie:
$$
\begin{array}{c}
L = (1+a)^{k+1} = (1+a)^k \cdot (1+a) >= (1+ka) \cdot (1+a) \\
= 1 + a +ka + ka^2 >= 1+a+ka = P 
\end{array}
$$
3. Na mocy zasady indukcji matematycznej nierówność Beroulliego jest prawdziwa.
---

### Udowodnić, że dla każdej liczby naturalnej $n>=3$ spełniona jest nierówność $2^n>2n$

Nierówność jest tu formą zdaniową $T(n), n0 = 3$.

1. Dla $n = 3$ nierówność jest prawdziwa, ponieważ $2^3 = 8 > 2 \cdot 3 = 6$. $T(3)$ jest więc zdaniem prawdziwym.

2. Niech k będzie taką liczbą naturalną, że prawdziwa jest nierówność $2^k > 2k$. (założenie indukcyjne)
Udowodnimy, że zachodzi $2^{k+1} > 2(k+1)$ (teza indukcyjna) 

---

Przekształćmy równoważnie:
$$
\begin{array}{c}
2^k > 2k \\
2 \cdot 2^k > 2 \cdot 2k \\
2 ^{k+1} > 2k + 2k \\
L = 2 ^{k+1}, P = 2k + 2k \\
P = 2k +2k > 2k + 2 = 2(k+1) \\
L > P \\
2 ^{k+1} > 2(k+1)
\end{array}
$$

3. Na mocy zasady indukcji matematycznej dla każdej liczby naturalnej $n>=3$ spełniona jest nierówność $2^n>2n$
---

# Inne zastosowania indukcji

### Indukcji matematycznej można używać również przy innych rodzajach dowodów, np w dowodach geometrycznych
<br>

 - <a href="http://www.math.uni.wroc.pl/~newelski/dydaktyka/wdm-A/skrypt2/skrypt/node14.html">N-kąt wpisany w okrąg ma $n(n−3)/2$ przekątnych.</a>
 - <a href="https://brain.fuw.edu.pl/edu/index.php/Indukcja_matematyczna">Wzór dwumienny Newtona</a>
 - <a href="https://edu.pjwstk.edu.pl/wyklady/mad/scb/mad09/main09_p4.html">Definicja ciągu Fibonacciego</a>
---

# Źródła  

 - http://www.math.uni.wroc.pl/~preisner/dyd/2016_3lo/files/3LO_lista03.pdf
 - http://www.math.us.edu.pl/~pgladki/faq/node67.html
 - https://edu.pjwstk.edu.pl/wyklady/mad/scb/mad09/main09_p4.html

Łukasz Wołodkiewicz WMiI UŁ
