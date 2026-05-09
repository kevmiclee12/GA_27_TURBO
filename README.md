# GA '27 Turbo

A pseudo-3D synthwave arcade racer starring Ron, the iConnections CEO, racing
his motorcycle to **Global Alts Miami** through neon Miami nights. Collect
Sponsors, Fund Managers, Allocators, and AI Boost charges. Dodge phishing
emails, platform outages, and snowstorms. Beat Apexion and Konnexxt to the
finish line.

[Play in your browser](https://kevmiclee12.github.io/GA_27_TURBO/)

## Controls

- **← →** Steer
- **↑** Accelerate (the closer you press it to **GO!**, the faster you start)
- **↓** Brake
- **SPACE** Trigger AI Boost charge

## Project structure

```
index.html             Single-file game (HTML, CSS, Web Audio synth, Canvas)
assets/icon_logo.svg   iConnections logo used on the Welcome to Miami screen
```

No build step, no dependencies, no server-side code. Every visual, sound, and
game-loop tick lives inside `index.html`.

## Local development

Just open `index.html` in any modern browser. If you want a local server (e.g.
to test relative paths exactly as GitHub Pages serves them):

```sh
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploying to GitHub Pages

This repo is configured to deploy from the `main` branch root.

1. Push `main` to GitHub.
2. In the repo on github.com, go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to *Deploy from a branch*,
   **Branch** to `main`, and folder to `/ (root)`.
4. Save. After a minute or two the site is live at
   `https://<your-username>.github.io/GA_27_TURBO/`.

Any subsequent `git push` to `main` redeploys automatically.
