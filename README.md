# RepreSENt GitHub Pages site

This is a clean static/Jekyll version of the RepreSENt website, ready to host on GitHub Pages.

## What is included

- Jekyll configuration for GitHub Pages
- Existing page structure and old-style URLs preserved:
  - `/about-represent.html`
  - `/the-sen-school-gap.html`
  - `/founders.html`
  - `/represent-girls.html`
  - `/useful-resources.html`
  - `/contact-us.html`
- Accessible, responsive layout
- Custom domain file: `CNAME`

## Before publishing

Search for `REPLACE_WITH_` and update the placeholder email addresses.

If you want to keep the current live site images, download them from the old hosting platform and add them to `assets/images/`, then insert them into the relevant Markdown pages.

## How to publish on GitHub

1. Create a new GitHub repository, for example `representsend-site`.
2. Upload all files in this folder to the repository.
3. Go to **Settings > Pages**.
4. Under **Build and deployment**, choose:
   - Source: `Deploy from a branch`
   - Branch: `main`
   - Folder: `/root`
5. Save.
6. In **Custom domain**, enter `www.representsend.co.uk`.
7. Update your domain DNS records where the domain is registered.

## Domain notes

This zip includes `CNAME` set to:

```txt
www.representsend.co.uk
```

For the apex/root domain `representsend.co.uk`, follow GitHub’s current DNS instructions for apex and `www` domains. Usually you will set GitHub Pages IP `A` records for the apex domain and a `CNAME` record for `www`, but check GitHub’s latest docs before changing DNS.

## Editing pages

Most pages are Markdown files. Edit the body text under the front matter block:

```yaml
---
layout: default
title: Page title
permalink: /page-url.html
---
```

The layout is in `_layouts/default.html`. The design is in `assets/css/style.css`.
