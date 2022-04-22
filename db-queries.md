---
# try also 'default' to start simple
theme: default
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
# background: /background.jpg
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

# Rodzaje kwerend w relacyjnych bazach danych

---
layout: two-cols
---

# Baza Danych a System Zarządzania Bazą Danych

To co potocznie nazywamy bazami danych to tak naprawdę Systemy Zarządzania Bazami Danych, np mySQl, Oracle, PostgreSQL

Zawiera on m.in.
- środki zapewniające integralność i bezpieczeństwo danych,
- dostęp do danych poprzez język zapytań bazy danych np. SQL,
- środki do zarządzania danymi,
- środki optymalizujące czas dostępu do danych, np. indeksy,


::right::

<img width=400 src="/dbms.png"/>

---
layout: two-cols
---

# Elementy budowy SZBD Microsoft Access

Obiekty budujące bazę danych to:
 - Tabele
 - Kwerendy
 - Raporty
 - Formularze
 - Makra
 - Moduły

::right::

<img width=400 src="/access.png"/>

---

# Definicja kwerendy

<br>

## Kwerenda jest zapytaniem (żądaniem) skierowanym do obiektu bazy danych.
<br>
<br>

 - umożliwia dostęp do danych w jednej lub wielu tabelach
 - pozwala na wybieranie i przetwarzanie danych: obliczenia, sortowanie, filtrowanie
 - pozwala na modyfikacje i usuwanie danych z tabel
 - pozwala modyfikować strukturę bazy danych
 - umożliwia łączenie wyników z wielu tabel

---

# Rodzaje kwerend w Microsft Access

 - Kwerendy wybierające
 - Kwerendy krzyżowe
 - Kwerendy funkcjonalne
   - Aktualizujące
   - Dołączające
   - Usuwające
   - Tworzące tabele
 
---

# Kwerendy wybierające

Najczęściej używany rodzaj kwerendy, umożliwiają wybieranie rekordów,
tworzenie nowych pól obliczeniowych i podsumowywanie danych. Kwerendy tego typu
są podobne do filtrów, jednak umożliwiają również:
 - Przeprowadzanie zapytań w więcej niż jednej tabeli
 - Tworzenie nowych pól obliczeniowych
 - Podsumowywanie i grupowanie danych
 - Wyznaczanie pól do ukrycia lub pokazania

<br>

# Kwerendy krzyżowe

Umożliwiają wybieranie rekordów, tworzenie nowych pól obliczeniowych i podsumowywanie danych
z różnych tabel. Niektórzy traktują ją jako podtyp kwerendy wybierającej.

---
layout: section
---

# Kwerendy funkcjonalne

---

# Kwerenda aktualizaująca
Dokonuje globalnych zmian w grupie rekordów w tabeli lub kilku tabelach. Za pomocą kwerend aktualizujących można zmienić dane w istniejacych tabelach.

# Kwerenda usuwająca 
Usuwa grupę rekordów z jednej lub kilku tabel. Użycie kwerendy usuwającej powoduje usunięcie całych rekordów, nie zaś wybranych pól w rekordach.

# Kwerenda dołączająca
Dodaje grupę rekordów z tabeli lub tabel na końcu innej tabeli lub tabel. Kwerendy dołaczające są również przydatne w następujących sytuacjach:
 - dołączanie pól wybranych na podstawie kryteriów;
 - dołączanie rekordów w sytuacjach, gdy część pól jednej tabeli nie ma swoich odpowiedników w drugiej tabeli.

---

# Kwerenda tworząca tabele
Tworzy nowa tabelę z wszystkich lub części danych znajdujących się w jednej lub kilku tabelach. Kwerendy tworzące tabelę są przydatne w następujacych sytuacjach:

 - tworzenie tabel, które maja być eksportowane do innych baz danych programu Microsoft Access;
 - tworzenie raportów zawierających dane od określonego momentu;
 - tworzenie kopii zapisowej tabeli;
 - tworzenie tabeli archiwalnej, zawierającej nieaktualne rekordy;
 - poprawianie sprawności działania formularzy i raportów utworzonych na podstawie kwerend korzystających z danych z wielu tabel lub instrukcji SQL

---

# Źródła  

 - https://www.bmc.com/blogs/dbms-database-management-systems/
 - http://www.math.us.edu.pl/~pgladki/faq/node67.html
 - https://edu.pjwstk.edu.pl/wyklady/mad/scb/mad09/main09_p4.html
 - https://krystianbrozek.pl/rodzaje-kwerend-w-accessie/
 - http://pwszjardefence.wikidot.com/1-wyja-nij-co-to-jest-kwerenda-i-podaj-ich-rodzaje

Łukasz Wołodkiewicz WMiI UŁ
