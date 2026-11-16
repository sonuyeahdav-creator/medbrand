# MedBrand public website

This is the public marketing site for MedBrand and the EmpowerMed 45-day accelerator. It is a standalone static page: no build step, no server, no secrets.

## What is here

- `index.html` — the whole site (HTML, CSS, and a small script in one file)
- `assets/` — the brand images derived from the two supplied logo files
- `site.webmanifest` — name, theme colour and app icons for "Add to home screen"
- `.nojekyll` — tells GitHub Pages to serve the files as-is

## Logo assets

Both supplied logos are used, each in the role it suits. Only web-sized derivatives live here — the original files are not published.

| File | Size | Where it is used |
| --- | --- | --- |
| `assets/medbrand-lockup.png` | 196×44 | Header and footer wordmark (icon + "MedBrand") |
| `assets/medbrand-mark.png` | 42×44 | Hero insight card; favicons are derived from it |
| `assets/medbrand-seal.png` | 512×512 | About-section quote card; social share image |
| `assets/favicon-16/32/48.png` | 16–48 | Browser tab icons |
| `assets/apple-touch-icon.png` | 180×180 | iOS home-screen icon |
| `assets/icon-192.png`, `icon-512.png` | 192 / 512 | Android and PWA manifest icons |
| `assets/og-image.png` | 1200×630 | Open Graph and Twitter card preview |

Notes:

- The horizontal lockup was cropped to remove a dark edge strip from the screenshot and made transparent; the enclosed white letter counters are kept solid, so it is only placed on light backgrounds (hence the white chip behind it in the dark footer).
- The square file is a navy circular seal on a grey gradient with a faint watermark in one corner. The seal is cropped to the disc, so the watermark is outside the visible area.
- Keep the HTML `width`/`height` attributes in step with the real pixel sizes if any of these files are regenerated.

## Lead paths

1. **WhatsApp community** — the primary call to action. It links to the public group invite at `chat.whatsapp.com`.
2. **Qualifier portal** — links to the live EmpowerMed qualification app on Cloud Run.
3. **Email enquiry form** — the form does not post anywhere. It opens the visitor's own email app with a prefilled message to `sonuyeahdav@gmail.com`, and tells them plainly that the site does not send or store their details.

Nothing is collected by this site. There is no analytics, no cookie, and no third-party script except Google Fonts.

## Publish

GitHub Pages serves this repository from `main` at the root, so any push to `main` publishes the site.

Expected URL: <https://sonuyeahdav-creator.github.io/medbrand/>

## Content notes

- The page describes EmpowerMed as a training and introduction program. It does not promise a job, a salary, or a timeline.
- HIPAA-conscious design language is a practice, not a certification or compliance guarantee.
- The qualifier portal is a product project, not a clinical service.
- No patient or personal health information should be sent through the form or the community group.
