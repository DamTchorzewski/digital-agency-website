# Repozytorium: opis i tagi

Rzeczy, które ustawia się na GitHubie ręcznie (nie da się ich zapisać w plikach repozytorium). Przegląd projektu: [README](../README.md).

## Opis i tagi (About)

GitHub: strona repozytorium → ⚙ obok „About” → pola poniżej. Opis ma limit 350 znaków, tagi (topics) pisze się małymi literami z myślnikami, najwyżej 20.

**Opis (Description):**

```text
Responsive two-page site of a web agency: home with offer, team, skills and clients, and a portfolio page with nine projects. Semantic HTML5, BEM, SASS, mobile-first with x1/x2/x3 images, mobile menu and modal. Hosted on GitHub Pages.
```

**Strona (Website):**

```text
https://damtchorzewski.github.io/WebStudio/
```

**Tagi (Topics):**

```text
html5 css3 sass scss bem responsive-design mobile-first portfolio-website landing-page github-pages javascript front-end
```

Z GitHub CLI (`gh`) to samo jedną komendą:

```bash
gh repo edit DamTchorzewski/WebStudio --homepage "https://damtchorzewski.github.io/WebStudio/" --description "Responsive two-page site of a web agency: home with offer, team, skills and clients, and a portfolio page with nine projects. Semantic HTML5, BEM, SASS, mobile-first with x1/x2/x3 images, mobile menu and modal. Hosted on GitHub Pages." --add-topic html5,css3,sass,scss,bem,responsive-design,mobile-first,portfolio-website,landing-page,github-pages,javascript,front-end
```

## Ustawienia do włączenia

| Gdzie (GitHub)                                          | Co ustawić                                           |
| ------------------------------------------------------- | ---------------------------------------------------- |
| Settings → Pages                                        | źródło: gałąź `main`, folder `/ (root)` (już działa) |
| Settings → General → Default branch                     | `main` (już jest)                                    |
| Settings → Branches (albo Rulesets) → `main`, `develop` | zablokuj force push i usuwanie gałęzi                |
