# Partita website

The website for Partita, a suite of small Windows audio apps:

| App | What it does | Code name | Status |
| --- | --- | --- | --- |
| Divisi | Routes every app to any output, or several, from one grid | WaveMatrix | Beta |
| Tacet | Removes noise and echo from your mic | MicClean | Free download (v0.10.0) |
| Giusto | Headphone app | | Coming soon |

Each name is a marking from sheet music: a partita is a suite for one instrument, *divisi*
splits a section, *tacet* tells a player to stay silent, and *giusto* means exactly right.

Plain HTML and CSS, no build step:

```
index.html          home page, the suite and "Coming soon" for Giusto
divisi/index.html   Divisi landing page
tacet/index.html    Tacet landing page
style.css           shared styles; each page picks its accent with a body class
favicon.svg         the logo
```

## Preview

```
python -m http.server 8137
```

Then open http://localhost:8137. Links are relative, so the site also works from a GitHub Pages
project URL.

## Before going live

- Replace `contact@example.com` (every page) with your real email.
- Divisi's pricing (Free / $15 Pro, $10 launch week, 14-day refund) is the launch plan, not yet
  built into the app. Change it on `divisi/index.html` if the plan changes.
- Tacet's download points at the `TooCoolCello/micclean` GitHub release, which still installs
  under the name MicClean.
