
# TC-002 — Poruszanie statkiem w lewo i prawo

**Projekt:** SpaceShooter  
**Rodzaj testu:** Test funkcjonalny  
**Środowisko:** Windows, Unity Editor 2022.3.51f1  
**Data wykonania:** 22.10.2026  
**Wynik:** PASS

## Warunki wstępne (Preconditions)

- Gra SpaceShooter jest uruchomiona.
- Rozgrywka została rozpoczęta.
- Statek gracza jest aktywny.

## Kroki testowe (Test Steps)

1. Naciśnij i przytrzymaj klawisz A.
2. Sprawdź, czy statek porusza się w lewo.
3. Naciśnij i przytrzymaj klawisz D.
4. Sprawdź, czy statek porusza się w prawo.
5. Zwolnij klawisze sterowania.
6. Sprawdź, czy statek zatrzymuje się.

## Oczekiwany rezultat (Expected Result)

- Klawisz A powoduje ruch statku w lewo.
- Klawisz D powoduje ruch statku w prawo.
- Po zwolnieniu klawiszy statek przestaje się poruszać.

## Rzeczywisty rezultat (Actual Result)

- Statek prawidłowo poruszał się w lewo po naciśnięciu klawisza A.
- Statek prawidłowo poruszał się w prawo po naciśnięciu klawisza D.
- Po zwolnieniu klawiszy statek zatrzymywał się.

## Status testu

**PASS**

## Uwagi

Nie zaobserwowano nieprawidłowości podczas wykonywania sprawdzanych czynności.
