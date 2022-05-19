Projekt zawiera procedury (klasy) wykorzystywane do otrzymania zestawieñ na stronie
https://wolniludzieslask.github.io/plandemia/
punkt "Nadmiarowe zgony na œwiecie 2020/2021 (19 maja 2022)" (Plandemia)

Katalog pliki_we_wy zawiera dane wejœciowe i wyjœciowe wykorzystywane przez klasy projektu.

Katalog testy zawiera zrzuty ekranów ilustruj¹cych dzia³anie klas.

Poni¿ej opis procedury do otrzymania danych przedstawionych w tabelach:

Rok 2020 i 2021
1. Klasa zgony_swiat_wm.FormatZgonySwiatWm2020_2021
plik wejœciowy world_mortality.csv
plik wyjœciowy zgony_wm2020_2021.txt
2. zgony_swiat_wm.ZgonySwiatSumyWm
plik wejœciowy zgony_wm2020_2021.txt
plik wyjœciowy zgony2020_2021suma.txt
3. Wczytujemy do arkusza OpenOffice Calc,
sortujemy rosn¹co wg kolumny liczby okresów (kolumna F),
usuwamy kraje z ma³¹ liczb¹ okresów np. poni¿ej 16 miesiêcy
(podzielone przez 2 daje 8 miesiêcy w roku)
2 kraje usun¹³em (dane z 6.05.2022): Gibraltar (2 mies), Bia³oruœ (6 mies)
4. Sortujemy wg klumny E (zmiana procentowa)
zapisujemy jako plik csv (zgony2020_2021suma.csv)
5. Plik zgony2020_2021suma.csv kopiujemy na zgony2020_2021suma.in
6. Klasa konwersje.DodanieNumerowWierszy
plik wejœciowy zgony2020_2021suma.in
plik wyjœciowy zgony2020_2021suma1.csv
7. Plik zgony2020_2021suma1.csv wczytujemy do arkusza OpenOffice Calc
Dodajemy nag³ówek, podsumowania i formatujemy dane
zapisujemy w formacie ods (zgony2020_2021suma1.ods)
8. Plik zgony2020_2021suma1.ods zapisujemy w formacie html
(zgony2020_2021suma1.html)
9. Plik zgony2020_2021suma1.html wczytujemy do jEdit, zmieniamy szerokoœci
kolumn tabeli (sekcja COLGROUP) i zapisujemy w kodowaniu UTF-8.
Zmieniamy wielkoœæ czcionki na small, usuwamy kaluzulê RULES=NONE
zmieniamy charset na utf-8
zmieniamy border na 1 (dla tabeli)
10. W pliku nadmiarowe_zgony_swiat2020_2021.html w edytorze 
wklejamy tabelê z pliku zgony2020_2021suma1.html
Opakowujemy tabelê przez
<div style= "width: 1000px" class="table-container">
<table class='scrollable'>
Pierwsz¹ sekcjê TR z tabeli przesuwamy przed <TBODY> i umieszczamy j¹
w sekcji <THEAD>
Zmieniamy z TD na TH dla tego pierwszego wiersza tabeli

Plik zgony_wm2020suma1.html kopiujemy na nadmiarowe_zgony_tabela2021.html
i zmieniamy szerokoœæ kolumn na takie, jak w pliku tabela.css

Rok 2020
11. Klasa zgony_swiat_wm.FormatZgonySwiatWm
plik wejœciowy world_mortality.csv
plik wyjœciowy zgony_wm2020.txt
12. Klasa zgony_swiat_wm.ZgonySwiatWm
plik wejœciowy zgony_wm2020.txt
plik wyjœciowy zgony_wm2020suma.txt
13. Otworzyæ plik zgony_wm2020suma.txt w arkuszu OpenOffice Calc
posortowaæ wiersze wg kolumny zmiana proc.
zapisaæ (zgony_wm2020suma.txt)
14. Skopiowaæ zgony_wm2020suma.txt na zgony_wm2020suma.in
15. Klasa konwersje.DodanieNumerowWierszy2
plik wejœciowy zgony_wm2020suma.in
plik wyjœciowy zgony_wm2020suma1.csv
16. Plik zgony_wm2020suma1.csv wczytujemy do arkusza OpenOffice Calc
Dodajemy nag³ówek, podsumowania i formatujemy dane
zapisujemy w formacie ods (zgony_wm2020suma1.ods)
17. Plik zgony_wm2020suma1.ods zapisujemy w formacie html
(zgony_wm2020suma1.html)
18. Plik zgony_wm2020suma1.html wczytujemy do jEdit, zmieniamy szerokoœci
kolumn tabeli (sekcja COLGROUP) i zapisujemy w kodowaniu UTF-8.
Zmieniamy wielkoœæ czcionki na small, usuwamy kaluzulê RULES=NONE
zmieniamy charset na utf-8
zmieniamy border na 1 (dla tabeli)
19. W pliku nadmiarowe_zgony_swiat2020_2021.html w edytorze 
wklejamy tabelê z pliku zgony_wm2020suma1.html
Opakowujemy tabelê przez
<div style= "width: 1000px" class="table-container">
<table class='scrollable'>
Pierwsz¹ sekcjê TR z tabeli przesuwamy przed <TBODY> i umieszczamy j¹
w sekcji <THEAD>
Zmieniamy z TD na TH dla tego pierwszego wiersza tabeli

Plik zgony_wm2020suma1.html kopiujemy na nadmiarowe_zgony_tabela2021.html
i zmieniamy szerokoœæ kolumn na takie, jak w pliku tabela.css

Rok 2021
20. Klasa zgony_swiat_wm.FormatZgonySwiatWm2021
plik wejœciowy world_mortality.csv
plik wyjœciowy zgony_wm2021.txt
21. Klasa zgony_swiat_wm.ZgonySwiatWm2021
plik wejœciowy zgony_wm2021.txt
plik wyjœciowy zgony_wm2021suma.txt
22. Otworzyæ plik zgony_wm2021suma.txt w arkuszu OpenOffice Calc
posortowaæ wiersze wg kolumny zmiana proc.
zapisaæ (zgony_wm2021suma.csv)
23. Skopiowaæ zgony_wm2021suma.csv na zgony_wm2021suma.in
24. Klasa konwersje.DodanieNumerowWierszy2
plikiem wejœciowym jest zgony_wm2021suma.in
plikiem wyjœciowym zgony_wm2021suma1.csv
25. Plik zgony_wm2021suma1.csv wczytujemy do arkusza OpenOffice Calc
Dodajemy nag³ówek, podsumowania i formatujemy dane
zapisujemy w formacie ods (zgony_wm2021suma1.ods)
26. Plik zgony_wm2021suma1.ods zapisujemy w formacie html
(zgony_wm2021suma1.html)
27. Plik zgony_wm2021suma1.html wczytujemy do jEdit, zmieniamy szerokoœci
kolumn tabeli (sekcja COLGROUP) i zapisujemy w kodowaniu UTF-8.
Zmieniamy wielkoœæ czcionki na small, usuwamy kaluzulê RULES=NONE
zmieniamy charset na utf-8
zmieniamy border na 1 (dla tabeli)
28. W pliku nadmiarowe_zgony_swiat2020_2021.html w edytorze 
wklejamy tabelê z pliku zgony_wm2021suma1.html
Opakowujemy tabelê przez
<div style= "width: 1000px" class="table-container">
<table class='scrollable'>
Pierwsz¹ sekcjê TR z tabeli przesuwamy przed <TBODY> i umieszczamy j¹
w sekcji <THEAD>
Zmieniamy z TD na TH dla tego pierwszego wiersza tabeli

Plik zgony_wm2021suma1.html kopiujemy na nadmiarowe_zgony_tabela2021.html
i zmieniamy szerokoœæ kolumn na takie, jak w pliku tabela.css
