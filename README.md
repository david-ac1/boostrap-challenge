# Bootstrap Challenge: Full Stack Conf

## Overview

In this Bootstrap challenge, the goal is to replicate a conference landing page using only the Bootstrap 5 framework. The project emphasizes responsive design principles and effective use of Bootstrap components.

The finished page is a single `index.html` file that loads Bootstrap 5.3.3 from the jsDelivr CDN. It contains no `<style>` blocks, no inline `style` attributes, and no custom scripts. The only JavaScript is Bootstrap's own bundle, which powers the registration modal.


## Project Requirements

| Requirement | Details |
| --- | --- |
| Framework | Bootstrap 5 only (no custom JavaScript, no other frameworks) |
| Responsiveness | Must work flawlessly on mobile, tablet, and desktop devices |
| Browser compatibility | Chrome, Firefox, Safari, Edge (latest versions) |
| Code quality | Clean, semantic HTML with proper Bootstrap classes |

## Page Sections

| Section | Anchor | Bootstrap features used |
| --- | --- | --- |
| **Navigation** | `#home` | Sticky header, navbar, responsive flex utilities, dark theme (`data-bs-theme`) |
| **Hero** | `#home` | `bg-warning` background, display and lead typography, button group with two calls to action |
| **About** | `#about` | Three-column responsive grid (`col-md-4`), fluid rounded image, list group of topics |
| **Speakers** | `#speakers` | Grid of six speaker cards |
| **Schedule** | `#schedule` | List group with pill badges for times, highlighted lunch row, "Register Now" button |
| **Registration and newsletter** | `#registration-form` | Two-column layout, input group with an email sign-up form |
| **Footer** | n/a | Flex utilities, border and spacing helpers, responsive column-to-row layout |
| **Registration modal** | `#registerModal` | Modal with form controls: text and email inputs, select, checkbox group, payment fields, expiry-date selects |

## Tech Stack

- **HTML5**: semantic markup (`header`, `nav`, `main`, `section`, `footer`)
- **Bootstrap 5.3.3**: CSS and JS bundle via CDN
- **Git and GitHub**: team collaboration and version control

## Project Structure

```
boostrap-challenge-main/
├── index.html                      # The complete page
├── README.md                       # Project documentation (this file)
├── TEAM_PLAN.md                    # Workstream split and collaboration order
├── Task-Allocation-Tracker - 1.pdf # Contribution record and meeting log
└── project-demo.webm               # Reference demo of the page to replicate
```

## Getting Started

No build step or dependencies are required.

1. **Clone the repository**

   ```bash
   git clone <repository-url>
   cd boostrap-challenge-main
   ```

2. **Open the page**

   Open `index.html` directly in your browser, or serve the folder locally:

   ```bash
   # Python 3
   python -m http.server 8000
   # then visit http://localhost:8000
   ```

An internet connection is needed on first load because Bootstrap and the About section image are loaded from CDNs.

## Responsive Behavior

The layout is built with Bootstrap's mobile-first grid and utility classes.

- **Mobile (below 576px)**: navbar links and branding stack and center; columns, speaker cards, and the footer stack vertically.
- **Tablet (576px to 991px)**: the About and newsletter sections move into multi-column layouts at the `md` breakpoint (768px).
- **Desktop (992px and up)**: full three-column About layout, multi-card speaker grid, and a row-style footer.

## Accessibility

- Semantic landmarks and a logical heading hierarchy (`h1` followed by `h2` and `h3`)
- `aria-label` on the primary navigation and the hero button group
- Descriptive `alt` text on images
- Visually hidden labels on the email sign-up input
- Properly associated `label`, `input`, and `fieldset`/`legend` elements in the registration form
- Autocomplete attributes on the form fields

An accessibility scan was run during the review stage and reported no violations.

## Browser Compatibility

The page was tested in the latest versions of:

- Google Chrome
- Mozilla Firefox
- Safari
- Microsoft Edge

## Team and Contributions

The work was split into four workstreams, as described in [`TEAM_PLAN.md`](./TEAM_PLAN.md).

| Member | Responsibility |
| --- | --- |
| David Achibiri | Page structure: semantic HTML, sections, headings, footer, Bootstrap grid; mobile navigation fix |
| Olivier Itangishaka | Header and hero: navbar, hero copy, calls to action, responsive alignment; duplicate-markup cleanup |
| Aime Ndayambaje | Activity content: speaker cards, schedule badges, content polish |
| Christian Mpano | Quality and submission: browser and device testing, accessibility review, README, contribution PDF |

The full task allocation, completion status, and meeting attendance log are recorded in [`Task-Allocation-Tracker - 1.pdf`](./Task-Allocation-Tracker%20-%201.pdf).

## Collaboration Workflow

1. Agree on the reference page sections and content before editing shared markup.
2. Pull the latest `main` branch before each work session.
3. Keep each commit focused on one workstream and commit from your own GitHub account.
4. Test at mobile, tablet, and desktop widths before merging.
5. Add the completed contribution record PDF before the final push.

## Testing Summary

| Check | Result |
| --- | --- |
| Cross-browser (Chrome, Firefox, Safari, Edge) | Loads without errors; layout consistent across all four |
| Phone, tablet, and desktop layouts | Columns and cards stack correctly at each size |
| Accessibility scan | No violations reported |
| Issues found and fixed | Sideways scroll on mobile in the newsletter section; sticky navbar covering section headings after clicking a nav link |

---
