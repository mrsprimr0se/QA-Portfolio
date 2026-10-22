
# TC-004 — Wstrzymanie rozgrywki klawiszem ESC

**Projekt:** SpaceShooter  
**Rodzaj testu:** Test funkcjonalny  
**Środowisko:** Windows, Unity Editor 2022.3.51f1  
**Data wykonania:** 22.10.2026  
**Wynik:** PASS

## Warunki wstępne (Preconditions)

- Gra SpaceShooter jest uruchomiona.
- Rozgrywka została rozpoczęta.
- Na ekranie znajdują się poruszające się obiekty.
- Gra nie jest wstrzymana.

## Kroki testowe (Test Steps)

1. Rozpocznij rozgrywkę.
2. Zaobserwuj poruszające się obiekty.
3. Naciśnij klawisz ESC.
4. Sprawdź, czy pojawia się menu pauzy.
5. Sprawdź, czy ruch obiektów zostaje zatrzymany.

## Oczekiwany rezultat (Expected Result)

- Po naciśnięciu ESC pojawia się menu pauzy.
- Rozgrywka zostaje wstrzymana.
- Poruszające się obiekty zatrzymują się.

## Rzeczywisty rezultat (Actual Result)

- Po naciśnięciu ESC wyświetliło się menu pauzy.
- Ruch obiektów w grze został zatrzymany.

## Status testu

**PASS**

## Uwagi

Nie zaobserwowano nieprawidłowości w sprawdzonym zakresie.

Funkcja wznowienia rozgrywki została przetestowana oddzielnie w TC-005.
