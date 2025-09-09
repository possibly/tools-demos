# Tools Demos (GitHub Pages)

Minimal site that lists interactive HTML/CSS/JS demos grouped by category, linking to each demo page.

## Add a demo (HTML)
Create an HTML file under `demos/` with YAML front matter (required for listing):

```html
---
title: "Canvas Particle Toy"
category: "Graphics"
description: "Interactive canvas demo (optional)"
---
<!doctype html>
<html>
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>{{ page.title }}</title>
</head>
<body>
  <canvas id="c"></canvas>
  <script>
    // Your interactive JS here
  </script>
</body>
</html>
```

The home page groups demos by `category` automatically.

## GitHub Pages
- Push to `main` and enable Pages (Settings → Pages → Deploy from a branch → `main`).
- If this is a project site, set in `_config.yml`:
  - `url: "https://<username>.github.io"`
  - `baseurl: "/<repo-name>"`
