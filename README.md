# FlowerSpot Events website

Static site (HTML + Tailwind + GSAP). No build step.

## Deploy on GitHub Pages
1. Create a new GitHub repository (for example `flowerspot-events`).
2. Upload everything in this folder to the repository root (index.html must be at the root), or push with Git:
       git init
       git add .
       git commit -m "FlowerSpot Events site"
       git branch -M main
       git remote add origin https://github.com/YOUR-USERNAME/flowerspot-events.git
       git push -u origin main
3. On GitHub open Settings, then Pages. Under Source choose "Deploy from a branch", branch `main`, folder `/ (root)`, and Save.
4. After a minute the site is live at https://YOUR-USERNAME.github.io/flowerspot-events/

## Tests
Run on every push by .github/workflows/tests.yml. To run locally:
    pip install -r requirements.txt
    playwright install chromium
    ./run_tests.sh

## Notes
- Needs internet for Tailwind, GSAP and Google Fonts (loaded from CDNs).
- Quote form opens WhatsApp +91 80984 15066 (search 918098415066 in index.html to change).
- Replace assets/hero.mp4 to change the hero video (keep the same file name).
