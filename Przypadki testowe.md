
### Przypadek testowy nr 1 - walidacja pola e-mail oraz przycisku do sprawdzania adresu email. 		 		
		
Kroki|Oczekiwany rezultat|Rzeczywisty rezultat 
---|---|---
Otworzenie ekranu sprawdzania adresu email|Otwiera się ekran z możliwością wpisania adresu e-mail| 	
Wpisanie adresu email w złym formacie (np.: jan.nowak@mail@com)|Wyświetla się komunikat dla usera o wprowadzeniu nieprawidłowych danych| 	
Kliknięcie w przycisk "x" w celu usunięcia całego tekstu z pola|Cały wprowadzony tekst został usunięty|	
Wprowadzenie adresu email w poprawnym formacie|Uaktywnia się przycisk do weryfikacji obecności adresu email w bazie zarejestrowanych użytkowników| 	
<br />

### Przypadek testowy numer 2: weryfikacja możliwości założenia konta użytkownika z podaniem poprawnych danych oraz walidacja pola email		
		
Krok|Oczekiwany rezultat|Rzeczywisty rezultat
---|---|--- 
Kliknięcie w pole email w celu edycji tego pola|Pole jest nieedytowalne|	
Przejście na pole "Hasło" poprzez kliknięcie na nie|Po wejściu na pole "Hasło" pod polem pojawia się informacja o wymaganiach dla hasła| 	
Uzupełnienie  wymaganego pola "Hasło" z uzyciem minimum 8 znaków, w tym liter i cyfr|Po wpisaniu hasła zgodnego z wymaganiami i przejściu na kolejną część formularza, pole zaznacza się na zielono|
Kliknięcie na "oczko" w celu odkrycia hasła|Po kliknięciu na "oczko", hasło zostaje odkryte|
Uzupełnienie wymaganego pola "Imię" poprawnymi danymi|Po wypełnieniu pola i przejściu na kolejną część formularza, zaznacza się ono na zielono|	
Uzupełnienie wymaganego pola "Nazwisko" poprawnymi danymi|Po wypełnieniu pola i przejściu na kolejną część formularza, zaznacza się ono na zielono|	
Zaznaczenie trzech pól typu checkbox (w tym checkboxa wymaganego, oznaczonego gwiazdką)|Checkboxy zostają zaznaczone, a przycisk "załóż konto" staje się aktywne i podświetla się na różowo|Dostępne są tylko dwa pola typu checkbox|

 		
		
### Przypadek testowy numer 3: weryfikacja możliwości założenia konta nowego użytkownika z podaniem niepoprawnych danych lub brakiem danych 		
		
Krok|Oczekiwany rezultat|Rzeczywisty rezultat
---|---|--- 
Wypełnienie wymaganego pola "Hasło" z użyciem 8 znaków, ale tylko liter|Po wpisaniu hasła niezgodnego z wymaganiami i przejściu na kolejną część formularza, pole zaznacza się na czerwono| 	
Uzupełnienie wymaganego pola "Imię" poprawnymi danymi|Pole zostało uzupełnione|	
Usunięcie danych  z pola "Imię" poprzez użycie krzyżyka|Po usunięciu danych z pola i przejściu na kolejną część formularza, pole zaznacza się na czerwono| 	
Uzupełnienie wymaganego pola "Nazwisko" poprawnymi danymi|Pole zostało uzupełnione|	
Usunięcie danych  z pola "Nazwisko" poprzez użycie krzyżyka|Po usunięciu danych z pola i przejściu na kolejną część formularza, pole zaznacza się na czerwono| 	
Przejście dalej w celu dokończenia rejestracji nowego użytkownika|Przycisk "załóż konto" jest nieaktywny, co uniemożliwia dokończenie rejestracji nowego użytkownika| 	


		
### Przypadek testowy numer 4: walidacja pola "Klauzula o ochronie danych osobowych"		
		
Krok|Oczekiwany rezultat|Rzeczywisty rezultat
---|---|--- 
Kliknięcie na "Klauzula o ochronie danych osobowych" w celu uzyskania więcej informacji|Użytkownik zostaje przeniesiony do osobnego ekranu z klauzula| 	
Kliknięcie na jeden z linków dostępnych w tekście klauzuli|Użytkownik zostaje przeniesiony na webview| 	
Kliknięcie na adres email dostępny w tekście klauzuli|Użytkownik zostaje przeniesiony na pocztę|Użytkownik nie zostaje przeniesiony na pocztę, lecz wyświetla się biały ekran|

 

### Przypadek testowy numer 5: weryfikacja poprawności wysłania linku potwierdzającgo założenie konta 		
		
Krok|Oczekiwany rezultat|Rzeczywisty rezultat
---|---|--- 
Kliknięcie w przycisk "załóż konto" na ekranie z formularzem założenia konta|Użytkownik zostaje przeniesiony na ekran wysłania formularza z linkiem potwierdzającym| 	
Sprawdzenie poprawności danych|Adres e-mail wyświetlony w informacji jest zgodny z adresem email podanym przez użytkownika w procesie rejestracji| 	
Kliknięcie w przycisk "zaloguj się"|Użytkownik zostaje przeniesiony na ekran logowania|

 	
			
### Przypadek testowy numer 6: weryfikacja próby ponownego wysłania linka aktywacyjnego w przypadku nieotrzymania maila potwierdzającego założenie konta 		
		
Krok|Oczekiwany rezultat|Rzeczywisty rezultat
---|---|--- 
Kliknięcie w przycisk "załóż konto" na ekranie z formularzem założenia konta|Użytkownik zostaje przeniesiony na ekran wysłania formularza z linkiem potwierdzającym| 	
Sprawdzenie poprawności danych|Adres e-mail wyświetlony w informacji jest zgodny z adresem email podanym przez użytkownika w procesie rejestracji| 	
Kliknięcie w przycsik "wyślij link ponownie"|Na górze ekranu wyświetla się popup koloru zielonego z informacją o ponownym wysłaniu linku aktywacyjnego|

 	
		
### Przypadek testowy numer 7: weryfikacja logowania użytkownika po aktywacji konta 		
		
Krok|Oczekiwany rezultat|Rzeczywisty rezultat 
---|---|---
Kliknięcie w link aktywacyjny otrzymany na adres email podany w czasie rejestracji|Użytkownik zostaje przeniesiony na ekran logowania| 	
Wpisanie poprawnych danych logowania|Poprawne dane zostały wpisane| 	
Kliknięcie w przycisk "zaloguj się"|Użytkownik zostaje zalogowany do aplikacji oraz przeniesiony do zakładki "Więcej"|	
