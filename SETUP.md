# Deploying Your GitHub Profile README (`AadiSharma1/AadiSharma1`)

## 1. Preview Locally First
Unzip this archive and double-click `preview.html` in Chrome, Edge, or Firefox to see all 11 bespoke animated SVGs running live in GitHub Dark layout.

## 2. Push to Your GitHub Profile Repo
1. Go to GitHub and make sure you have a **public** repository named exactly **`AadiSharma1`** (matching your GitHub username).
2. Copy `README.md` and the entire `assets/` folder into the root of that repo:
   ```text
   AadiSharma1/
   ├── README.md
   └── assets/
       ├── hero-banner.svg
       ├── divider-pulse.svg
       ├── research-matrix.svg
       ├── projects-showcase.svg
       ├── stack-architecture.svg
       ├── activity-waveform.svg
       ├── footer-terminal.svg
       ├── btn-portfolio.svg
       ├── btn-linkedin.svg
       ├── btn-orcid.svg
       └── btn-email.svg
   ```
3. Commit and push to `main`:
   ```bash
   git add README.md assets/
   git commit -m "feat: custom animated telemetry profile README"
   git push origin main
   ```

## 3. Update Individual Repo Links (Optional)
In `README.md`, under `DIRECT REPOSITORIES:`, swap each `https://github.com/AadiSharma1` link to the exact repository slug (e.g., `https://github.com/AadiSharma1/VORTEX-GNC`) once those repos are public.

## Why Every Animation Works Reliably on GitHub
- **Zero JavaScript / Zero External Fonts:** GitHub renders SVGs inside sandboxed `<img>` tags that strip `<script>` and block Google Fonts. Every animation here uses pure CSS `@keyframes` + native SMIL (`<animate>`, `<animateTransform>`, `<animateMotion>`), and the hero `AADI SHARMA` wordmark is built from pure custom geometric `<path>` geometry so it renders identically on every OS.
- **Zero Third-Party Outages:** Because all SVGs live inside your own `assets/` folder, your profile never breaks with Vercel 503 errors.
