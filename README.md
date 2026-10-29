# Anub8x

Personal site of **Anub8te** — aspiring exploit developer (exploit development and reverse engineering). Built with [Hugo](https://gohugo.io/) and deployed to GitHub Pages at <https://anub8te.github.io/>.

## Structure

```
anub8te.github.io/
├── .github/workflows/hugo.yaml   # build, verify, deploy to Pages
├── archetypes/                   # template for `hugo new post/...`
├── content/
│   ├── about.md                  # About page
│   ├── cves/                     # disclosures section
│   ├── post/                     # logbook entries
│   ├── archives/  search.md      # archive and search pages
├── data/                         # about, team, friends, cves, advisories (TOML)
├── docs/                         # design, fonts, editing and publishing notes
├── scripts/verify.py             # post-build checks (links, feed, search index)
├── static/                       # avatar, images, fonts, favicon
├── themes/after-hours/           # layouts, CSS, JS
├── hugo.toml                     # site configuration
├── LICENSE  NOTICE.md
└── README.md
```

## Local development

Requires Hugo Extended 0.154.5 or newer.

```bash
hugo server            # live preview at http://localhost:1313
hugo --gc --minify     # production build into public/
python3 scripts/verify.py public
```

## Writing a post

```bash
hugo new post/my-post.md
```

Fill in the front matter, write the entry, set `draft = false`, then push to `main`. See [docs/PUBLISHING.md](docs/PUBLISHING.md).

## Deployment

Pushing to `main` runs the GitHub Actions workflow, which builds the site, runs `scripts/verify.py`, and publishes to Pages. In the repository settings, set **Pages → Source** to **GitHub Actions**.

## Changing the avatar

Replace `static/avatar/avatar.jpg` (square image, 640×640 recommended), commit, and push. If the old image still shows, hard-refresh the browser.

## License

MIT — see [LICENSE](LICENSE) and [NOTICE.md](NOTICE.md).
