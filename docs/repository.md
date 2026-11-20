# Repozytorium: opis i tagi

Rzeczy, które ustawia się na GitHubie ręcznie (nie da się ich zapisać w plikach repozytorium). Przegląd projektu: [README](../README.md).

## Nazwa repozytorium: `digital-agency-website`

Standard nazw repozytoriów: `reops/standards/repo-names.md`. Repozytorium nazywało się wcześniej `WebStudio`, potem `web-studio`; od 2026-11-20 nazywa się `digital-agency-website` (nazwa mówi, czym jest projekt: fraza szukana na GitHubie). GitHub przekierowuje stary adres repozytorium, ale **adres strony (GitHub Pages) zmienił się** na `https://damtchorzewski.github.io/digital-agency-website/`, a stary przestał działać. Settings → Pages nadal wskazuje `main` / root. Linki do strony w innych repozytoriach (`WebCraftStudio`: `project-4.html`) trzeba poprawić na nowy adres.

## Opis i tagi (About)

GitHub: strona repozytorium → ⚙ obok „About” → pola poniżej. Opis ma limit 350 znaków, tagi (topics) pisze się małymi literami z myślnikami, najwyżej 20.

**Opis (Description):**

```text
Responsive static agency website in HTML, SASS and JavaScript: portfolio grid and modals.
```

**Strona (Website):**

```text
https://damtchorzewski.github.io/digital-agency-website/
```

**Tagi (Topics):**

```text
html5 css3 sass bem responsive-design mobile-first portfolio-website agency-website github-pages javascript front-end
```

Z GitHub CLI (`gh`) to samo jedną komendą:

```bash
gh repo edit DamTchorzewski/digital-agency-website --homepage "https://damtchorzewski.github.io/digital-agency-website/" --description "Responsive static agency website in HTML, SASS and JavaScript: portfolio grid and modals." --add-topic html5 --add-topic css3 --add-topic sass --add-topic bem --add-topic responsive-design --add-topic mobile-first --add-topic portfolio-website --add-topic agency-website --add-topic github-pages --add-topic javascript --add-topic front-end
```

## Ustawienia do włączenia

| Gdzie (GitHub)                                          | Co ustawić                                           |
| ------------------------------------------------------- | ---------------------------------------------------- |
| Settings → Pages                                        | źródło: gałąź `main`, folder `/ (root)` (już działa) |
| Settings → General → Default branch                     | `main` (już jest)                                    |
| Settings → Branches (albo Rulesets) → `main`, `develop` | zablokuj force push i usuwanie gałęzi                |
