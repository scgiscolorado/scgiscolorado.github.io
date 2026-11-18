# SCGIS Colorado website

Website for the Colorado chapter of the Society for Conservation GIS.
Modeled on the SCGIS DC chapter site (https://scgis-chapters.github.io/dc/).

Static HTML and CSS, hosted with GitHub Pages. No build step.

## Structure

- `index.html` - all page content
- `assets/css/styles.css` - layout, colors, typography
- `assets/images/` - logo and photos
- `assets/js/header.js` - mobile header behavior
- `.nojekyll` - serve the files as-is

## Common updates (all in `index.html`)

- **Next event**: edit the banner near the top (`survey-announcement`), the
  `event-highlight` block in the Events section, and the first card in
  Chapter Updates.
- **Calendar**: the Google Calendar `<iframe>` in the Events section shows
  the calendar for scgis_colorado_chapter@scgis.org as a list of upcoming
  events (`mode=AGENDA` in the address; remove it to show a month grid). That calendar must be
  set to "Make available to public" in Google Calendar settings, or visitors
  will see an empty calendar.
- **ListServe**: the button currently opens an email to the chapter. When a
  Google Group exists, replace the button's `href` with the group address.
- **Chapter leads**: each lead is a `lead-card` block with a photo, name,
  and LinkedIn link (put photos in `assets/images/`).
- **Resources**: each link is a `resource-card` block.

## Publish

Push to `main`, then in the repository go to Settings > Pages and set the
source to "Deploy from a branch", branch `main`, folder `/ (root)`. The site
appears at https://scgiscolorado.github.io/ after a few minutes.

## Image credits

- Hero photos: chapter photo (`hero-bandana.jpg`) fading into the 2026 SCGIS
  Conference group photo. To change them, swap the two images inside
  `hero-media` in `index.html`.
- SCGIS logo and conference photo: SCGIS.
