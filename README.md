# Mohammed Qasem — Sports Portfolio

A responsive, bilingual (English / Arabic) sports portfolio for Mohammed Qasem, based on the provided English and Arabic CVs.

## Features

- Bold athletic dark-green and lime aesthetic
- Fully responsive desktop and mobile layouts
- English / Arabic language toggle with RTL support
- About, career metrics, experience, specialties, photo gallery, credentials, contact
- Downloadable English and Arabic CVs
- No framework or build tools required: HTML + CSS + vanilla JavaScript

## Local preview

Open `index.html` in a browser, or from the project directory run:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

## Add photographs

1. Put actual photos in the `assets/` directory, for example `assets/coach.jpg`, `assets/training.jpg`, `assets/match.jpg`, `assets/team.jpg`, `assets/fitness.jpg`.
2. Open `script.js` and update the `portfolioImages` object at the bottom:

```js
const portfolioImages = {
  hero: 'assets/coach.jpg',
  training: 'assets/training.jpg',
  match: 'assets/match.jpg',
  team: 'assets/team.jpg',
  fitness: 'assets/fitness.jpg'
};
```

3. Refresh the page. Photos fill the placeholders automatically.

## Change content

Edit the `translations.en` / `translations.ar` objects in `script.js` to change any text. The two supplied PDFs are in `cv/`.

## Publish on GitHub Pages

1. Create a **public** GitHub repository named `mohammed-qasem-portfolio` under the GitHub account where you want the site hosted.
2. Upload all contents of this project to the repository root (including the `assets/` and `cv/` directories).
3. In the repository select **Settings → Pages → Build and deployment → Deploy from a branch**.
4. Select **main**, root `/`, and save.
5. The website should become available at `https://YOUR-USERNAME.github.io/mohammed-qasem-portfolio/` after GitHub Pages builds successfully.

**Privacy note:** This project displays the phone number included in the supplied CVs. If that should not be public, change the phone number in `index.html` before publishing and replace the public CV copies.

## Accuracy

Experience, qualifications and metrics are based on the supplied CVs; no fabricated awards, photography, contact emails, or testimonials were added.