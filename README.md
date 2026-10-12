# Blog Post Page

A single, semantic HTML blog post page. This is a beginner project from [roadmap.sh](https://roadmap.sh/projects/blog-post-page) focused on marking up long-form content with the right HTML elements. The page is intentionally unstyled; the goal is a clean structure that readers, screen readers and search engines can all understand, and that makes a solid base for adding CSS later.

## Project Overview

The page represents one blog post and demonstrates:

- Semantic page regions
- A correct heading hierarchy
- The right text element for each kind of content
- Meaningful emphasis
- Descriptive links
- An accessible figure with an image and caption
- Proper head metadata

## Page Structure

| Region | Purpose |
| --- | --- |
| `<header>` | Site name and primary navigation |
| `<main>` | Contains a single `<article>` holding the post |
| `<article>` | The blog post itself |
| `<footer>` | Closing content such as copyright |

### Headings

- One `<h1>` for the post title
- `<h2>` and `<h3>` for sub-sections inside the article, with no skipped levels

### Text Elements

- `<p>` for paragraphs
- `<ul>` / `<ol>` for lists
- `<blockquote>` with `<cite>` for quoted text and its source
- `<code>` / `<pre>` for inline code and code blocks
- `<em>` for stress and `<strong>` for importance (not just for italic or bold looks)

### Links

Every link uses descriptive text that says where it goes. There are no "click here" or "read more" links.

### Figure

One image inside the article, wrapped in `<figure>` with a `<figcaption>`. The `<img>` has a useful `alt` attribute, since the caption does not replace alt text.

### Head Metadata

- `<title>`
- `<meta charset>`
- `<meta name="viewport">`
- `<meta name="description">` summarising the post

## Getting Started

1. Clone the repository:

   ```bash
   git clone https://github.com/KunalGuhagarkar/Blog-Post-Page.git
   cd Blog-Post-Page
   ```

2. Open the HTML file in `src/` in any modern browser. No build step or dependencies are needed.

   Optionally, serve it locally:

   ```bash
   cd src
   python3 -m http.server 8000
   ```

   Then visit `http://localhost:8000`.

## Project Structure

```
Blog-Post-Page/
├── src/          # The HTML page and its assets (e.g. the figure image)
└── README.md
```

## Submission Checklist

- [x] Single HTML page with header, main, article and footer regions
- [x] One `<h1>` for the post title, with `<h2>` / `<h3>` for real subsections
- [x] Lists, quotes and code elements used semantically
- [x] Descriptive link text on every link
- [x] `<figure>` with `<img alt>` and `<figcaption>`
- [x] Head metadata set, including a meta description

## What I Learned

- Choosing semantic tags for the kinds of text found in blogs, docs, release notes and product descriptions
- Keeping a logical heading outline for accessibility and SEO
- Writing meaningful alt text and link text
- Building a structure that can be styled with CSS later without rewriting the HTML

## Next Steps

- Add CSS for layout, typography and responsiveness
- Run an accessibility check (for example Lighthouse or axe)

## Author

**Kunal Guhagarkar**
GitHub: [@KunalGuhagarkar](https://github.com/KunalGuhagarkar)

## Acknowledgements

Project idea from [roadmap.sh](https://roadmap.sh/projects/blog-post-page).