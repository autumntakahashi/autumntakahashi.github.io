# Personal site (Jekyll + GitHub Pages)

## Go live
1. Create a public GitHub repo named `yourusername.github.io`.
2. Edit `_config.yml`: set `title`, `email`, `github_username`, and `url`.
3. Upload these files to the repo (or `git push` them).
4. Repo Settings > Pages > Deploy from a branch > `main` / root.
5. Wait a minute or two, then visit `https://yourusername.github.io`.

## Where things go
| What | Where |
|---|---|
| Home page text | `index.md` |
| Papers and projects | `_data/publications.yml` (PDFs in `assets/papers/`) |
| Artwork | add an image to `assets/art/`, then an entry in `_data/art.yml` |
| Articles | new file in `_posts/` named `YYYY-MM-DD-title.md` |
| Colors and fonts | top of `assets/css/main.css` |

## Equations
Use double dollar signs for both inline and display math:

    Inline: $$x_i^2$$
    Display:
    $$
    \int_0^1 x\,dx = \tfrac12
    $$

## Preview locally (optional)
    bundle install
    bundle exec jekyll serve
Then open http://localhost:4000.

## Custom domain later
Settings > Pages > Custom domain, add a DNS record at your registrar,
and change `url` in `_config.yml`.
