# RepreSENt GitHub Pages site

This version fixes markdown rendering on subpages and uses a simpler visual style closer to the original RepreSENt site.

For testing on GitHub Pages project URL:

```yaml
url: "https://alicethoylesense.github.io"
baseurl: "/representsend-site"
```

When mapping the real domain, change `_config.yml` to:

```yaml
url: "https://www.representsend.co.uk"
baseurl: ""
```

Then add a `CNAME` file containing:

```text
www.representsend.co.uk
```
