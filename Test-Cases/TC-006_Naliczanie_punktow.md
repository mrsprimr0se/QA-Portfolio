
# TC-006 — Naliczanie punktów po trafieniu przeciwnika

**Projekt:** SpaceShooter  
**Rodzaj testu:** Test funkcjonalny  
**Środowisko:** Windows, Unity Editor 2022.3.51f1  
**Data wykonania:** 22.10.2026  
**Wynik:** PASS

## Warunki wstępne (Preconditions)

- Gra SpaceShooter jest uruchomiona.
- Rozgrywka została rozpoczęta.
- Gracz może wystrzeliwać pociski.
- Obiekt Player korzysta z prefabu Bullet.
- W prefabie Bullet ustawiono Points = 1.

## Kroki testowe (Test Steps)

1. Rozpocznij rozgrywkę.
2. Sprawdź aktualną liczbę punktów.
3. Wystrzel pocisk w kierunku przeciwnika.
4. Traf przeciwnika pociskiem.
5. Sprawdź zmianę wyniku punktowego.

## Oczekiwany rezultat (Expected Result)

Po trafieniu przeciwnika wynik zwiększa się o 1 punkt, zgodnie z konfiguracją używanego prefabu Bullet.

## Rzeczywisty rezultat (Actual Result)

- Przed trafieniem przeciwnika wynik wynosił 1 punkt.
- Po trafieniu przeciwnika wynik zwiększył się do 2 punktów.
- Zaobserwowany przyrost wynosił 1 punkt.

## Status testu

**PASS**

## Analiza zaobserwowanej rozbieżności

Podczas testowania zauważono różnicę pomiędzy domyślną wartością punktów w skrypcie C# a rzeczywistym przyrostem punktacji.

W skrypcie BulletController.cs znajduje się deklaracja:

`public int points = 10;`

Weryfikacja w Unity Inspector wykazała jednak, że:

- Player ma przypisany prefab Bullet.
- W komponencie Bullet Controller (Script) zapisano Points = 1.
- Rzeczywisty przyrost punktów wynosił 1.

Wartość zapisana w konfiguracji prefabu nadpisuje wartość domyślną zadeklarowaną w skrypcie.

## Wniosek QA

Zaobserwowany przyrost punktów jest zgodny z konfiguracją używanego prefabu.

Nie potwierdzono błędu w sprawdzonym scenariuszu.

**Ostateczny wynik: PASS**

## Materiały dowodowe (Test Evidence)

- Nagranie rozgrywki przedstawiające zmianę punktacji.
- Zrzut ekranu konfiguracji Player.
- Zrzut ekranu prefabu Bullet z widocznym Points = 1.

Materiały zostały dołączone do dokumentacji testowej w Jira.
