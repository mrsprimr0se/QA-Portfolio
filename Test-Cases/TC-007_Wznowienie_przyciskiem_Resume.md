
# TC-007 — Wznowienie rozgrywki przyciskiem Resume

**Projekt:** SpaceShooter  
**Rodzaj testu:** Test funkcjonalny  
**Środowisko:** Windows, Unity Editor 2022.3.51f1  
**Data wykonania:** 22.10.2026  
**Wynik:** PASS

## Warunki wstępne (Preconditions)

- Gra SpaceShooter jest uruchomiona.
- Rozgrywka została rozpoczęta.
- Gra została wstrzymana klawiszem ESC.
- Menu pauzy jest widoczne.

## Kroki testowe (Test Steps)

1. Sprawdź, czy w menu pauzy widoczny jest przycisk Resume.
2. Kliknij przycisk Resume.
3. Sprawdź, czy menu pauzy zostaje zamknięte.
4. Sprawdź, czy rozgrywka zostaje wznowiona.

## Oczekiwany rezultat (Expected Result)

- Przycisk Resume jest widoczny w menu pauzy.
- Po kliknięciu Resume menu pauzy zostaje zamknięte.
- Gra powraca do aktywnej rozgrywki.

## Rzeczywisty rezultat (Actual Result)

- Przycisk Resume był widoczny w menu pauzy.
- Po jego kliknięciu rozgrywka została prawidłowo wznowiona.
- Nie zaobserwowano nieprawidłowości w sprawdzonym zakresie.

## Status testu

**PASS**

## Uwagi

Test potwierdził prawidłowe działanie funkcji wznowienia rozgrywki za pomocą przycisku Resume.

Wznowienie gry za pomocą klawisza ESC zostało przetestowane oddzielnie w TC-005.
