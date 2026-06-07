# 🐍 SnakeGame - Konsolowa Gra Snake w C#

Projekt edukacyjny klasycznej gry "Snake" zaimplementowany jako aplikacja konsolowa w języku C#. Głównym celem projektu było przećwiczenie zespołowego cyklu życia kodu (z wykorzystaniem Git i GitHub), debugowanie błędów logicznych oraz zarządzanie konfliktami scalania.

---

## 🎮 Zasady Gry

1. **Cel gry:** Steruj wężem i zbieraj błękitne przeszkody (`*`), aby zwiększać swój wynik (`Score`).
2. **Sterowanie:** Poruszanie po planszy odbywa się za pomocą strzałek na klawiaturze (`GÓRA`, `DÓŁ`, `LEWO`, `PRAWO`).
3. **Przegrana (Game Over) następuje w dwóch przypadkach:**
   * Uderzenie głową węża w białe obramowanie planszy.
   * Najechanie głową węża na swój własny ogon (kolizja z samym sobą).

---

## 🛠️ Wymagania Systemowe i Środowisko

* **Język programowania:** C#
* **Platforma uruchomieniowa:** .NET 8.0 (lub nowszy)
* **Środowisko programistyczne:** Visual Studio 2022 (z zainstalowanym pakietem ".NET desktop development")
* **Typ aplikacji:** Aplikacja konsolowa (Console Application)

---

## 🌿 Struktura Gałęzi w Repozytorium

W projekcie zastosowano uproszczony model pracy **Git Flow**, w którym proces naprawy błędów został odizolowany:
* `main` - Główna, stabilna gałąź zawierająca produkcyjną, działającą wersję gry.
* `fix-syntax-errors-1` - Gałąź dedykowana naprawie błędów kompilacji, zdublowanych deklaracji zmiennych oraz struktury instrukcji `switch`.
* `fix-logic-obstacle-2` - Gałąź robocza odpowiedzialna za korektę operatorów logicznych (`&&`) w detekcji kolizji oraz wdrożenie kolorowania interfejsu.
* `fix-final-bugs-3` - Gałąź naprawiająca braki strukturalne w klasie `Obstakel` i komunikaty końcowe.

Wszystkie zmiany trafiały do gałęzi `main` wyłącznie poprzez formalną procedurę **Pull Request** po uprzedniej recenzji drugiego członka zespołu.

---

## 🚀 Instrukcja Uruchomienia w Visual Studio

1. **Klonowanie projektu:** Sklonuj repozytorium na dysk lokalny za pomocą komendy:
   ```bash
   git clone [https://github.com/jurczykk/SnakeGame.git](https://github.com/jurczykk/SnakeGame.git)
