# Installing on Moodle H5P v1.28

Use `css/units-h5p-global.css` as the custom CSS payload for H5P.

## Preferred path

1. Open the Moodle/H5P custom CSS configuration used by the site.
2. Paste or reference the contents of `css/units-h5p-global.css`.
3. Purge Moodle caches.
4. Open an H5P Interactive Book activity and confirm that text, accordion, quiz, dialog cards, audio recorder, hotspot, and table components inherit the UNITS styling.

## Notes

- This stylesheet is global. It does not target a specific cmid or course.
- The original `cmid-26` loader applied JavaScript-driven page backgrounds. Pure CSS cannot reliably map an Interactive Book page title to a background image, so this CSS keeps the color, typography, spacing, panel, and component styling only.
- The CSS imports Google Fonts. If the Moodle site blocks external font loading, remove the `@import` lines and keep the fallback font stack.
- If Moodle/H5P strips `@import`, load the fonts from the Moodle theme instead.

## Rollback

Remove the CSS from the H5P custom CSS field or stop referencing the file, then purge Moodle caches.
