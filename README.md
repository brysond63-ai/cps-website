# Carroll Professional Services — Website

A calming, professional website for **Carroll Professional Services**, a psychology
practice led by **Jennifer Carroll, PhD**, in **Tupelo, Mississippi**. In-person and
telehealth psychological services.

## Structure

```
carroll-professional-services/
├── index.html          # Home
├── what-we-do.html     # What We Do
├── about.html          # About Jennifer Carroll, PhD
├── associates.html     # Meet Our Associates
├── telehealth.html     # Telehealth
├── contact.html        # Contact + appointment request form
├── css/
│   └── styles.css       # All site styling (brand palette, layout, responsive)
└── assets/
    ├── logo.svg         # Emblem: white dove + green beak, cradled in leaves, blue ring
    └── favicon.svg      # Simplified favicon version of the emblem
```

It is a static site — no build step. Open `index.html` in a browser, or serve the
folder (e.g. `python3 -m http.server`) and visit `http://localhost:8000`.

## Brand palette (in `css/styles.css` `:root`)

| Token | Value | Use |
|-------|-------|-----|
| `--navy` | `#1C3E6B` | Headers, buttons, footer |
| `--blue` | `#2D5C9E` | Logo ring blue — secondary accents |
| `--green` | `#5E9A47` | Logo leaf green — highlights, icons, dividers, leaf accents |
| `--sage` / `--sage-soft` | `#D6E3CD` / `#EDF3E7` | Calm section backgrounds |
| `--cream` | `#FBF8F1` | Main background |

Palette is sampled directly from the logo (royal blue ring, leaf-green laurel/hands,
white dove). Deep navy is a darker shade of the same blue hue for grounding.

Fonts: **Lora** (serif headings) + **Source Sans 3** (sans-serif body), via Google Fonts.

## Placeholders to replace before launch

- **Logo**: `assets/logo.svg` is an on-brand SVG interpretation of the real emblem
  (white dove with green beak, cradled in green leaves, inside a blue heart and a
  green/blue ring). For print-quality fidelity, swap in the official logo file when
  available — keep the filename `assets/logo.svg` to avoid touching markup.
- **Contact details**: phone, email, street address, and office hours (search for
  `(000) 000-0000`, `office@example.com`, `0:00`).
- **Associates**: name, credentials, role, focus, bio, availability, and photos on
  `associates.html`.
- **Photos**: portrait on `about.html` and associate photos use styled placeholders.
- **Form handling**: the contact form `action="#"` is not yet wired to a backend or
  email service.

## Copy guardrails honored

Uses psychological services / evaluations, individualized care, professional
consultations, compassionate support, telehealth. Avoids psychiatric / psychiatrist /
medical doctor / medication / prescriptions and any guaranteed-outcome language.
Dr. Carroll is presented as a PhD-level psychology professional.
