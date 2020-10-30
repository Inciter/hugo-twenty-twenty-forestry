# Inciter Hugo Theme and Site

## CSS
We are using SASS and Tailwind with PostCSS as part of the site build process.  Currently the SASS styles are broken into 4 files:
- icons.scss (the style for our icon usage)
- blocks.scss (the styles for block elements and blocks of content.  Usually related to spacing, sizing, etc.)
- responsive.scss (styles related to different screen size presentation, mostly padding/margin/display types)
- typography.scss (styles related to font presentation and colors)

Also, in typical tailwind fashion, we can override styles/introduce new styles in assets/css/tailwind.config.js.

Full documentation for TailwindCSS can be found [here](https://tailwindcss.com/docs/installation)

## Icons
We use SVG icons from FontAwesome, however, we do not load the entire font awesome library/CSS/JS for purposes of performance.  Instead, we have the svg icons we use downloaded to the `fontawesome` folder in the repository's root, and we use the `fontawesome.html` partial to render icons by name (matching their file name).

### Adding a new icon
Simply download the SVG for the icon you wish to use from FontAwesome's repository, and save it in the `fontawesome` folder.  After that is committed, you can reference that icon using the `fontawesome` partial by using the icon name/svg file name.

Ex.

You downloaded a new icon with a filename of 'awesome-icon.svg'.  Anywhere that we use icon names in the Hugo blocks, you can reference this icon by the name 'awesome-icon' and it will work.  Using it in the partial in a template would look like: `{{ partial "fontawesome.html" "awesome-icon" }}`