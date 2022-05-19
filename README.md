Projekt zawiera procedury (klasy) wykorzystywane do otrzymania zestawie� na stronie
https://wolniludzieslask.github.io/plandemia/
punkt "Nadmiarowe zgony na �wiecie 2020/2021 (19 maja 2022)" (Plandemia)

Katalog pliki_we_wy zawiera dane wej�ciowe i wyj�ciowe wykorzystywane przez klasy projektu.

Katalog testy zawiera zrzuty ekran�w ilustruj�cych dzia�anie klas.

Poni�ej opis procedury do otrzymania danych przedstawionych w tabelach:

Rok 2020 i 2021
1. Klasa zgony_swiat_wm.FormatZgonySwiatWm2020_2021
plik wej�ciowy world_mortality.csv
plik wyj�ciowy zgony_wm2020_2021.txt
2. zgony_swiat_wm.ZgonySwiatSumyWm
plik wej�ciowy zgony_wm2020_2021.txt
plik wyj�ciowy zgony2020_2021suma.txt
3. Wczytujemy do arkusza OpenOffice Calc,
sortujemy rosn�co wg kolumny liczby okres�w (kolumna F),
usuwamy kraje z ma�� liczb� okres�w np. poni�ej 16 miesi�cy
(podzielone przez 2 daje 8 miesi�cy w roku)
2 kraje usun��em (dane z 6.05.2022): Gibraltar (2 mies), Bia�oru� (6 mies)
4. Sortujemy wg klumny E (zmiana procentowa)
zapisujemy jako plik csv (zgony2020_2021suma.csv)
5. Plik zgony2020_2021suma.csv kopiujemy na zgony2020_2021suma.in
6. Klasa konwersje.DodanieNumerowWierszy
plik wej�ciowy zgony2020_2021suma.in
plik wyj�ciowy zgony2020_2021suma1.csv
7. Plik zgony2020_2021suma1.csv wczytujemy do arkusza OpenOffice Calc
Dodajemy nag��wek, podsumowania i formatujemy dane
zapisujemy w formacie ods (zgony2020_2021suma1.ods)
8. Plik zgony2020_2021suma1.ods zapisujemy w formacie html
(zgony2020_2021suma1.html)
9. Plik zgony2020_2021suma1.html wczytujemy do jEdit, zmieniamy szeroko�ci
kolumn tabeli (sekcja COLGROUP) i zapisujemy w kodowaniu UTF-8.
Zmieniamy wielko�� czcionki na small, usuwamy kaluzul� RULES=NONE
zmieniamy charset na utf-8
zmieniamy border na 1 (dla tabeli)
10. W pliku nadmiarowe_zgony_swiat2020_2021.html w edytorze 
wklejamy tabel� z pliku zgony2020_2021suma1.html
Opakowujemy tabel� przez
<div style= "width: 1000px" class="table-container">
<table class='scrollable'>
Pierwsz� sekcj� TR z tabeli przesuwamy przed <TBODY> i umieszczamy j�
w sekcji <THEAD>
Zmieniamy z TD na TH dla tego pierwszego wiersza tabeli

Plik zgony_wm2020suma1.html kopiujemy na nadmiarowe_zgony_tabela2021.html
i zmieniamy szeroko�� kolumn na takie, jak w pliku tabela.css

Rok 2020
11. Klasa zgony_swiat_wm.FormatZgonySwiatWm
plik wej�ciowy world_mortality.csv
plik wyj�ciowy zgony_wm2020.txt
12. Klasa zgony_swiat_wm.ZgonySwiatWm
plik wej�ciowy zgony_wm2020.txt
plik wyj�ciowy zgony_wm2020suma.txt
13. Otworzy� plik zgony_wm2020suma.txt w arkuszu OpenOffice Calc
posortowa� wiersze wg kolumny zmiana proc.
zapisa� (zgony_wm2020suma.txt)
14. Skopiowa� zgony_wm2020suma.txt na zgony_wm2020suma.in
15. Klasa konwersje.DodanieNumerowWierszy2
plik wej�ciowy zgony_wm2020suma.in
plik wyj�ciowy zgony_wm2020suma1.csv
16. Plik zgony_wm2020suma1.csv wczytujemy do arkusza OpenOffice Calc
Dodajemy nag��wek, podsumowania i formatujemy dane
zapisujemy w formacie ods (zgony_wm2020suma1.ods)
17. Plik zgony_wm2020suma1.ods zapisujemy w formacie html
(zgony_wm2020suma1.html)
18. Plik zgony_wm2020suma1.html wczytujemy do jEdit, zmieniamy szeroko�ci
kolumn tabeli (sekcja COLGROUP) i zapisujemy w kodowaniu UTF-8.
Zmieniamy wielko�� czcionki na small, usuwamy kaluzul� RULES=NONE
zmieniamy charset na utf-8
zmieniamy border na 1 (dla tabeli)
19. W pliku nadmiarowe_zgony_swiat2020_2021.html w edytorze 
wklejamy tabel� z pliku zgony_wm2020suma1.html
Opakowujemy tabel� przez
<div style= "width: 1000px" class="table-container">
<table class='scrollable'>
Pierwsz� sekcj� TR z tabeli przesuwamy przed <TBODY> i umieszczamy j�
w sekcji <THEAD>
Zmieniamy z TD na TH dla tego pierwszego wiersza tabeli

Plik zgony_wm2020suma1.html kopiujemy na nadmiarowe_zgony_tabela2021.html
i zmieniamy szeroko�� kolumn na takie, jak w pliku tabela.css

Rok 2021
20. Klasa zgony_swiat_wm.FormatZgonySwiatWm2021
plik wej�ciowy world_mortality.csv
plik wyj�ciowy zgony_wm2021.txt
21. Klasa zgony_swiat_wm.ZgonySwiatWm2021
plik wej�ciowy zgony_wm2021.txt
plik wyj�ciowy zgony_wm2021suma.txt
22. Otworzy� plik zgony_wm2021suma.txt w arkuszu OpenOffice Calc
posortowa� wiersze wg kolumny zmiana proc.
zapisa� (zgony_wm2021suma.csv)
23. Skopiowa� zgony_wm2021suma.csv na zgony_wm2021suma.in
24. Klasa konwersje.DodanieNumerowWierszy2
plikiem wej�ciowym jest zgony_wm2021suma.in
plikiem wyj�ciowym zgony_wm2021suma1.csv
25. Plik zgony_wm2021suma1.csv wczytujemy do arkusza OpenOffice Calc
Dodajemy nag��wek, podsumowania i formatujemy dane
zapisujemy w formacie ods (zgony_wm2021suma1.ods)
26. Plik zgony_wm2021suma1.ods zapisujemy w formacie html
(zgony_wm2021suma1.html)
27. Plik zgony_wm2021suma1.html wczytujemy do jEdit, zmieniamy szeroko�ci
kolumn tabeli (sekcja COLGROUP) i zapisujemy w kodowaniu UTF-8.
Zmieniamy wielko�� czcionki na small, usuwamy kaluzul� RULES=NONE
zmieniamy charset na utf-8
zmieniamy border na 1 (dla tabeli)
28. W pliku nadmiarowe_zgony_swiat2020_2021.html w edytorze 
wklejamy tabel� z pliku zgony_wm2021suma1.html
Opakowujemy tabel� przez
<div style= "width: 1000px" class="table-container">
<table class='scrollable'>
Pierwsz� sekcj� TR z tabeli przesuwamy przed <TBODY> i umieszczamy j�
w sekcji <THEAD>
Zmieniamy z TD na TH dla tego pierwszego wiersza tabeli

Plik zgony_wm2021suma1.html kopiujemy na nadmiarowe_zgony_tabela2021.html
i zmieniamy szeroko�� kolumn na takie, jak w pliku tabela.css
