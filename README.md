<div align="center">

# Thanga Paresh T

### AWS DevOps Enthusiast · MERN Stack · Vibe Coding

<img src="./hero.svg?v=1" alt="Animated profile hero" width="100%">

</div>

## About me

- 📍 Nagercoil, India
- 🏢 JCS Infotech
- ☁️ Exploring AWS, DevOps and cloud-native workflows
- 🧩 Building with the MERN stack
- 🎧 Hobby: vibe coding — experimenting, prototyping and shipping ideas

<img src="./about-life.svg?v=1" alt="About and interests" width="100%">

## Tech stack

<img src="./stack.svg?v=1" alt="Animated technology orbit and skill chips" width="100%">

## Developer dashboard

<img src="./id-dashboard.svg?v=1" alt="Developer ID and animated dashboard" width="100%">

> Dashboard values are illustrative design placeholders, not live GitHub statistics. Replace them with verified repository metrics before publishing.

## Featured projects

| Project | What it does | Stack |
|---|---|---|
| **MERN Portfolio** | Responsive portfolio and project showcase | React, Vite, Tailwind CSS |
| **Cloud & DevOps Lab** | Deployment, automation and infrastructure experiments | AWS, Docker, CI/CD |
| **Full-stack CRUD App** | REST API with data persistence and role-based flows | Node.js, Express, MongoDB |
| **UI Motion Experiments** | Small interfaces exploring gradients, SVG and CSS motion | CSS, SVG, React |

Replace these example rows with links to your actual repositories.

## Connect

<img src="./connect.svg?v=1" alt="Connect with Thanga Paresh" width="100%">

- GitHub: [@thangaparesh-dev](https://github.com/thangaparesh-dev)
- Email: [thangaparesh028@gmail.com](mailto:thangaparesh028@gmail.com)
- Company: JCS Infotech
- Location: Nagercoil, India

---

## Daily 3D contribution city with GitHub Actions

Save this as `.github/workflows/profile-3d.yml` in your profile repository. It uses [yoshi389111/github-profile-3d-contrib](https://github.com/yoshi389111/github-profile-3d-contrib).

```yaml
name: Generate 3D contribution city

on:
  schedule:
    - cron: "17 0 * * *"
  workflow_dispatch:

permissions:
  contents: write

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: yoshi389111/github-profile-3d-contrib@latest
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
          USERNAME: thangaparesh-dev
      - name: Commit generated visuals
        run: |
          git config user.name "github-actions[bot]"
          git config user.email "41898282+github-actions[bot]@users.noreply.github.com"
          git add -A
          git diff --cached --quiet || git commit -m "chore: refresh 3D contribution profile"
          git push
```

After the workflow runs, confirm the exact generated filenames in the repository and add the night-view SVG, for example:

```md
<img src="./profile-3d-contrib/profile-night-rainbow.svg?v=1" alt="3D contribution city" width="100%">
```

Use the actual output path from the action version you pin. For reproducibility, replace `@latest` with a reviewed release tag or commit SHA.

## Compatibility notes

- All five SVG cards are self-contained and embed their image assets as base64 PNGs. No remote image/font assets are requested.
- Animation uses CSS and SVG SMIL only; no JavaScript is included.
- The supplied attachments did not include the waving video. `hero.svg` uses the supplied developer illustration as a still-image fallback with animated viewfinder elements. Once you provide the clip, its frames can replace the fallback.
- WOFF2 font files were not supplied, so these files use system font fallbacks rather than claiming to embed base64 fonts.
- GitHub sanitizes SVGs and may handle CSS/SMIL animation differently from a full browser. Preview the cards in a modern browser as well as on GitHub.
