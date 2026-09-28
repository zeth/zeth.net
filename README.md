# zeth.net

The website for **Zeth Ltd**, an independent UK software engineering company.
It is a plain [Jekyll](https://jekyllrb.com/) site that uses the `github-pages`
gem, so local builds match GitHub Pages.

## Setup

You need Ruby (3.x), Bundler and a C compiler with the Ruby development headers
(on Ubuntu: `sudo apt install ruby-full build-essential`).

```bash
bundle config set --local path vendor/bundle   # optional: keep gems inside the project
bundle install
```

## Local preview

```bash
bundle exec jekyll serve --livereload
# Open http://127.0.0.1:4000/
```

If port 4000 is already in use (for example by another Jekyll site), choose
different ports:

```bash
bundle exec jekyll serve --livereload --port 4001 --livereload-port 35730
```

## Production-style build

```bash
bundle exec jekyll build      # output in _site/
```

The warning about `faraday-retry` comes from the `github-pages` gem and is harmless.

## Editing

| What | Where |
|---|---|
| Company facts, email, GitHub links, Holder links | `_data/company.yml` |
| Main navigation | `_data/navigation.yml` |
| Site title, description, production URL | `_config.yml` |
| Homepage | `index.html` |
| Other pages | `services/`, `work/`, `open-source/`, `about/`, `contact/`, `company/`, `legal/` (Markdown) |
| Shared layout, header, footer | `_layouts/`, `_includes/` |
| Styles | `assets/css/main.scss` (colour tokens at the top) |
| Images | `assets/images/` |

**Placeholders.** Any empty value in `_data/company.yml` is shown on the site as
a highlighted **To confirm** marker, and editorial gaps in the page copy use
`{% include placeholder.html text="…" %}`. Before publication, search for
remaining placeholders:

```bash
grep -rn "placeholder.html" --include=*.md --include=*.html . | grep -v _includes
```

The business email address is set once in `_data/company.yml` (`email:`); every
contact button and `mailto:` link on the site uses it.

The Holder screenshot (`assets/images/holder-desktop.jpg`) is copied from the
holder-website repository. The Holder panel is in `_includes/holder-slot.html`.

The original photos in `images/` are not published (excluded in `_config.yml`);
web-sized, metadata-stripped copies are in `assets/images/`.

## To confirm before publication

- [ ] **Business email address**: `email` in `_data/company.yml`.
- [ ] **Registered office**: `_data/company.yml`.
- [ ] **VAT number**, if registered (set `show_vat: true`).
- [ ] **Contract Engineering**: specific technologies, experience summary, location, terms and availability.
- [ ] **About**: introductions to Zeth and Jutta, Zeth's professional background, open-source and community involvement.
- [ ] **Open Source**: any other projects or contributions.
- [ ] **Work**: client or contract work (only with the client's permission), or remove that section.
- [ ] **Holder**: check the "shared C/C++ core" description and the release details on the Work page are current.
- [ ] **Company page**: which apps, if any, are published under Zeth Ltd's name.
- [ ] **Privacy notice** (`legal/privacy.md`): write it from the facts, then have it reviewed.
- [ ] **Holder privacy** (`legal/holder/privacy.md`): holder.team already has a privacy policy. Decide whether to link to it, mirror it or remove this page.
- [ ] **Photos**: approve the portrait (homepage, About) and the photo of Zeth and Jutta (About).
