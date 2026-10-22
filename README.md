# Portfolio QA — Testowanie Manualne i Game QA

Witaj w moim portfolio testowania manualnego oprogramowania!

Repozytorium prezentuje moje praktyczne doświadczenia związane z testowaniem funkcjonalnym gier, projektowaniem przypadków testowych, dokumentowaniem wyników oraz analizowaniem zaobserwowanych nieprawidłowości.

## O mnie

Rozwijam się w kierunku **Junior QA Tester / Manual Tester / Game QA**.

Ukończyłam roczne kształcenie w zakresie Game Design, podczas którego pracowałam z silnikami Unity i Unreal Engine oraz rozwijałam podstawy programowania w C#.

Obecnie doskonalę umiejętności testowania manualnego, przygotowywania dokumentacji testowej, pracy z Jira oraz wykorzystywania GitHub do prezentacji projektów.

## Projekt 1 — SpaceShooter

**Testowana aplikacja:** SpaceShooter — gra stworzona w Unity

**Środowisko:** Windows, Unity Editor 2022.3.51f1

**Rodzaj testów:** Manualne testy funkcjonalne

**Narzędzia:** Unity, Unity Inspector, Jira, GitHub

**Data testowania:** 22 października 2026 r.

**Kod źródłowy gry:** [SpaceShooter — GitHub](https://github.com/mrsprimr0se/SpaceShooter)

### Cel testowania

Sprawdzenie poprawności działania wybranych podstawowych funkcjonalności gry oraz udokumentowanie przebiegu i wyników testów.

### Przypadki testowe i wyniki

| ID | Scenariusz testowy | Wynik |
|---|---|---|
| [TC-001](Test-Cases/TC-001_Uruchomienie_rozgrywki.md) | Uruchomienie rozgrywki z menu głównego | PASS |
| [TC-002](Test-Cases/TC-002_Poruszanie_statkiem.md) | Poruszanie statkiem w lewo i prawo | PASS |
| [TC-003](Test-Cases/TC-003_Wystrzeliwanie_pociskow.md) | Wystrzeliwanie pocisków | PASS |
| [TC-004](Test-Cases/TC-004_Wstrzymanie_rozgrywki.md) | Wstrzymanie rozgrywki klawiszem ESC | PASS |
| [TC-005](Test-Cases/TC-005_Wznowienie_rozgrywki_ESC.md) | Wznowienie rozgrywki klawiszem ESC | PASS |
| [TC-006](Test-Cases/TC-006_Naliczanie_punktow.md) | Naliczanie punktów po trafieniu przeciwnika | PASS |
| [TC-007](Test-Cases/TC-007_Wznowienie_przyciskiem_Resume.md) | Wznowienie rozgrywki przyciskiem Resume | PASS |

### Podsumowanie wyników

- **Wykonane testy:** 7
- **PASS:** 7
- **FAIL:** 0
- **Potwierdzone błędy w testowanym zakresie:** 0

Wszystkie siedem wykonanych przypadków testowych zakończyło się wynikiem PASS.

Brak wykrytych błędów dotyczy wyłącznie sprawdzonych scenariuszy i nie oznacza, że cała aplikacja jest wolna od usterek.

### Raport końcowy

[Otwórz raport z testowania SpaceShooter](Test-Reports/SpaceShooter_Test_Summary_Report.md)

Raport zawiera zakres testów, środowisko, wyniki, ograniczenia testowania, dodatkową analizę oraz wnioski końcowe.

## Analiza QA — TC-006

Podczas weryfikacji mechaniki naliczania punktów zauważyłam różnicę między domyślną wartością punktów w skrypcie C# a wynikiem obserwowanym podczas rozgrywki.

**Zaobserwowane zachowanie:**

- Wynik wzrósł z 1 do 2 punktów.
- W skrypcie `BulletController.cs` znajdowała się domyślna wartość `points = 10`.
- W Unity Inspector używany prefab Bullet miał ustawienie `Points = 1`.

**Podjęte działania:**

1. Sprawdziłam konfigurację obiektu Player.
2. Zweryfikowałam prefab Bullet przypisany do gracza.
3. Porównałam ustawienia prefabu z rzeczywistym zachowaniem gry.

**Wniosek:** Gra naliczała punkty zgodnie z konfiguracją prefabu. Nie potwierdzono błędu.

**Wynik TC-006: PASS.**

### Materiały dowodowe

- [TC-006 — przypisanie prefabu Bullet do obiektu Player](Test-Evidence/TC-006_Player_BulletPrefab.png)
- [TC-006 — konfiguracja Points = 1](Test-Evidence/TC-006_Bullet_Points1.png)
- [Folder z materiałami dowodowymi](Test-Evidence/README.md)

## Dokumentacja projektu

W repozytorium znajdują się trzy główne foldery:

- **[Test-Cases](Test-Cases/)** — szczegółowe przypadki testowe z krokami, oczekiwanymi i rzeczywistymi rezultatami.
- **[Test-Reports](Test-Reports/)** — raport podsumowujący przeprowadzone testy.
- **[Test-Evidence](Test-Evidence/)** — materiały dowodowe z testowania w Unity.

Dodatkowa dokumentacja testowa oraz nagranie rozgrywki zostały zapisane w Jira.

## Umiejętności prezentowane w projekcie

- Projektowanie i wykonywanie testów funkcjonalnych.
- Tworzenie przypadków testowych (Test Cases).
- Dokumentowanie wyników testów.
- Analiza oczekiwanych i rzeczywistych rezultatów.
- Weryfikowanie konfiguracji aplikacji w Unity Inspector.
- Rozpoznawanie różnicy między błędem a prawidłowym zachowaniem aplikacji.
- Korzystanie z Jira i GitHub.

## Dalszy rozwój

Planuję rozbudowywać portfolio o kolejne scenariusze testowe, rzeczywiście wykryte błędy, raporty QA oraz projekty związane z testowaniem API i podstawami SQL.

---

**Cel portfolio:** przedstawienie praktycznych umiejętności i dokumentowanie rozwoju w kierunku Junior QA Tester / Manual Tester / Game QA.
