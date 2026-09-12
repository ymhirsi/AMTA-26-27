# AMTA Website

A static website for the Appalachian Music Teachers Association.

## File Structure

```
amta-site/
├── index.html               Homepage
├── about.html               About + mission + history
├── executive-committee.html Leadership / officers
├── events.html              Public events calendar
├── for-students.html        Student info, auditions guide
├── resources.html           Find a Teacher (search) + affiliated orgs
├── contact.html             Single contact form
├── styles.css               Shared styles
├── images/
│   └── amta-group.jpg       Group photo (used on homepage)
└── README.md
```

## What's Working

- **Teacher search** on `resources.html` — fully functional. Populated with 24 real AMTA members from the 2026–2027 yearbook. Instrument specialties are not yet populated; the search accounts for this and returns all teachers regardless of instrument filter.
- **Contact form** on `contact.html` — configured for Netlify Forms. When deployed to Netlify, submissions appear in the Netlify dashboard automatically. No backend required.
- **Group photo** on homepage — image is at `images/amta-group.jpg`.

## Content Source

The 2026–2027 season content is drawn from the 2026-2027 AMTA yearbook. Officer names, events, and member directory reflect that source.

## To Add Instrument Data to Teachers

Open `resources.html`, scroll to the `<script>` section, and edit the `instruments: []` array for each teacher. Use lowercase strings that match the dropdown options (e.g. `["piano", "voice"]`).

## Items Flagged for Confirmation Before Publishing

- **Audition registration deadline year** — Yearbook lists "postmark March 15, 2026" for the April 10, 2027 auditions. Confirmed to be intended as 2027 before publishing. Flagged in `events.html`, `for-students.html`, and `index.html`.
- **Member emails** — 24 personal emails are now published on the public directory. Confirm each member has consented to public listing before deploying.
- **December potluck / May luncheon dates and locations** — Both listed as TBD in the yearbook.
- **March 6 masterclass location and time** — TBD in the yearbook.

## Sections Still Needing Real Content

Search for `placeholder` in the files to find every placeholder at once. Main items:
- About page: History section
- Executive Committee: Officer bios and photos
- For Students page: Step-by-step audition process, Honors Recital details, TMTA State details
- Bristol Music Club and Kingsport Music Club websites / contact info

## To Deploy

1. Drag the `amta-site` folder onto netlify.com
2. Netlify gives you a URL like `random-name-123.netlify.app`
3. In Netlify settings → Forms, you'll see the contact form submissions
4. Set up email notifications in Netlify → Forms → Notifications

## Updating with Claude

Share the relevant file(s) and describe what you want changed. For site-wide changes, share the full folder as a zip.
