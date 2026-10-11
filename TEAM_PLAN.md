# Team Plan

This challenge is split into four small workstreams so the project can move forward even if the group is unavailable.

| Member | Responsibility | Deliverable |
| --- | --- | --- |
| 1 | Page structure | Semantic HTML, document sections, headings, footer, and Bootstrap container/grid layout |
| 2 | Header and hero | Navbar, hero copy, calls to action, and responsive alignment |
| 3 | Activity content | Activity cards, badges, progress summary, and content polish |
| 4 | Quality and submission | Mobile/desktop checks, accessibility pass, browser testing, README updates, and contribution PDF |

## Suggested collaboration order

1. Agree on the reference page sections and content before editing shared markup.
2. Pull the latest `main` branch before each work session.
3. Keep each commit focused on one workstream and use the contributor's own GitHub account.
4. Test at narrow mobile width, tablet width, and desktop width before merging.
5. Add the completed contribution record PDF before the final push.

## Current implementation

`index.html` is the shared baseline for the Full Stack Conf reference. It uses Bootstrap 5 CDN classes only and intentionally has no custom JavaScript or stylesheet. The page is divided into the navigation and hero, overview columns, speaker cards, schedule, registration/newsletter area, and footer.