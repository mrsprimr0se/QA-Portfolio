
# TC-003 — Wystrzeliwanie pocisków

**Projekt:** SpaceShooter  
**Rodzaj testu:** Test funkcjonalny  
**Środowisko:** Windows, Unity Editor 2022.3.51f1  
**Data wykonania:** 22.10.2026  
**Wynik:** PASS

## Warunki wstępne (Preconditions)

- Gra SpaceShooter jest uruchomiona.
- Rozgrywka została rozpoczęta.
- Statek gracza jest aktywny.
- Gra nie jest wstrzymana.

## Kroki testowe (Test Steps)

1. Naciśnij i przytrzymaj klawisz SPACJA przez około sekundę.
2. Sprawdź, czy statek wystrzeliwuje pociski.
3. Zaobserwuj kierunek poruszania się pocisków.
4. Zwolnij klawisz SPACJA.
5. Sprawdź, czy nowe pociski przestają być wystrzeliwane.

## Oczekiwany rezultat (Expected Result)

- Podczas przytrzymywania SPACJI statek wystrzeliwuje pociski.
- Pociski poruszają się w górę ekranu.
- Po zwolnieniu SPACJI statek przestaje wystrzeliwać nowe pociski.

## Rzeczywisty rezultat (Actual Result)

- Po przytrzymaniu SPACJI statek wystrzeliwał pociski.
- Pociski przemieszczały się w górę ekranu.
- Po zwolnieniu SPACJI nowe pociski przestawały być wystrzeliwane.

## Status testu

**PASS**

## Uwagi

Nie zaobserwowano nieprawidłowości podczas wykonywania sprawdzanych czynności.

Test obejmował podstawowe działanie mechaniki strzelania. Nie przeprowadzono jeszcze rozszerzonych testów dotyczących szybkiego, wielokrotnego naciskania klawisza.
