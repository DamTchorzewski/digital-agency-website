<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="docs/images/banner-dark.png">
    <img src="docs/images/banner-light.png" alt="WebStudio: website of a web agency" width="100%">
  </picture>
</p>

<p align="center">
  <img src="docs/images/showcase.jpg" alt="WebStudio on desktop and on a phone" width="100%">
</p>

## About

<a href="https://damtchorzewski.github.io/digital-agency-website/"><img src="docs/images/open-site.png" alt="Open the live site" width="130"></a>

**WebStudio** is a two-page, responsive site of a fictional web agency, built as a front-end exercise: a home page
that presents the offer, the team, the skills and the clients, and a portfolio page with nine sample projects. It
is plain HTML, SASS-compiled CSS and a little JavaScript, with no build step in the repository.

- **Semantic HTML5.** `index.html` (hero banner with a contact modal, "what we do", team, skills, clients, footer
  with a newsletter form and social links) and `portfolio.html`.
- **BEM and SASS.** Styles follow the BEM methodology; the sources are in `sass/` (components and utilities) and are
  compiled to minified CSS with source maps in `css/`.
- **Mobile-first.** Media queries adjust the layout at 480 px, 768 px and 1200 px.
- **Mobile menu and modal.** A burger menu (`js/mobile-menu.js`, with `body-scroll-lock` from a CDN) and a
  contact modal (`js/modal.js`).
- **Responsive images.** Background and content images come in `@1x`, `@2x` and `@3x` variants per breakpoint.
- **Portfolio.** Nine projects as cards with an image, a name and a category, and a row of category buttons.

> **Status:** a finished exercise with placeholder content: the team members are "John Doe" and the skill cards
> hold Lorem ipsum. The category buttons on the portfolio page are markup only: no script filters the cards yet.

## Tech stack

|          |                                                                                              |
| -------- | -------------------------------------------------------------------------------------------- |
| Stack    | HTML5, SASS (compiled to `css/*.min.css`), vanilla JavaScript; no framework, no bundler      |
| UI       | BEM, mobile-first, `modern-normalize` and Google Fonts from CDNs                             |
| Tests    | none                                                                                         |
| Hosting  | GitHub Pages                                                                                 |

The page content is in Polish; the README, commits and branches are in English.

## Screenshots

<p align="center">
  <img src="docs/images/pages.jpg" alt="Team and portfolio sections on desktop" width="100%">
</p>
<p align="center">
  <img src="docs/images/mobile.jpg" alt="Mobile: home, offer, team and portfolio" width="100%">
</p>

## Quick start

```bash
git clone https://github.com/DamTchorzewski/digital-agency-website.git
cd digital-agency-website
npx serve .      # or open index.html in a browser
```

Requirements: none to view the site (open `index.html`); Node.js is only needed for the optional `npx serve`. To
change the styles, edit `sass/` and compile it to `css/` with the *Live Sass Compiler* extension of VS Code (the
settings are in `.vscode/settings.json`) or the `sass` command line.

## Scripts

There is no `package.json` scripts section (the repository has only an empty `package-lock.json`). One command
rebuilds the CSS, if you have the Sass CLI:

| Command                                                                                  | What it does                                  |
| ---------------------------------------------------------------------------------------- | --------------------------------------------- |
| `sass --style=compressed sass/main.scss css/main.min.css`                                | compile the home page styles                  |
| `sass --style=compressed sass/portfolio.scss css/portfolio.min.css`                      | compile the portfolio page styles             |

## Configuration

None: no environment variables, keys or settings; the newsletter form and the contact modal are front-end only.

## Structure

```
index.html            ★ home page
portfolio.html        ★ portfolio page
sass/                 main.scss, portfolio.scss, components/ (header, menu, banner, team, skills, clients, modal...), utils/
css/                  compiled and minified styles with source maps (generated from sass/)
js/                   mobile-menu.js, modal.js
images/               site images in @1x / @2x / @3x variants
docs/                 documentation; docs/images/ holds the README images (generated)
.vscode/              Live Sass Compiler settings
```

## Branches and workflows

Shared standards from `reops/standards`: `main` ≤ `develop` ≤ a working branch `<type>/<topic>`, fast-forward
merges, Conventional Commits in English. The repository has no workflows: GitHub Pages serves the files as they are.

**Departures from the standards (and why):**

- **No build, hooks, tests or CI:** a static course exercise; the compiled CSS is committed because Pages serves
  the repository directly.
- **README images** are made by `tools/readme-images` (profile `digital-agency-website`) from the live site; the logo is the site's
  own wordmark.
- **Page content in Polish.**

## Documentation

| Document                                   | Covers                          |
| ------------------------------------------ | ------------------------------- |
| [docs/repository.md](docs/repository.md)   | GitHub description and topics   |

The README images (`docs/images/`) are regenerated with `tools/readme-images`, profile `digital-agency-website`; the working shots go
to `.scratch/`.

---

<p align="center"><a href="https://damreboot.pl"><picture><source media="(prefers-color-scheme: dark)" srcset="docs/images/damreboot/company-dark.svg"><img src="docs/images/damreboot/company-light.svg" alt="damreboot.pl: company website" height="36"></picture></a><a href="https://www.linkedin.com/in/damian-tchorzewski-3b2388275/"><picture><source media="(prefers-color-scheme: dark)" srcset="docs/images/damreboot/linkedin-dark.svg"><img src="docs/images/damreboot/linkedin-light.svg" alt="LinkedIn: let's connect" height="36"></picture></a><a href="mailto:damianchabracki@gmail.com"><picture><source media="(prefers-color-scheme: dark)" srcset="docs/images/damreboot/email-dark.svg"><img src="docs/images/damreboot/email-light.svg" alt="E-mail: write to me" height="36"></picture></a></p>

<p align="center">
  <picture><source media="(prefers-color-scheme: dark)" srcset="docs/images/damreboot/engineered-dark.svg"><img src="docs/images/damreboot/engineered-light.svg" alt="" height="33" align="middle"></picture> Engineered by <b>Damian Chabracki</b> (DamReboot IT)
</p>
