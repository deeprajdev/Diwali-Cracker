# Diwali Crackers AR

Light virtual Diwali crackers over your phone or laptop camera. Plain HTML, CSS and JavaScript: one `index.html` plus an `assets/` folder. No build step, no dependencies.

**Live:** https://diwali-crackers-ar.vercel.app

## How to use

1. Press **Begin** and allow camera access (or choose **Continue without camera**).
2. **Tap** (or click) anywhere to light the selected cracker where you pressed.
3. Pick a cracker from the bar at the bottom.
4. Use the top buttons to take a photo, record a video (with sound), flip the camera, toggle music and sound, and open settings.

A short step-by-step guide opens on the first visit. Press the **?** button (or `H`) to open it again.

| Cracker | What it does |
| --- | --- |
| Mix | A random cracker from the range |
| Anaar | Fountain of sparks and tall flame |
| Chakri | Spins on the ground, flames shoot outward |
| Rocket | Climbs high, then bursts |
| Spark | Phooljhari: press and drag to draw with sparks |
| Ladi | A long string of crackers |
| Sutli | Jute bomb with a big blast |

**Keyboard (computer):** `1`–`7` pick a cracker, `M` toggles music, `H` or `?` opens the guide, `Esc` closes menus.

**Settings:** Night mode, Glow boost, Soft flashes, Pin to surroundings.

## Run it locally

The camera needs a secure context, so open it over `localhost` rather than `file://`:

```bash
git clone https://github.com/deeprajdev/Diwali-Cracker.git
cd Diwali-Cracker
python3 -m http.server 8000
```

Then open http://localhost:8000. To try it on a phone, deploy it (see below) and open the HTTPS link, since phones only allow the camera on HTTPS.

## Deploy

It is a static site, so any static host works. On Vercel: import the repo, leave the framework as **Other**, and leave the build and output settings empty. Vercel Web Analytics is already included in `index.html`; turn it on in the project's Analytics tab.

## Files

- `index.html`: the whole app (layout, effects, sound, guide)
- `assets/`: cracker photos (`anaar`, `chakri`, `sutli`, `ladi`, `rocket` as `.webp`) and `diwali.mp3`
