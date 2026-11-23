# Folly Consulting website

A Jekyll site for GitHub Pages, styled with the Folly Consulting style guide
(Spruce / Fir / Lichen / Bark Brown, Fraunces + DM Sans, pine-ridge logo).

## Publish on GitHub Pages
1. Create a GitHub repo (name it `USERNAME.github.io` for a user site, or any name for a project site).
2. Upload these files to the `main` branch.
3. Repo **Settings > Pages**: Source = *Deploy from a branch*, Branch = `main`, folder = `/ (root)`.
4. Project site only: set `baseurl: "/repo-name"` in `_config.yml`.
5. Custom domain: add `follyconsulting.com` under Settings > Pages, point your DNS at GitHub Pages, then tick *Enforce HTTPS*.

## Run locally (optional)
```
bundle install
bundle exec jekyll serve
```
Open http://localhost:4000

## Where things live
| To change | Edit |
|---|---|
| Phone, email, tagline | `_data/company.yml` |
| Menu links | `_data/navigation.yml` |
| Services list | `_data/services.yml` |
| Pages | `index.html`, `services.md`, `about.md`, `contact.md` |
| Colours, fonts, spacing | `assets/css/style.css` (variables at the top) |
| Logo | `assets/img/logo-mark.png` (transparent; recolours via CSS) |

Add a page: create `name.md` with `layout: page`, a `title`, and a `permalink`, then add it to `navigation.yml`.
