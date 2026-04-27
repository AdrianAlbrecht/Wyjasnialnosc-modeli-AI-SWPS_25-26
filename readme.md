# Wyjaśnialność modeli w uczeniu maszynowym, semestr 2026L

## 1. Cel i zakres przedmiotu

Celem przedmiotu jest przybliżenie osobie studenckiej zagadnień związanych z **wyjaśnialnością modeli w uczeniu maszynowym (Explainable Artificial Intelligence – XAI)**. W trakcie zajęć główny nacisk zostanie położony na zrozumienie, w jaki sposób modele podejmują decyzje oraz jak można interpretować ich działanie zarówno na poziomie globalnym (całego modelu), jak i lokalnym (pojedynczej predykcji). Zajęcia będą prowadzone z wykorzystaniem języka **Python** oraz popularnych bibliotek do uczenia maszynowego i analizy wyjaśnień modeli.

W trakcie zajęć osoba studencka pozna m.in. zagadnienia takie jak:

* podstawowe pojęcia związane z wyjaśnialnością modeli (XAI), motywacje stosowania wyjaśnień oraz przykłady ich zastosowań w praktyce
* przygotowanie danych oraz budowę podstawowych modeli uczenia maszynowego w Pythonie z wykorzystaniem biblioteki **scikit-learn**
* tworzenie pipeline’ów, dobór metryk oceny modeli oraz stosowanie walidacji krzyżowej
* interpretowalne „z natury” modele uczenia maszynowego (np. regresja logistyczna, drzewa decyzyjne) oraz interpretację współczynników i reguł decyzyjnych
* globalne metody wyjaśniania modeli typu post-hoc, w tym analizę ważności cech (permutation feature importance) oraz wykresy zależności PDP i ICE
* wykorzystanie narzędzi do analizy wyjaśnień modeli, w tym biblioteki **DALEX**
* lokalne metody wyjaśniania predykcji, w szczególności metodę **LIME**, wraz z analizą stabilności wyjaśnień i wpływu losowości
* metodę **SHAP** – podstawy teoretyczne oraz praktyczne zastosowanie dla modeli liniowych i drzewiastych
* interpretację wizualizacji i wykresów wykorzystywanych w analizie wyjaśnień modeli
* ocenę jakości wyjaśnień modeli (m.in. sanity checks, spójność wyjaśnień) oraz sposoby komunikowania wyników interesariuszom
* elementy podejścia **human-centered XAI**, uwzględniającego potrzeby użytkowników końcowych
* przegląd dodatkowych narzędzi i metod wyjaśniania modeli, takich jak **Anchor** czy **ELI5**.


## 2. Oprogramowanie

W trakcie zajęć do pracy niezbędne będzie posiadanie:
* zainstalowanego interpretera **Pythona** w wersji 3.10 lub nowszej
* narzędzie IDE, preferowane **Visual Studio Code**, ale zachęcam do używania również **PyCharm Professional** (licencja studencka) lub wersja Community. Może to być również inne oprogramowanie ze wsparciem dla języka Python. Na zajęciach prowadzący będzie używał **Visual Studio Code**.
* narzędzie Git do zarządzania kodem projektu (nie jest to obligatoryjne)
* możliwe, że w zależności od konfiguracji projektu niezbędne będzie zainstalowanie i konfiguracja odpowiednich pakietów czy bibliotek do języka python, natomiast będzie to zaznaczane odpowiednio na konketnych zajęciach

## 3. Warunki zaliczenia przedmiotu.

- Efektem finalnym pracy na zajęciach będzie **projekt** stworzony w języku python, który będzie analizą krytyczną jakości wytrenowanych modeli w kontekście wyjaśnialności decyzji tych modeli,
- Osoby studenckie wykonują ten projekt **samodzielnie** - nie przewiduję możliowści prac grupowych,
- Oceniane będą:
   - Jakość kodu programistycznego (brak kodu spaghetti),
   - Implementacja zagadnień przedstawionych na zajęciach,
   - Poziom skomplikowania projektu według wymagań (np. ilość modeli, działanie modeli, itp.)
   - Sens i jakość wniosków oraz wyknanych kroków
- W przypadku braku projektu nie ma możliwości alternatywnego zaliczenia przedmiotu.

## 4. Praca samozielna

Każda osoba studencka musi pracować samodzielnie. Zachęcam jednak do wspomagania się narzędziami sztucznej inteligencji, jednakowoż zabiegam o sprawiedliwość - każde użycie sztucznej inteligencji powinno być zaznaczone i opisane: co zostało zrobione samemu, co zrobiło AI, jaki zakres, prompt, krytyczna ocena, itd. Oceniana będzie całość projektu natomiast z naciskiem na część pracy wykonanej przez osobę studencką. Znajomość swojego projektu i umiejętność poruszania się w nim jest **_obligatoryjnym warunkiem zaliczenia przemdiotu_** - w przypadku, gdy student nawet nie wie co się dzieje w jego pracy, praca uznana jest za niesamodzielną, a punkty są zerowane bez możliwości poprawy. 

Wszystko jest dla ludzi, ale z rozwagą :)

## 5. Zakres materiału
1. Wprowadzenie do XAI – pojęcia, motywacja, przykłady z praktyki.
2. Dane i modele bazowe w Python (scikit‑learn): pipeline, metryki, walidacja krzyżowa.
3. Interpretowalność modeli „z natury” (logistic regression, drzewo): współczynniki, reguły, ograniczenia.
4. Wyjaśnienia globalne post‑hoc: ważność cech (permutation), PDP/ICE; wprowadzenie do DALEX.
5. Wyjaśnienia lokalne: LIME - interpretacja jednostkowych decyzji, analiza stabilności i wpływu losowości.
6. SHAP - teoria w pigułce i praktyka (drzewa i modele liniowe), interpretacja wykresów.
7. Ocena jakości wyjaśnień: sanity checks, spójność, komunikacja dla interesariuszy; elementy human‑centered XAI.
8. Anchor/ELI5 - przegląd.

## 6. Harmonogram zajęć (może ulec zmianie) _**zmiany**_
1. 12.03:
    - SYLABUS, sprawy organizacyjne + Wprowadzenie do XAI.
    - Dane i modele bazowe w Python (scikit‑learn).
2. 26.03:
    - Interpretowalność modeli „z natury” (logistic regression, drzewo)
    - Wyjaśnienia globalne post‑hoc
3. 09.04:
    - Wyjaśnienia lokalne
    - SHAP
4. 30.04: _**zmiany**_
    - Ocena jakości wyjaśnień
    - Anchor/ELI5
5. 07.05: _**zmiany**_
    - Praca nad projektami
    - Przegląd narzędzi AI
    - sprawdzian pisemny (do ustalenia termnin zamienny, w razie potrzeby) _**zmiany**_
6. 21.05:
    - Prezentacja projektów + obrona (na obu zajęciach).
    - Wystawienie ocen (punktów) za warsztaty.


## 7. Obecność i punktacja
Na zajęciach sprawdzana będzie obecność. Dopuszczone są 2 nieobecności nieusprawiedliwione.
Każda nieobecność nadmiarowa musi być nadrobiona krótką (maksymalnie 2 strony A4) teoretyczną pracą pisemną na wybrany temat, kóry był przerabiany w dniu nadrabianej nieobecności (nie chcę widzieć "copy - paste" z Gemini czy innych chatów - też potrafię napisać i poczytać :) ).

Aby zaliczyć zajęcia warsztatowe należy:
- stworzyć projekt (max: 40 pkt, na zaliczenie 20 pkt)
- obronić ten projekt (max: 20 pkt, na zaliczenie 10 pkt)
- napisać sprawdzian pisemny (teoria, max: 40 pkt, na zaliczenie 21 pkt)

Punktacja:
- Projekt:
    - dobranie i opis zbioru danych do odpowiedniego problemu (2 pkt)
    - preprocessing i przygotowanie danych do uczenia (3 pkt)
    - przygotowanie i trenowanie modeli AI - min. 3 różne modele, w tym tylko jeden "z natury wyjaśnialny" (5 pkt)
    - ocena jakości modeli (5 pkt)
    - próba wyjaśnialności modeli i ich interpretacja poznanymi metodami (15 pkt)
    - wnioski (5 pkt)
- Obrona:
    - znajomość swojego projektu (obligatoryjny warunek zaliczenia)
    - odpowiedź na 4 pytania doyczące projektu, np. dlaczego została wkorzystana dana metoda (każde pytanie maksymalnie 5 pkt, sumarycznie 20 pkt)


> # WAŻNA INFORMACJA - PRZYPOMNIENIE!
> **Projekt zaliczeniowy, to zaliczenie przedmiotu!**
>
>Zgodnie z [REGULAMINEM STUDIÓW W SWPS UNIWERSYTECIE HUMANISTYCZNOSPOŁECZNYM](https://bip.swps.pl/attachments/1020/download) §6 pkt 2 ppkt 4) i ppkt 6) student ma obowiązek do _"**poszanowania praw własności intelektualnej** i dóbr osobistych osób trzecich, w szczególności majątkowych i osobistych praw autorskich oraz przestrzegania uczelnianych przepisów dotyczących praw własności intelektualnej"_ oraz  _"rzetelnego, terminowego i **samodzielnego** wykonywania zadań nałożonych przez osoby prowadzące zajęcia, a wynikających z realizowanego programu studiów oraz decyzji organów i osób działających w imieniu Uczelni w zakresie organizacji studiów"_, co jednoznacznie odnosi się do samodzielności wykonania m.in. prac zaliczeniowych.
>
> Przypominam również, że zgodnie z §8  _"Student podlega odpowiedzialności dyscyplinarnej za naruszenie przepisów obowiązujących w Uczelni oraz za czyn uchybiający godności studenta na zasadach określonych w Ustawie."_.
>
> Informuję, że w związku z tym **każda praca zaliczeniowa, która będzie osądzona o pracę niesamodzielną i zostanie to udowodnione i zweryfikowane przez prowadzącego oceniona będzie na 0 pkt bez możliwości poprawy**.


## Kontakt
Adrian Albrecht ([aalbrecht@swps.edu.pl](mailto:aalbrecht@swps.edu.pl))
