# TJ Joints — Company Website

A single-page website for **TJ Joints**, a Singapore-based provider of professional electrical cabling and jointing services (LV and HV, up to 22kV).

## Overview

The whole site is one self-contained file, `index.html`, with inline CSS and JavaScript. It needs no build step, framework or server. The only external resource is the Google Fonts stylesheet (Barlow and Barlow Condensed).

### Page sections

| Section  | Anchor      | Contents                                                        |
|----------|-------------|-----------------------------------------------------------------|
| Hero     | `#top`      | Headline, calls to action, cable joint illustration             |
| Stats    | —           | Key figures (experience, joints completed, voltage, response)   |
| Services | `#services` | Six service cards: HV jointing, terminations, LV cabling, cable laying, testing, fault repair |
| About    | `#about`    | Why choose TJ Joints, voltage ranges, company summary           |
| Process  | `#process`  | Four-step workflow from site survey to handover                 |
| Sectors  | `#sectors`  | Industries served                                               |
| FAQ      | `#faq`      | Expandable common questions                                     |
| Contact  | `#contact`  | Contact details, emergency hotline, quote request form          |

### Features

- Responsive layout for desktop, tablet and mobile, with a collapsible menu on small screens
- Sections fade in as you scroll, and the animation is turned off for visitors who prefer reduced motion
- Semantic HTML with accessible labels and keyboard-friendly FAQ items
- The quote form checks required fields, then opens the visitor's email app with the enquiry filled in, so no backend is needed

## Running locally

Open `index.html` in any modern browser. To serve it over HTTP instead:

```bash
# Python 3
python -m http.server 8000
# then visit http://localhost:8000
```

## Before going live

Replace these placeholder values in `index.html`:

- [ ] **Phone number:** `+65 0000 0000` (header of the contact section and the emergency hotline)
- [ ] **Email address:** `enquiry@tjjoints.sg` (contact details and the form's `mailto:` link in the script)
- [ ] **Office address:** currently just "Singapore"
- [ ] **Stats:** years of experience and number of joints completed
- [ ] **Claims:** voltage range, 24/7 availability, standards and certifications, office hours, and the quote in the About panel

To have form submissions sent straight to an inbox instead of opening the visitor's email app, connect the form to a form service such as Formspree or Netlify Forms.

## Deployment

Any static host works. Upload `index.html` to one of these:

- GitHub Pages
- Netlify / Vercel (drag and drop or Git integration)
- Any traditional web host

## Project structure

```
company-site/
├── index.html   # The complete website
└── README.md    # This file
```
