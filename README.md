Portfolio Testera Manualnego QA:

Witaj w moim portfolio testowania manualnego oprogramowania!

Repozytorium dokumentuje moją praktyczną naukę i rozwój umiejętności w zakresie testowania manualnego, ze szczególnym uwzględnieniem testowania gier, testów funkcjonalnych, projektowania przypadków testowych oraz zgłaszania błędów.

O mnie:

Rozwijam się w kierunku Junior QA Tester. Ukończyłam roczne szkolenie Game Design - projektowanie i testowanie gier, podczas którego zdobyłam praktyczne doświadczenie w pracy z Unity, Unreal Engine oraz skryptami C#.

Posiadam doświadczenie w realizacji projektów technicznych oraz korzystaniu z Git i GitHub.

Obecnie rozwijam umiejętności związane z testowaniem manualnym, przygotowywaniem dokumentacji testowej, raportowaniem błędów oraz obsługą narzędzia Jira.

Projekt 1: SpaceShooter - testowanie manualne gry

Testowana aplikacja: SpaceShooter - gra stworzona w Unity

Środowisko testowe: Windows, Unity Editor 2022.3.51f1

Rodzaj testów: Testowanie manualne i funkcjonalne

Wykorzystane narzędzia: Unity, Jira, GitHub

Data testowania: 22.10.2026

Repozytorium gry: https://github.com/mrsprimr0se/SpaceShooter

Zakres przeprowadzonych testów

W ramach testowania sprawdziłam następujące funkcjonalności:

- Uruchamianie rozgrywki z menu głównego.
- Sterowanie postacią - poruszanie się w lewo i prawo.
- Mechanikę wystrzeliwania pocisków.
- Wstrzymywanie rozgrywki klawiszem ESC.
- Wznawianie rozgrywki klawiszem ESC.
- Naliczanie punktów po trafieniu przeciwnika.
- Wznawianie rozgrywki za pomocą przycisku Resume.

Wyniki wykonanych testów

| ID testu | Scenariusz testowy | Wynik |

- TC-001: Uruchomienie rozgrywki z menu głównego- PASS
- TC-002: Poruszanie postacią w lewo i prawo- PASS
- TC-003: Wystrzeliwanie pocisków- PASS
- TC-004: Wstrzymanie rozgrywki klawiszem ESC- PASS
- TC-005: Wznowienie rozgrywki klawiszem ESC- PASS
- TC-006: Naliczanie punktów po trafieniu przeciwnika- PASS
- TC-007: Wznowienie rozgrywki przyciskiem Resume- PASS

Podsumowanie testów

- Liczba wykonanych przypadków testowych: 7
- Testy zakończone sukcesem (PASS): 7
- Testy niezaliczone (FAIL): 0
- Potwierdzone błędy w sprawdzonych scenariuszach: 0

Wszystkie wykonane przypadki testowe zakończyły się wynikiem zgodnym z oczekiwaniami w zakresie przeprowadzonych czynności.

Analiza nieoczekiwanego zachowania - TC-006

Podczas testowania mechanizmu naliczania punktów zaobserwowałam rozbieżność pomiędzy domyślną wartością punktów określoną w skrypcie C# a rzeczywistym przyrostem punktacji w grze.

Zaobserwowane zachowanie:
- Początkowy wynik wynosił 1 punkt.
- Po trafieniu przeciwnika wynik zwiększył się do 2 punktów.
- Rzeczywisty przyrost wynosił 1 punkt, podczas gdy w kodzie C# znajdowała się domyślna wartość 10 punktów.

Podjęte działania:

1. Przeanalizowałam zaobserwowaną rozbieżność.
2. Sprawdziłam konfigurację obiektu Player w Unity Inspector.
3. Zweryfikowałam przypisany prefab Bullet.
4. Ustaliłam, że w komponencie Bullet Controller ustawiono wartość `Points = 1`.
5. Porównałam konfigurację obiektu z rzeczywistym wynikiem testu.

Wniosek:

Gra naliczała punkty zgodnie z konfiguracją prefabu Bullet. Zaobserwowane zachowanie było prawidłowe i nie wymagało utworzenia zgłoszenia błędu.

Ostateczny wynik TC-006: PASS.

Dokumentacja testowa

Przypadki testowe, przebieg testowania oraz wyniki zostały udokumentowane w narzędziu Jira.

Dokumentacja obejmuje:

- Przypadki testowe (Test Cases).
- Warunki wstępne (Preconditions).
- Kroki testowe (Test Steps).
- Oczekiwane rezultaty (Expected Results).
- Rzeczywiste rezultaty (Actual Results).
- Statusy wykonania testów (PASS/FAIL).
- Materiały dowodowe (Test Evidence).

Do dokumentacji testowej dołączono nagrania rozgrywki oraz zrzuty ekranu z Unity Inspector.

Zdobywane i rozwijane umiejętności

- Testowanie manualne oprogramowania.
- Testowanie funkcjonalne gier.
- Projektowanie i wykonywanie przypadków testowych.
- Analiza oczekiwanych i rzeczywistych rezultatów.
- Dokumentowanie wyników testowania.
- Podstawy raportowania błędów.
- Obsługa Jira.
- Analiza nieprawidłowości i weryfikacja konfiguracji aplikacji.
- Testowanie aplikacji w środowisku Unity.
- Wykorzystanie GitHub do dokumentowania projektów.

Dalszy rozwój portfolio

Planuję rozwijać repozytorium poprzez:

- Rozszerzanie zakresu testów funkcjonalnych.
- Przygotowywanie dodatkowych przypadków testowych.
- Dokumentowanie rzeczywiście wykrytych błędów.
- Tworzenie raportów z przebiegu testowania.
- Doskonalenie umiejętności pracy z Jira.
- Naukę testowania REST API przy użyciu Postmana.
- Rozwijanie podstaw SQL przydatnych w testowaniu oprogramowania.

Cel portfolio: praktyczne dokumentowanie rozwoju kompetencji testerskich i przygotowanie do rozpoczęcia kariery zawodowej jako Junior QA Tester / Manual Tester / Game QA.
