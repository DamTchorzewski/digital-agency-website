# Repozytorium: opis i tagi

Rzeczy, które ustawia się na GitHubie ręcznie (nie da się ich zapisać w plikach repozytorium). Przegląd projektu: [README](../README.md).

## Zmiana nazwy na `web-studio`

Standard nazw repozytoriów: `reops/standards/repo-names.md`. Kolejność:

1. GitHub: Settings → General → Repository name → `web-studio`. Adres repozytorium GitHub przekieruje, ale **adres strony (GitHub Pages) zmieni się** z `.../WebStudio/` na `.../web-studio/`, a stary przestanie działać. Settings → Pages nadal ma wskazywać `main` / root.
2. Lokalnie: folder `web-studio` i `git remote set-url origin https://github.com/DamTchorzewski/web-studio.git`.
3. Linki do strony w innych repozytoriach (`WebCraftStudio`: `project-4.html`) wskazują już nowy adres.

## Opis i tagi (About)

GitHub: strona repozytorium → ⚙ obok „About” → pola poniżej. Opis ma limit 350 znaków, tagi (topics) pisze się małymi literami z myślnikami, najwyżej 20.

**Opis (Description):**

```text
Responsive website of a web agency: offer, team, clients and a portfolio of nine projects, with a contact window and a mobile menu. A fast static site (HTML, SASS, vanilla JavaScript) that works on phone, tablet and desktop and is hosted free on GitHub Pages.
```

**Strona (Website):**

```text
https://damtchorzewski.github.io/web-studio/
```

**Tagi (Topics):**

```text
html5 css3 sass scss bem responsive-design mobile-first portfolio-website agency-website github-pages javascript front-end
```

Z GitHub CLI (`gh`) to samo jedną komendą:

```bash
gh repo edit DamTchorzewski/web-studio --homepage "https://damtchorzewski.github.io/web-studio/" --description "Responsive website of a web agency: offer, team, clients and a portfolio of nine projects, with a contact window and a mobile menu. A fast static site (HTML, SASS, vanilla JavaScript) that works on phone, tablet and desktop and is hosted free on GitHub Pages." --add-topic html5,css3,sass,scss,bem,responsive-design,mobile-first,portfolio-website,agency-website,github-pages,javascript,front-end
```

## Ustawienia do włączenia

| Gdzie (GitHub)                                          | Co ustawić                                           |
| ------------------------------------------------------- | ---------------------------------------------------- |
| Settings → Pages                                        | źródło: gałąź `main`, folder `/ (root)` (już działa) |
| Settings → General → Default branch                     | `main` (już jest)                                    |
| Settings → Branches (albo Rulesets) → `main`, `develop` | zablokuj force push i usuwanie gałęzi                |
