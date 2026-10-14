# otium.quest

The Otium landing page: the name, the tagline, and the beta signup form.

Public **only** so free static hosting can deploy it — Vercel's Hobby plan refuses
private organization repos, and GitHub Pages needs a paid plan for private ones. The app
itself lives in the private `getotiumapp/otium_app` repo.

Nothing here is sensitive: static HTML, two open-licence font files, and a link to a
Google Form that is already public.

## Editing

One file, `index.html`, no build step. Open it directly in a browser to preview.

The signup form is an iframe, and Google Forms is cross-origin — it cannot report its own
height, so the heights in the CSS are measured by hand. Narrow viewports need a *taller*
frame, because fields wrap as the frame gets narrower.

The source of truth for this page is `web/` in the app repo; changes are copied here.
