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
- Pricing is the launch plan, not yet built into the apps: $15 per app ($10 in its launch week),
  $20 for the Partita bundle (all three, Giusto when it ships), 14-day refund, and Divisi's free
  tier (up to 3 apps). It appears on all three pages; change them together.
- The buy buttons point at the beta or an email until a store (Gumroad, Lemon Squeezy) is set up.
- Tacet's download points at the `TooCoolCello/micclean` GitHub release, which still installs
  under the name MicClean.
