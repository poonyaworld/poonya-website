# Poonya Website

Static HTML/CSS website for GitHub Pages.

## Files

- `index.html` - home page with app overview and five app preview screens.
- `terms.html` - Terms of Use page.
- `privacy.html` - Privacy Policy page.
- `contact.html` - contact form page.
- `styles.css` - responsive styling.
- `assets/AppLogo.png` - Poonya app logo.
- `images/app-preview-1.svg` through `images/app-preview-5.svg` - replaceable home page preview images.

## Replacing Home Page Images

Replace the files in `images/` with your real app screenshots. Keep the same filenames for the easiest update:

- `app-preview-1.svg`
- `app-preview-2.svg`
- `app-preview-3.svg`
- `app-preview-4.svg`
- `app-preview-5.svg`

You can also use PNG or JPG screenshots. If you change the file extensions, update the matching `src` values in `index.html`.

## Google Form Setup

The contact form is ready to submit to Google Forms, but the Google Form endpoint and field IDs must be replaced first.

1. Create a Google Form with fields for name, email, and message.
2. Open the form, inspect the prefilled form or page source, and find the `formResponse` URL plus each `entry.xxxxx` field name.
3. In `contact.html`, replace:
   - `YOUR_GOOGLE_FORM_ID`
   - `entry.YOUR_NAME_FIELD_ID`
   - `entry.YOUR_EMAIL_FIELD_ID`
   - `entry.YOUR_MESSAGE_FIELD_ID`

## GitHub Pages

Push these files to a GitHub repository, then enable Pages from the repository settings. Use the repository root as the Pages source.
