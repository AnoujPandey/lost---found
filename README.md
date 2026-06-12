# Campus Lost & Found — Final Project

Members:Anouj Pandey-Topendra Gharti Magar-Kabiraj Chaudhary-Anish Kafle
**Course:** Web Programming
**University:** Dong-Eui University

---

## Project Overview

A multi-page website for reporting, browsing, and recovering lost and found items on campus. Students can report lost belongings, submit items they have found, view current listings, and contact the Lost & Found office.

---

## Pages

| File | Purpose |
|---|---|
| `index.html` | Home page with video hero and about section |
| `listings.html` | Browse all lost and found item cards and table |
| `report-lost.html` | Form to report a lost item |
| `report-found.html` | Form to submit a found item |
| `contact.html` | Contact form and office information |

---

## File Structure

```
final-project/
│
├── index.html          ← Home page
├── listings.html       ← Item listings page
├── report-lost.html    ← Report lost item form
├── report-found.html   ← Report found item form
├── contact.html        ← Contact page
│
├── style.css           ← Main styles — used by ALL pages
├── layout.css          ← Page width and column layouts — used by ALL pages
├── forms.css           ← Form-specific styles — used by form pages only
│
├── media/              ← Images and video files
│   ├── campus.mp4
│   ├── backpack.jpeg
│   ├── earbuds.jpeg
│   ├── id.jpeg
│   ├── keys.jpeg
│   ├── phone.jpeg
│   └── wallet.jpeg
│
└── README.md           ← This file

---

## CSS Files Explained

### style.css
The main stylesheet loaded by every page. Contains:
- CSS variables (colours, fonts, spacing)
- Base reset and typography
- Header and navigation
- Cards, buttons, table, gallery
- Home page hero (video background) and about section
- Footer
- Responsive breakpoints for tablet and mobile

### layout.css
Controls page width and structural layouts:
- Centres content and limits max width
- Header flex layout (logo + nav)
- Hero two-column grid (text + image)
- Contact page flex layout (form + sidebar)
- Responsive overrides

### forms.css
Loaded only by `report-lost.html`, `report-found.html`, and `contact.html`:
- Form section cards and fieldsets
- All input, textarea, and select styling
- Radio buttons and checkboxes
- Submit and clear buttons
- Office info sidebar and hours table
- Map embed and tips card

---

## Technologies Used

- HTML5 (semantic elements: `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>`, `<footer>`, `<figure>`, `<fieldset>`)
- CSS3 (Grid, Flexbox, custom properties, media queries, transitions)
- No JavaScript or external libraries used

---

## Responsive Design

| Screen size | Layout |
|---|---|
| Desktop (above 860px) | Full multi-column layouts |
| Tablet (max 860px) | Two-column grids, stacked header |
| Mobile (max 560px) | Single column, full-width buttons |
| Form pages (max 768px) | Stacked form and sidebar |

---

## Accessibility Features

- Skip link on every page for keyboard navigation
- `aria-label` on navigation and interactive elements
- `aria-hidden="true"` on decorative SVG icons
- `alt` text on all images
- `title` attribute on the embedded map iframe
- `scope` attributes on all table headers
- Required fields marked with both `required` attribute and visual asterisk
