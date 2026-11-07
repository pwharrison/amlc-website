# CLAUDE.md — Applied Machine Learning Conference Website

## Project overview

Jekyll static site for the Applied Machine Learning Conference (appliedml.us). The conference is annual; content is organized by year under `2026/`, `2025/`, etc. The 2026 conference has concluded — the site is now an archival resource.

## Local development

```bash
bundle exec jekyll serve   # http://localhost:4000
bundle exec jekyll build   # writes to _site/
```

## Architecture

### Per-year content
- `2026/index.md` — landing page (hero, about, highlights, venues, keynote speakers, speaker wall, sponsors)
- `2026/schedule.md` — conference schedule
- `2026/*.md` — other pages (cfp, jobs, register, sponsors, venue, survey)

### Session pages (2026)
- `_sessions/2026/*.md` — one file per session (40 talks + 1 lightning-talks page)
- Layout: `session-2026` — renders title, metadata, optional YouTube embed, description, speaker bio
- Permalink pattern: `/2026/sessions/slug/`
- To add a YouTube recording: set `youtube_id: VIDEO_ID` in the front matter

### Static embeds (generated, not hand-edited)
- `_includes/schedule-2026.html` — schedule grid (CSS Grid layout, ~80KB)
- `_includes/speaker-wall-2026.html` — speaker photo grid (~60KB)

### Layouts and includes
- `_layouts/session-2026.html` — session page layout; splits content at `<hr />` to inject YouTube embed between metadata and description
- `_layouts/page-2026.html`, `home-2026.html` — other 2026 layouts
- `_includes/header-2026.html`, `footer-2026.html` — shared chrome

### CSS
- Single stylesheet: `assets/css/style.css`
- Uses CSS custom properties (`--spacing-*`, `--bg-primary`, `--border-color`, etc.) defined in `:root`
- Key section classes: `.session-article`, `.speaker-wall`, `.featured-speaker`, `.speaker-card`

## Session page structure

Each `_sessions/2026/*.md` file follows this pattern:

```markdown
---
layout: session-2026
title: "Session Title"
permalink: /2026/sessions/session-slug/
youtube_id:
---

# Session Title

**Day, Month DD, YYYY · HH:MM AM – HH:MM PM · Venue Name**

---

Session description.

## About the Speaker

<div class="speaker-profile">
  <div class="speaker-profile-headshot">
    <img src="/assets/images/2026/speakers/First_Last.jpg" alt="Full Name">
  </div>
  <div class="speaker-profile-info">
    <h3>Full Name</h3>
    <p><em>Tagline</em></p>
    <p>Bio text.</p>
  </div>
</div>
```

The `---` after the metadata line is the split point used by the layout to position the YouTube embed.

## Speaker headshots

Stored at `assets/images/2026/speakers/First_Last.jpg` (or `.png`). Naming uses the speaker's first and last name joined with `_`. Multi-word first names also use `_` (e.g. `Akshata_Kishore_Moharir.png`).

## Jekyll collections config

```yaml
collections:
  sessions:
    output: true
```

The `_sessions/` directory maps to the `sessions` collection.

## Key CSS patterns

- `section:nth-child(even)` applies `background-color: var(--bg-secondary)` for alternating section backgrounds. Override with a more specific selector (e.g. `section.featured-speaker`) to pin a section's background regardless of position.
- `.session-article` is a flex column; flex `order` values reposition the YouTube embed (order 3) visually between the metadata (order 2) and the description (order 10) even though the embed appears earlier in the DOM.
- Speaker wall headshot circles require `overflow: hidden` on the container and `height: 100%; object-fit: cover` on the img.
