
# Test Summary Report — SpaceShooter

## 1. Informacje o projekcie

**Projekt:** SpaceShooter  
**Testowana aplikacja:** Gra komputerowa stworzona w Unity  
**Rodzaj testów:** Testy manualne, funkcjonalne  
**Środowisko:** Windows, Unity Editor 2022.3.51f1  
**Data testowania:** 22.10.2026

**Repozytorium aplikacji:**  
https://github.com/mrsprimr0se/SpaceShooter

## 2. Cel testowania

Celem testowania była weryfikacja poprawności działania wybranych podstawowych funkcjonalności gry SpaceShooter, identyfikacja ewentualnych nieprawidłowości oraz udokumentowanie wyników testowania manualnego.

## 3. Zakres testowania

Przeprowadzono testy obejmujące:

- Uruchamianie rozgrywki z menu głównego.
- Sterowanie statkiem gracza.
- Wystrzeliwanie pocisków.
- Wstrzymywanie rozgrywki klawiszem ESC.
- Wznawianie rozgrywki klawiszem ESC.
- Naliczanie punktów po trafieniu przeciwnika.
- Wznawianie rozgrywki przyciskiem Resume.

## 4. Wyniki testów

| ID | Przypadek testowy | Wynik |
|---|---|---|
| TC-001 | Uruchomienie rozgrywki | PASS |
| TC-002 | Poruszanie statkiem | PASS |
| TC-003 | Wystrzeliwanie pocisków | PASS |
| TC-004 | Wstrzymanie rozgrywki | PASS |
| TC-005 | Wznowienie gry klawiszem ESC | PASS |
| TC-006 | Naliczanie punktów | PASS |
| TC-007 | Wznowienie gry przyciskiem Resume | PASS |

### Podsumowanie liczbowe

- Liczba wykonanych przypadków testowych: 7
- PASS: 7
- FAIL: 0
- BLOCKED: 0
- Potwierdzone błędy w testowanym zakresie: 0

**Wynik wykonania zaplanowanych testów: 100% PASS.**

## 5. Analiza nieoczekiwanego zachowania — TC-006

Podczas testowania naliczania punktów zaobserwowano przyrost wyniku z 1 do 2 punktów.

Początkowo oczekiwano przyrostu o 10 punktów na podstawie wartości domyślnej zadeklarowanej w skrypcie C#.

W ramach dodatkowej weryfikacji:

1. Sprawdzono konfigurację obiektu Player.
2. Zweryfikowano przypisany prefab Bullet.
3. Odczytano wartość Points = 1 w Unity Inspector.
4. Porównano konfigurację prefabu z zachowaniem gry.

**Wniosek:** Przyrost wyniku o 1 punkt był zgodny z konfiguracją używanego prefabu.

Nie potwierdzono występowania błędu.

## 6. Wykorzystane narzędzia

- Unity — uruchamianie i testowanie gry.
- Jira — dokumentowanie przypadków testowych i wyników.
- GitHub — przechowywanie dokumentacji.
- Unity Inspector — weryfikacja konfiguracji obiektów.
- Nagrania i zrzuty ekranu — materiały dowodowe.

## 7. Ograniczenia testowania

Przeprowadzone testy obejmowały wybrane podstawowe funkcjonalności gry.

Nie wykonano pełnego testowania wydajnościowego, kompatybilności, bezpieczeństwa ani wszystkich możliwych scenariuszy rozgrywki.

Brak potwierdzonych błędów w wykonanych testach nie oznacza, że aplikacja jest całkowicie wolna od usterek.

## 8. Wnioski końcowe

Wszystkie siedem wykonanych przypadków testowych zakończyło się wynikiem PASS.

W sprawdzonym zakresie funkcje gry działały zgodnie z oczekiwaniami.

Podczas analizy TC-006 przeprowadzono dodatkową weryfikację konfiguracji aplikacji, która pozwoliła wyjaśnić zaobserwowaną rozbieżność bez zgłaszania niepotwierdzonego błędu.

## 9. Rekomendowane dalsze testy

- Sprawdzenie zachowania gry po utracie wszystkich punktów życia.
- Testowanie kolizji statku z przeciwnikami.
- Weryfikacja przechodzenia między poziomami.
- Testowanie szybkiego, wielokrotnego naciskania klawiszy.
- Sprawdzenie działania menu po zakończeniu rozgrywki.
