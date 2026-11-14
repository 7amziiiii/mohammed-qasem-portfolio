# Mohammed Qasem — Sports Portfolio

A responsive, bilingual (English / Arabic) sports portfolio for Mohammed Qasem, based on the provided English and Arabic CVs.

## Features

- Bold athletic dark-green and lime aesthetic
- Fully responsive desktop and mobile layouts
- English / Arabic language toggle with RTL support
- About, career metrics, experience, specialties, photo gallery, credentials, contact
- English and Arabic print-ready CV pages (Print / Save as PDF)
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

Edit the `translations.en` / `translations.ar` objects in `script.js` to change any text. The CV pages are in `cv/english.html` and `cv/arabic.html`. Each provides a Print / Save as PDF button. The original PDFs remain in the downloadable project archive, but are not part of this GitHub source repository.

## Publish on GitHub Pages

1. Change the repository visibility to **Public** under Settings → General → Danger Zone if your GitHub plan does not support Pages for private repositories.
2. The included `.github/workflows/deploy.yml` workflow deploys the website automatically after pushes to `main`.
3. If Pages is not activated, open Settings → Pages and set the build source to **GitHub Actions**, then manually run the Deploy portfolio workflow in Actions.
4. The website URL is `https://7amziiiii.github.io/mohammed-qasem-portfolio/` once the workflow finishes successfully.

**Privacy note:** This project displays the phone number included in the supplied CVs. If that should not be public, change the phone number in `index.html` before publishing and replace the public CV copies.

## Accuracy

Experience, qualifications and metrics are based on the supplied CVs; no fabricated awards, photography, contact emails, or testimonials were added.