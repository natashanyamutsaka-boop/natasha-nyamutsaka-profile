# natasha-nyamutsaka-profile
A personal profile website created using html and css for my web technologies assignment
## Prompt Log
[view my Prompt Log](PROMPT_LOG.md)


## Accessibility Issue and Fix

### Issue Identified
During peer review, it was identified that the background colours intended for the different sections of the website were not being displayed. This was caused by a mismatch between the selectors used in the HTML and the corresponding CSS selectors. The sections were assigned classes in the HTML, while the CSS styling was written to target IDs.

### Fix Applied
I corrected the HTML and CSS selectors so that the section IDs and their corresponding CSS ID selectors matched correctly. This allowed the intended background colours to be applied to each section and display properly on the website.


## Responsive Notes

### Breakpoints tested
Tested in Chrome DevTools device toolbar at **375px (mobile)**, **768px (tablet)**
and **1280px (desktop)**. No horizontal scrolling, overlapping text or broken
navigation at any of the three widths. The page is `profile3.html`.

### Mobile-first approach
Base styles in `style3.css` target mobile. Custom `min-width` media queries at
768px and 1200px add larger-screen layouts.

### Flexbox vs Grid
- **Flexbox:** the skills list (`flex-wrap`, `gap`, `justify-content`, `align-items`),
  because skill tags are a one-dimensional row that should wrap naturally.
- **Grid:** the About section, with the article and aside in `2fr 1fr` columns
  on tablet and desktop and stacked on mobile, because I'm controlling column
  proportions for the whole section.

### Tailwind vs custom CSS
- **Tailwind:** header/nav (`md:` variants) and the contact form (`sm:` variant).
- **Custom CSS (`style3.css`):** typography, colour variables, section spacing,
  skills Flexbox, About Grid and the media queries.
- Tailwind's preflight reset is disabled so it doesn't override my base styles.