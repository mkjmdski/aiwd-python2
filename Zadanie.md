Twoim zadaniem jest przeanalizowanie zbioru danych "Online Retail" (zrodlo: na platformie UCI Machine Learning Repository: https://archive.ics.uci.edu/ml/datasets/online+retail), przygotowanie raportu z analizy eksploracyjnej danych (Exploratory Data Analysis, EDA) oraz odpowiedzenie na poniższe **pytania biznesowe**:
1.   Jak przedstawia sie sprzedaz (ilosciowo i wartosciowo) produktow w poszczegolnych krajach i regionach. 
    - Jaka jest srednia wartosc zamowienia? 
    - Ile produktow jest sprzedawanych na jedno zamowienie (fakture)?
    - ilu klientow zlozylo zamowienia?
    - ilu klientow zlozylo zamowienia wiecej niz raz?
2. Ile jest zwrotow produktow i jakie produkty sa najczesciej zwracane.
3. Jakie produkcty sa najbardziej popularne w poszczegolnych krajach.

Do okreslenia regionu uzyj danych z zbioru iso_country.

- Podczas analizy zastanów się jakich informacji brakuje o ktore mógłbyś zapytać SME. 
- Jakie problemy z danymi mozna zidentyfikować i jak można je rozwiązać?

Jako efekt koncowy stworz raport w postaci notatnika zawierajacy:
- podstawowa analize wsztystkich zmiennych: czy zawieraja braki danych, rozklad danych, podstawowe statystyki opisowe, inne istotne informacje ktore uda Ci sie zidentyfikowac.
- odpowiedzi na powyzsze **pytania biznesowe** wraz z wizualizacjami.



Pytania pomocnicze:
1. Customer_id - dlaczego jest floatem? zmienic na Int
5. Faktury [Invoice]:
    - ile mamy faktur?
    - jaki jest rozklad wartosci faktur?
    - ile roznych produktow jest na fakturze?
    - w jakiej liczbie kupowane są produkty?
    - czy da sie zidentyfikowac zwroty?
6. Pozycje na Fakturze [StockCode]:
    - co znajduje sie na fakturze - produkty, dostawa? inne
    - ile mamy produktow? w jakich cenach? Czy cena jest zawsze stala?
    - w jakich ilosciach sa zazwyczaj kupowane? 
    - czy cos sie wyroznia w typach produktow? 
    - czy format codu moze miec jakies znaczenie?
7. Quantity:
    - jakie sa wartosci ujemne? czy to zwroty?
    - jakie sa wartosci ekstremalne?
7. z jakiego okresu czasu mamy dane?
