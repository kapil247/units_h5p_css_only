# UNITS H5P CSS Only

Global custom CSS for the UNITS H5P activities on Moodle H5P framework v1.28 (`h5plib_v128`).

This repository converts the earlier `cmid-26` JavaScript-driven customization into a plain CSS package that can be loaded globally through the H5P custom CSS mechanism.

## Files

- `css/units-h5p-global.css` - production CSS to load in H5P.
- `docs/install-h5p-v128.md` - installation notes for Moodle/H5P v1.28.

## Scope

This is option 1: one global H5P stylesheet. Once loaded, the rules apply to matching H5P content types across the Moodle site, especially Interactive Book content and its embedded activities.

The CSS intentionally avoids Moodle page selectors such as course id or cmid. If the client later needs per-course styling, that should be handled with Moodle-side conditional CSS injection.
