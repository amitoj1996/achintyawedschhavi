# Achintya & Chhavi — Wedding Invitation

A web-based wedding invitation for **Achintya Jain & Chhavi Jain**, with separate landing pages for the groom's and bride's families.

## Wedding Details

### Groom
- **Achintya Jain**
- Son of Shri Alok Jain & Smt. Pratibha Jain
- Grandson of (late) Shri Sureshchandra & Smt. Vidyavati Jain

### Bride
- **Chhavi Jain**
- Daughter of Shri Sanjay Jain & Smt. Rakhi Jain
- Granddaughter of (late) Shri Kusumchand & Smt. Kanta Devi Jain

## Events

| Day | Event | Time |
|-----|-------|------|
| **Saturday, June 20, 2026** | सगाई (Sagai) | 11:00 AM |
| | मायरा (Mayra) | 12:30 PM |
| | हल्दी (Haldi) | 2:00 PM |
| | संगीत संध्या (Sangeet Sandhya) | 7:30 PM |
| **Sunday, June 21, 2026** | देव दर्शन (Dev Darshan) | 8:00 AM |
| | बारात (Baraat) | 10:00 AM |
| | पाणिग्रहण संस्कार (Panigrahan Sanskar) | 2:00 PM |
| | आशीर्वाद समारोह एवं स्वरुचिभोज | 5:30 PM onwards |

**Venue**: Royal Orchid Resort, Near Malwa Institute, Nipania Bypass Road, Indore (M.P.)

## File Structure

```
.
├── index.html              # Groom's landing page (Achintya & Chhavi)
├── bride.html              # Bride's landing page (Chhavi & Achintya)
├── invitation.html         # 7-page flipbook (groom name first)
├── invitation-bride.html   # 7-page flipbook (bride name first, families swapped)
├── styles.css              # Shared section styles
├── Images/
│   ├── jain-emblem-gold.svg
│   └── jain-emblem-crimson.svg
└── README.md
```

## URLs once deployed

- Groom's side: `/` (default → `index.html`)
- Bride's side: `/bride.html`

## Local Preview

```bash
python3 -m http.server 8000
```

Open `http://localhost:8000/` for the groom flow or `http://localhost:8000/bride.html` for the bride flow.

## Editing Tips

- **Event times / names** — edit in both `invitation.html` and `invitation-bride.html` (look for `event-card` blocks)
- **Family details** — edit the `family-card` blocks in both invitation files; bride/groom order is swapped between them
- **Countdown target** — search for `new Date('2026-06-21T10:00:00+05:30')` in both invitation files
- **Theme colors** — edit `:root` variables in [styles.css](styles.css)
- **Jain emblem** — swap `Images/jain-emblem-gold.svg` (used on dark backgrounds) and `Images/jain-emblem-crimson.svg` (used on light backgrounds)
