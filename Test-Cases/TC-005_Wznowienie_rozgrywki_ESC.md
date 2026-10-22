
# TC-005 — Wznowienie rozgrywki klawiszem ESC

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

1. Naciśnij ponownie klawisz ESC.
2. Sprawdź, czy menu pauzy zostało zamknięte.
3. Sprawdź, czy obiekty w grze ponownie się poruszają.
4. Naciśnij klawisze A i D, aby sprawdzić sterowanie statkiem.
5. Naciśnij SPACJĘ, aby sprawdzić możliwość strzelania.

## Oczekiwany rezultat (Expected Result)

- Menu pauzy zostaje zamknięte.
- Rozgrywka zostaje wznowiona.
- Obiekty ponownie zaczynają się poruszać.
- Sterowanie statkiem i strzelanie działają prawidłowo.

## Rzeczywisty rezultat (Actual Result)

- Po ponownym naciśnięciu ESC menu pauzy zniknęło.
- Obiekty w grze ponownie zaczęły się poruszać.
- Sterowanie statkiem za pomocą klawiszy A i D działało prawidłowo.
- Wystrzeliwanie pocisków za pomocą SPACJI działało prawidłowo.

## Status testu

**PASS**

## Uwagi

Nie zaobserwowano nieprawidłowości podczas wykonywania testu.

Wznowienie rozgrywki za pomocą przycisku Resume zostało przetestowane oddzielnie w TC-007.
