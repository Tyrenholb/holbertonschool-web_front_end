# CSS Advanced - Techium

This project applies CSS to the Techium digital-agency homepage. It develops
the page through 32 numbered stylesheets, moving from foundational styles and
custom properties to a responsive-looking layout with themed sections,
component states, and transitions.

The final homepage is [index.html](index.html), which loads
[`styles/32-style.css`](styles/32-style.css). Each numbered stylesheet is a
standalone cumulative version of the work completed up to that task, so the
progression can be reviewed by opening the files in order.

## Project contents

| File or folder | What it contains |
| --- | --- |
| [`index.html`](index.html) | The final Techium homepage with header, hero, services, works, about, news, testimonials, contact, and footer sections |
| [`styles/`](styles/) | The 32 cumulative CSS task files |
| [`images/`](images/) | Logos, favicon, portfolio images, article images, and testimonial avatars |

## CSS progression

| Tasks | What was added |
| --- | --- |
| 1–4 | Base colors, typography variables, link defaults, utility classes, and section text foundations |
| 5–13 | Custom properties for fonts, sizes, weights, line heights, colors, and smooth scrolling, plus Google Fonts integration |
| 14–18 | Normalize.css rules, universal box sizing, the main container, section spacing, and the initial page layout |
| 19–25 | Navigation, grid columns, footer layout, clearfix behavior, dark-section themes, service cards, and button states |
| 26–32 | Testimonial cards, hero styling, header positioning, animated navigation indicators, works overlays, quote decoration, and transitions |

## Final page sections

The completed homepage includes:

- A dark header with the Techium logo and navigation.
- A hero section with a background image and call to action.
- Services cards with hover states.
- A dark works section with image overlays and transitions.
- About, latest news, testimonials, and contact sections.
- A dark footer with contact details and social SVG icons.

## View the project locally

From the repository root:

```bash
cd CSS_advanced
python3 -m http.server 8000 --bind 127.0.0.1
```

Open `http://127.0.0.1:8000/` in a browser. The final page uses Google Fonts,
so font loading requires network access. Stop the server with `Ctrl+C`.

## Notes

- The numbered stylesheets are cumulative standalone files rather than an
  import chain, allowing each task to be inspected independently.
- The project is a CSS exercise built on the supplied Techium HTML structure;
  it does not include JavaScript or a package-based build system.
- Several homepage links use `#` placeholders because this project focuses on
  styling rather than routing or application behavior.
