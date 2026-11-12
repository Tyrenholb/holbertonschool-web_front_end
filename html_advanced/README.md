# HTML Advanced - Techium

This project builds the HTML structure for Techium, a fictional digital agency.
I worked through progressive exercises covering document structure, semantic
elements, navigation, text content, images, and embedded media.

The directory keeps earlier numbered versions alongside the final homepage
and style guide, so the progression can be followed through the source files.
The focus is HTML structure; there are no CSS stylesheets or JavaScript files.

## Main pages and assets

| File or folder | What it contains |
| --- | --- |
| [`index.html`](index.html) | The latest homepage, with services, works, about, news, testimonials, contact, and footer sections |
| [`styleguide.html`](styleguide.html) | Examples of headings, paragraphs, lists, quotes, typography, tables, details, video, audio, and an iframe |
| [`about.html`](about.html) | An About-titled page retaining the earlier homepage layout and sample content |
| [`latest_news.html`](latest_news.html) | A Latest news-titled page retaining the earlier homepage layout and sample content |
| [`contact.html`](contact.html) | A Contact-titled page retaining the earlier homepage layout and sample content |
| [`article.html`](article.html) | A basic article scaffold with header, main, aside, and footer landmarks |
| [`images/`](images/) | Ten images used for portfolio work, blog posts, the about section, and testimonial avatars |
| [`logo-black.png`](logo-black.png) | The Techium logo used in the homepage header and footer |
| [`favicon.ico`](favicon.ico) and [`favicon.png`](favicon.png) | Browser icon assets referenced by the pages |

## Exercise progression

There are 37 numbered HTML files. They are saved stages of the homepage or
style guide, rather than separate finished websites. Some exercises update an
unnumbered page, so the filenames do not form a continuous number sequence.

| Files | What was added |
| --- | --- |
| `0-index.html` through `3-index.html` | Initial HTML document, head/body structure, metadata, favicons, and page landmarks |
| `5-index.html` through `10-index.html` | Homepage sections, articles, navigation structure, and heading levels |
| `11-styleguide.html`, `12-index.html`, `13-styleguide.html` | Heading examples, homepage paragraphs, and a paragraph style-guide section |
| Numbered files from `14` through `25` | Content wrappers, comments, links, navigation lists, calls to action, and footer links |
| Numbered files from `26` through `34` | Lists, rules, quotations, contact details, typography, a table, and collapsible details, alongside homepage refinements |
| `35-index.html` and `36-index.html` | Logo, portfolio images, blog images, about image, and testimonial avatars |
| `38-styleguide.html` and `39-styleguide.html` | Video and audio examples |
| `index.html` and `styleguide.html` | Latest versions, including SVG social icons on the homepage and a YouTube iframe in the style guide |

## HTML features

- Document language, text direction, character encoding, viewport metadata,
  page titles, descriptions, and favicon links.
- Semantic structure using `header`, `nav`, `main`, `section`, `article`,
  `aside`, and `footer` where relevant.
- Headings, paragraphs, lists, links, blockquotes, citations, and addresses.
- Images with alternative-text attributes, including named testimonial avatars,
  plus inline SVG social icons.
- Table captions and scoped headers, and native `details`/`summary` controls.
- Native video and audio controls, plus a titled iframe.

## Requirements

- A modern browser to view the HTML and native media elements.
- Python 3 if using the local preview server below.
- Internet access for the externally hosted video, poster image, audio, and
  YouTube embed. Their availability depends on the external services.

There is no package installation, compilation, or application backend.

## View the project locally

From the repository root:

```bash
cd html_advanced
python3 -m http.server 8000 --bind 127.0.0.1
```

Open these addresses in your browser:

- Homepage: `http://127.0.0.1:8000/`
- Style guide: `http://127.0.0.1:8000/styleguide.html`
- Article scaffold: `http://127.0.0.1:8000/article.html`

Other pages and numbered exercises can be opened by appending their filenames,
for example `http://127.0.0.1:8000/36-index.html`.

Stop the server with `Ctrl+C`. Serving from this directory lets the homepage's
root link (`/`) return to Techium rather than the parent repository listing.

## What to explore

1. Compare an early numbered homepage with `index.html` to follow the growth
   of the document structure and content.
2. Open `styleguide.html` to inspect each element example. Toggle the details
   controls and try the media players when external resources are available.
3. Follow the homepage's About and Contact links to the supporting pages.
4. Inspect the HTML source to see the relationship between headings, landmarks,
   images, and content sections.

## Current limitations

- The pages use browser-default presentation. CSS styling and JavaScript
  interactions are outside this checked-in project.
- Many links use `#` as a placeholder. Homepage section links such as
  `#services` currently have no matching section IDs, so those navigation jumps
  are not connected.
- The supporting About, Contact, and Latest news pages still reuse an earlier
  homepage template. The article page is a scaffold, and much of the text is
  sample content.
- Media playback depends on network access, browser support, and the external
  hosts. The audio and video are linked, not bundled in this directory.
- Local file and preview checks do not establish complete HTML validity or
  accessibility conformance.
