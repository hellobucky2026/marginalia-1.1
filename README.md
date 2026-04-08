# Marginalia

A literary editorial theme for [Micro.blog](https://micro.blog) — clean, typographic, and unhurried.

Inspired by *The Paris Review* and longform personal publishing. Designed for writers who want their words to breathe.

---

## Features

- **EB Garamond** body type, **Playfair Display** headlines, **DM Mono** for metadata
- Editorial red accent (`#b34a2a`) for links, category tags, and micro-post markers
- Distinct treatment for **titled long posts** vs **short micro posts** (¶ marker)
- Clean single-column layout with generous whitespace
- Responsive, print-friendly, accessible
- Dark footer contrast strip

---

## Installation

### Via Micro.blog (recommended)

1. Log into Micro.blog → **Design** → **Edit Themes**
2. Click **New Theme**
3. Upload this zip, or paste files into the editor

### Manual (Hugo)

```
themes/
  marginalia/
    layouts/
    static/
    theme.toml
```

Add to your `config.toml`:
```toml
theme = "marginalia"
```

---

## Configuration

In your `config.toml` or Micro.blog custom parameters:

```toml
[params]
  tagline    = "Notes on reading, medicine, and everything else."
  footerText = "All opinions my own."
```

### Menus

```toml
[[menus.main]]
  name = "Archive"
  url  = "/archive/"

[[menus.main]]
  name = "About"
  url  = "/about/"

[[menus.footer]]
  name = "RSS"
  url  = "/feed.xml"
```

---

## Customization

All design tokens live in CSS custom properties at the top of `marginalia.css`:

```css
:root {
  --accent: #b34a2a;     /* change the editorial accent color */
  --measure: 68ch;       /* line length / content width */
}
```

---

## License

MIT
