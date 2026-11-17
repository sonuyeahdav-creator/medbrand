# MedBrand public website

The public marketing site for MedBrand, a founder-led healthcare growth practice, and the EmpowerMed 45-day accelerator. It is a standalone static page: no build step, no server, no secrets.

## What is here

- `index.html` — the whole site (HTML, CSS, and a small script in one file)
- `assets/` — the brand images derived from the two supplied logo files
- `site.webmanifest` — name, theme colour and app icons for "Add to home screen"
- `.nojekyll` — tells GitHub Pages to serve the files as-is

## Site structure

One page, two clear audiences:

- **For clinics and health brands** — WhatsApp first, then a scheduled discovery call, then an email enquiry. Services are grouped into four clusters: Brand & Reputation; Growth & Acquisition; Product & Automation; Footfall & Appointments.
- **For applicants and career builders** — qualifier test first, then counseling and enrollment on Google Meet or Zoom, then the WhatsApp community talent pool. The qualifier and cohort are paid programs.
- EmpowerMed stays the flagship program, with the 45-day roadmap.
- Proof uses the founder's real, verifiable portfolio outcomes (hackathon placing, deployed RAG workflows, shipped MedBrand MVP). Client case studies are confidential.
- A short founder section links to the real LinkedIn and portfolio profiles.

## Logo assets

Both supplied logos are used, each in the role it suits. Only web-sized derivatives live here — the original files are not published.

| File | Size | Where it is used |
| --- | --- | --- |
| `assets/medbrand-lockup.png` | 196×44 | Header and footer wordmark (icon + "MedBrand") |
| `assets/medbrand-mark.png` | 42×44 | Hero insight card; favicons are derived from it |
| `assets/medbrand-seal.png` | 512×512 | Founder-section quote card; social share image |
| `assets/favicon-16/32/48.png` | 16–48 | Browser tab icons |
| `assets/apple-touch-icon.png` | 180×180 | iOS home-screen icon |
| `assets/icon-192.png`, `icon-512.png` | 192 / 512 | Android and PWA manifest icons |
| `assets/og-image.png` | 1200×630 | Open Graph and Twitter card preview |

Notes:

- The horizontal lockup was cropped to remove a dark edge strip from the screenshot and made transparent; the enclosed white letter counters are kept solid, so it is only placed on light backgrounds (hence the white chip behind it in the dark footer).
- The square file is a navy circular seal on a grey gradient with a faint watermark in one corner. The seal is cropped to the disc, so the watermark is outside the visible area.
- Keep the HTML `width`/`height` attributes in step with the real pixel sizes if any of these files are regenerated.

## Lead paths

1. **Clinic WhatsApp** — primary client CTA. Direct `wa.me` link to `+91 99583 88301` with a prefilled message, so no form has to be filled before a conversation starts. The WhatsApp Business chatbot should ask name, organisation and need.
2. **Discovery call** — a `mailto:` link requests preferred times; the meeting itself happens on Google Meet or Zoom. To use Google Calendar appointment scheduling instead, replace the `CALL` link in the page with your booking URL.
3. **Email enquiry form** — tertiary. It does not post anywhere. It opens the visitor's own email app with a prefilled message to `sonuyeahdav@gmail.com` and states plainly that the site does not send or store details.
4. **Qualifier portal** — the live EmpowerMed qualification app on Cloud Run. It is **for applicants only**, and is now the first step in the student funnel (fee to appear).
5. **Community WhatsApp** — used after enrollment as the talent-pool community, not as the primary client CTA.
6. **Payments** — qualifier and cohort fees are collected during counseling through a Razorpay payment link. Razorpay accepts international cards when international payments are enabled and KYC is complete. No card details are taken on this site.

The site itself collects nothing: no analytics, no cookie, no form storage. WhatsApp, the qualifier portal, Google Meet and Razorpay handle their own data under their own privacy policies.

## Before launch

- Enable international payments on the Razorpay account and complete KYC. Test with Razorpay's international test cards.
- Configure the WhatsApp Business chatbot to ask name, organisation and need, and to hand off to you.
- Confirm the qualifier test fee and cohort fee amounts (they are deliberately not published on the site).
- Optionally replace the discovery-call `mailto:` with a Google Calendar appointment-scheduling URL.

## Publish

GitHub Pages serves this repository from `main` at the root, so any push to `main` publishes the site.

Expected URL: <https://sonuyeahdav-creator.github.io/medbrand/>

## Content notes

- No prices are published. Work is scoped per engagement; program fees are shared during application.
- EmpowerMed is a paid training program. It does not promise a job, a salary, or a timeline.
- HIPAA-conscious design language is a practice, not a certification or compliance guarantee.
- The qualifier portal is a product project, not a clinical service.
- No patient or personal health information should be sent through the form, WhatsApp, or the community group.
- Public copy avoids "side hustle" and "freelancer" framing. MedBrand is presented as a founder-led practice with vetted associates.
