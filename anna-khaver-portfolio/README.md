# Anna Khaver – Portfolio

A static portfolio site: plain HTML, CSS and a little vanilla JavaScript.
No build step, no dependencies, no framework.

## Structure

```
index.html                       Home: hero, about & experience, case study cards, toolkit, contact
case-studies/
  filter-discovery.html          Pipedrive – Filter discovery experiment
  referral-program.html          Pipedrive – Referral program redesign
  conrad-seller-onboarding.html  Conrad Marketplace – Seller onboarding
assets/img/                      All images: product screens, portrait, hand-drawn letters and stars, card previews
```

All links between pages and to images are **relative**, so the site works from a folder on your computer,
from a local server, or from GitHub Pages under a sub-path (`https://<user>.github.io/<repo>/`).

## Run locally

Open `index.html` in a browser. It works straight from the file system.
Or run a tiny server: `python3 -m http.server 8000` and visit http://localhost:8000.

## Publish on GitHub Pages

1. Push this folder to a GitHub repository.
2. Settings → Pages → *Deploy from a branch* → branch `main`, folder `/ (root)`.
3. Your site appears at `https://<user>.github.io/<repo>/`.

## Editing

- **Case study cards and filters:** the `PROJECTS` array near the bottom of `index.html`
  (title, text, tags, preview image `img`, page `go`, and the filter badges in `cats`).
- **Case study pages:** each file in `case-studies/` is self-contained. Styling is repeated in each file on purpose,
  so a page keeps working on its own.
- **Images:** replace files in `assets/img/` (keep the file names, or update the references).

## Notes

- **Fonts:** Inter is loaded from Google Fonts, so it needs an internet connection. Without it the site falls back to
  the system sans-serif. To self-host, download Inter, put the files in `assets/fonts/` and add `@font-face` rules.
- **External links:** LinkedIn, Instagram, the full CV (Google Doc) and the Figma prototype open in a new tab.
  The Google Doc and the Figma file must be shared as "anyone with the link" for visitors to open them.
- **Dark mode:** the pages follow the visitor's system theme.
- **Before making the repository public:** the case studies include screens and numbers from Pipedrive and Conrad work.
  Check that you are allowed to publish them.
