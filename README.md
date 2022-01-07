# Live Free or Dy-nasty

*The source code for the Live Free or Dy-nasty website.*

## Development

The website a Jekyll site, with the full Jekyll install inside the `/docs` folder. All website changes should be made in the `/docs` directory to keep the root clean.

To set up your environment to develop this theme, run `script/bootstrap`.

To test your theme, run `script/server` (or `bundle exec jekyll serve`) and open your browser at `http://localhost:4000`. This starts a Jekyll server using your theme and the contents. As you make modifications, your site will regenerate and you should see the changes in the browser after a refresh.

## Adding a new page

Create a new markdown file inside the `docs` folder. Any `*.md` file will automatically become a page, and is automatically added to the site navigation.

Initiate your file with the following lines:

```md
---
layout: {layout-type}
title: {page-title}
permalink: {permalink}
---
```

### Layout (required)

The layout option chooses which template from the `_layouts` folder this page will use. Suggested layout for a new basic page is `page`.
### Title (optional)

The title of the page, which could display automatically in an `h1` tag, depending on which layout you choose.
### Permalink (optional)

A human-friendly link to use for this page. For instance, a file saved as `new-file.md` will have a URL of `livefreeordynasty.com/new-file.md` if no permalink is provided. If a permalink of `/new-file/` is provided, the page URL will be `livefreeordynasty.com/new-file/`.

## Publishing changes

Create a PR to the `main` branch, or create a commit directly to the `main` branch and push to GitHub. Any changes to `main` are automatically deployed to the website.
