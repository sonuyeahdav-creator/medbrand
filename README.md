# MedBrand public website

This is the public marketing site for MedBrand and the EmpowerMed 45-day accelerator. It is a standalone static page: no build step, no server, no secrets.

## What is here

- `index.html` — the whole site (HTML, CSS, and a small script in one file)
- `.nojekyll` — tells GitHub Pages to serve the files as-is

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
