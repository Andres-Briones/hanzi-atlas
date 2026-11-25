# Hanzi Atlas

A static site to explore the 3,500 most common Chinese characters: how each one is built
(decomposition tree drawn from its own strokes), where it comes from, its sound and meaning parts,
a short pet name, the words it appears in, and example sentences.

No build step and no server code: `index.html` plus JSON files under `data/`.

## Publish on GitHub Pages

1. Create an empty repository on GitHub and push this folder to it:
   `git remote add origin git@github.com:<you>/<repo>.git && git push -u origin main`
2. In the repository: Settings → Pages → Source "Deploy from a branch", branch `main`, folder `/ (root)`.
3. The site appears at `https://<you>.github.io/<repo>/` after a minute. All links are relative, so it
   works under that sub-path. `.nojekyll` tells GitHub to serve the files as they are.

To look at it locally: `python3 -m http.server` in this folder, then open http://localhost:8000.

## Where the content comes from

See [NOTICE.md](NOTICE.md) for sources and licences. The origin notes and names were written with
AI assistance from the cited sources; each note states its confidence. Treat them as a starting point.
