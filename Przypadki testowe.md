
### Przypadek testowy nr 1 - Walidacja pola e-mail oraz przycisku do sprawdzenia adresu email. 		 		
		
Kroki|Oczekiwany rezultat|Rzeczywisty rezultat 
---|---|---
Otworzenie ekranu sprawdzania adresu email|Otwiera się ekran z możliwością wpisania adresu e-mail| 	&#x2611;
Wpisanie adresu email w złym formacie (np.: jan.nowak@mail@com)|Wyświetla się komunikat dla usera o wprowadzeniu nieprawidłowych danych| 	&#x2611;
Kliknięcie w przycisk "x" w celu usunięcia całego tekstu z pola|Cały wprowadzony tekst został usunięty|	&#x2611;
Wprowadzenie adresu email w poprawnym formacie|Uaktywnia się przycisk do weryfikacji obecności adresu email w bazie zarejestrowanych użytkowników| 	&#x2611;
Kliknięcie w przycisk "Sprawdź email"|Użytkownik zostaje przeniesiony na ekran z formularzem założenia konta| &#x2611;
<br />

### Przypadek testowy numer 2: Weryfikacja możliwości założenia konta użytkownika z podaniem poprawnych danych		
		
Krok|Oczekiwany rezultat|Rzeczywisty rezultat
---|---|--- 
Przejście na pole "Hasło" poprzez kliknięcie na nie|Po wejściu na pole "Hasło" pod polem pojawia się informacja o wymaganiach dla hasła| 	&#x2611;
Uzupełnienie  wymaganego pola "Hasło" z użyciem minimum 8 znaków, w tym liter i cyfr|Po wpisaniu hasła zgodnego z wymaganiami i przejściu na kolejną część formularza, pole zaznacza się na zielono|&#x2611;
Kliknięcie na "oczko" w celu odkrycia hasła|Po kliknięciu na "oczko", hasło zostaje odkryte|&#x2611;
Uzupełnienie wymaganego pola "Imię" poprawnymi danymi|Po wypełnieniu pola i przejściu na kolejną część formularza, zaznacza się ono na zielono|	&#x2611;
Uzupełnienie wymaganego pola "Nazwisko" poprawnymi danymi|Po wypełnieniu pola i przejściu na kolejną część formularza, zaznacza się ono na zielono|	&#x2611;
Zaznaczenie trzech pól typu checkbox (w tym checkboxów wymaganych, oznaczonych gwiazdką)|Checkboxy zostają zaznaczone, a przycisk "załóż konto" staje się aktywne i podświetla się na różowo|Dostępne są tylko dwa pola typu checkbox
<br>

### Przypadek testowy numer 3: Walidacja pola email oraz weryfikacja możliwości założenia konta nowego użytkownika bez podania danych
Krok|Oczekiwany rezultat|Rzeczywisty rezultat
---|---|--- 
Kliknięcie w pole email w celu edycji tego pola|Pole jest nieedytowalne|	&#x2611;
Kliknięcie w przycisk "Załóż konto"|Przycisk "załóż konto" jest przyciemniony i nie ma możliwości kliknięcia w niego|	&#x2611;
<br>
	
### Przypadek testowy numer 4: Weryfikacja możliwości założenia konta nowego użytkownika z podaniem niepoprawnych danych lub brakiem danych 		
		
Krok|Oczekiwany rezultat|Rzeczywisty rezultat
---|---|--- 
Wypełnienie wymaganego pola "Hasło" niezgodnie z wymaganiami (np. z użyciem minimum 8 znaków, ale wyłącznie liter)|Po wpisaniu hasła niezgodnego z wymaganiami i przejściu na kolejną część formularza, pole zaznacza się na czerwono| 	&#x2611;
Uzupełnienie wymaganego pola "Imię" poprawnymi danymi|Pole zostało uzupełnione|	&#x2611;
Usunięcie danych  z pola "Imię" poprzez użycie krzyżyka|Po usunięciu danych z pola i przejściu na kolejną część formularza, pole zaznacza się na czerwono| 	&#x2611;
Uzupełnienie wymaganego pola "Nazwisko" poprawnymi danymi|Pole zostało uzupełnione|	&#x2611;
Usunięcie danych  z pola "Nazwisko" poprzez użycie krzyżyka|Po usunięciu danych z pola i przejściu na kolejną część formularza, pole zaznacza się na czerwono| 	&#x2611;
Przejście dalej w celu dokończenia rejestracji nowego użytkownika|Przycisk "załóż konto" jest przyciemniony i nie ma możliwości kliknięcia w niego| 	&#x2611;
<br>
		
### Przypadek testowy numer 5: Walidacja pola "Klauzula o ochronie danych osobowych"		
		
Krok|Oczekiwany rezultat|Rzeczywisty rezultat
---|---|--- 
Kliknięcie na tekst "Klauzula o ochronie danych osobowych" na ekranie z fomularzem założenia konta |Użytkownik zostaje przeniesiony do osobnego ekranu, który zawiera tekst klauzuli| 	&#x2611;
Kliknięcie na jeden z linków dostępnych w tekście klauzuli|Użytkownik zostaje przeniesiony na webview| 	&#x2611;
Kliknięcie na adres email dostępny w tekście klauzuli|Użytkownik zostaje przeniesiony na pocztę|Użytkownik nie zostaje przeniesiony na pocztę, lecz wyświetla się biały ekran|
<br>

### Przypadek testowy numer 6: Weryfikacja poprawności wysłania linku potwierdzającego założenie konta 		
Warunek wstępny: Użytkownik podał poprawne dane potrzebne do rejestracji.

Krok|Oczekiwany rezultat|Rzeczywisty rezultat
---|---|--- 
Kliknięcie w przycisk "załóż konto" na ekranie z formularzem założenia konta|Użytkownik zostaje przeniesiony na ekran wysłania formularza z linkiem potwierdzającym| 	&#x2611;
Sprawdzenie poprawności danych|Adres e-mail wyświetlony w informacji jest zgodny z adresem email podanym przez użytkownika w procesie rejestracji| 	&#x2611;
Kliknięcie w przycisk "zaloguj się"|Użytkownik zostaje przeniesiony na ekran logowania|&#x2611;
<br>
			
### Przypadek testowy numer 7: Weryfikacja próby ponownego wysłania linka aktywacyjnego w przypadku nieotrzymania maila potwierdzającego założenie konta 	
Warunek wstępny: Użytkownik nie otrzymał na podany adres email maila z linkiem potwierdzającym założenie konta lub link potwierdzający założenie konta wygasł

Krok|Oczekiwany rezultat|Rzeczywisty rezultat
---|---|--- 
Kliknięcie w przycisk "załóż konto" na ekranie z formularzem założenia konta|Użytkownik zostaje przeniesiony na ekran wysłania formularza z linkiem potwierdzającym| 	&#x2611;
Sprawdzenie poprawności danych|Adres e-mail wyświetlony w informacji jest zgodny z adresem email podanym przez użytkownika w procesie rejestracji| 	&#x2611;
Kliknięcie w przycisk "wyślij link ponownie"|Na górze ekranu wyświetla się popup koloru zielonego z informacją o ponownym wysłaniu linku aktywacyjnego|&#x2611;
<br>
		
### Przypadek testowy numer 8: weryfikacja logowania użytkownika po aktywacji konta 		
Warunek wstępny: Użytkownik przeszedł proces rejestracji i otrzymał link potwierdzający założenie konta na adres email podany w procesie rejestracji

Krok|Oczekiwany rezultat|Rzeczywisty rezultat 
---|---|---
Kliknięcie w link aktywacyjny otrzymany na adres email podany w czasie rejestracji|Użytkownik zostaje przeniesiony na ekran logowania| 	&#x2611;
Wpisanie poprawnych danych logowania|Poprawne dane zostały wpisane| 	&#x2611;
Kliknięcie w przycisk "zaloguj się"|Użytkownik zostaje zalogowany do aplikacji oraz przeniesiony do zakładki "Więcej"|	&#x2611;
<br>
