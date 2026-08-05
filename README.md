# pyweblib.org

The landing page for [PyWebLib](https://github.com/SebastianHagemeyer/PyWebLib).
One static page, no build step, no dependencies.

| | |
| --- | --- |
| **This repo** | `pyweblib.org` - the front door |
| **The app** | `play.pyweblib.org` - playground, docs, community, assets, leaderboards ([PyWebLib repo](https://github.com/SebastianHagemeyer/PyWebLib)) |

Kept separate because GitHub Pages allows one custom domain per repo, and the
app is a much larger thing that deploys on its own schedule. Every link out of
this page points at `play.pyweblib.org`.

## Local preview

```
python -m http.server 8000
```

Then open http://localhost:8000. Nothing else to run.

## Deploying

GitHub Pages, from `main`. The `CNAME` file holds `pyweblib.org`; changing it
changes the domain Pages serves this on.

DNS lives at NameSilo. The apex needs GitHub's four A records, and `www` is a
CNAME to `sebastianhagemeyer.github.io`.

## Brand

Design tokens in `styles.css` are copied from the app's stylesheet so the two
read as one product. If you change a colour there, change it here too. Icons
and `logo.svg` are copies of the app's, kept local so this page loads nothing
from another origin.
