## Analize strat w zbiorze Online Retail

**Definicje:**
- **Straty** = rekordy BEZ `customer_id`
- **Zwroty** = faktury zaczynające się na "C" ORAZ z `customer_id`
- **Zamówienia** = pozostałe rekordy (z `customer_id`, nie zaczynające się na "C")

**WYKLUCZYĆ z analizy:**
- Faktury zaczynające się na "A"
- Dwa zamówienia oraz zwroty z liczbą produktów ≥ 70,000 (podejrzanie duże wartości)

---

**Minimalne kryteria zaliczenia:**

1. Przygotuj dane: 
    * wyklucz faktury zaczynające sie na "A" i te z Quantity > 70 000;
    * wyodrębnij zwroty, zamówienia i straty. 

2. Przygotuj zestawienie porównujące produkty zamówione i utracone: 
    * WYNIK - Tabela z kolumnami: 
        - StockCode, 
        - suma quantity dla zamówień
        - średnia (a moze mediana?) z Unit Price dla zamówien 
        - suma quantity dla strat
        - średnia (a moze mediana?) z Unit Price dla strat 
    * PODPOWIEDZ: mozna to zrobić w dwóch krokach: zgrupować i zagregowac dane osobno dla zamówień i strat a następnie połączyc oba zbiory (funkcja merge).

3. Przygotuj wykres z wielkością strat w poszczególnych miesiacach. Opisz krótko w jaki sposob zdefiniowałaś/eś "wielkość strat" i jak jeszcze inaczej mozna by ją zdefiniować.


--- 

**Pytania pomocnicze:**

1. ze wszystkich dostepnych produktow - jakie produktu sa najczesciej "tracone"? Czy częściej zamawiane produkty sa częściej tracone? 
    - jako wszystkie produkty weź te, które sa dostepne w naszym zbiorze danych i byly zamawiane lub utracone. 
2. czy byly stracone jakieś produkty, które nigdy nie byly zamówione?
3. w jakich okresach identyfikowane sa straty? (codziennie czy np. tylko pod koniec tygodnia? czy widać, zeby w jakims okresie było wiecej / mniej strat?)
4. czy wartosc (UnitPrice) jest wpisywana przy stratach? zestaw rozkład wartosci UnitPrice dla strat z wartościa wpisywana w zamówieniu - znajdź produkty z najwieksza róznica na wartości średniej i/lub medianie.
5. jaki jest rozklad strat w poszczególnych miesiacach / tygodniach? - czy lepszą miarą bedzie liczba (Quantity) czy wartość? 
6. Na jakie kraje zapisywane są straty?
7. Czy jakies rekordy (produkty, wartosci) wydaja sie dziwne w tym zestawieniu?


