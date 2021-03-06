---
outputs:
- Reveal
reveal_hugo:
  margin: 0.2
  templates:
    blue:
      background: '#0011DD'
      transition: zoom
  theme: night
title: Template presentation
---

## Template Example

---

This presentation shows how to take advantage of reveal-hugo's slide template feature.

---

Slide templates let you specify groups of slide attributes in one place and reuse them throughout the presentation.

---

{{< slide template="blue" >}}

Here's an example of using a template called `blue`, defined in the front matter of this presentation's `_index.md` file.

---

The template can contain any valid slide customization params:

```toml
[reveal_hugo.templates.blue]
background = "#0011DD"
transition = "zoom"
```

---

Then add it to any slide using the slide shortcode:

```
{{</* slide template="blue" */>}}
```

