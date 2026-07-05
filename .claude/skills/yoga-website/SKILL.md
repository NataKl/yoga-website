---
name: yoga-website
description: Skill for working with the Body & Mind yoga landing page repository. Helps Claude Code understand the project structure, launch the site, make edits, update the README, check for issues, and prepare the project for publication.
---

# yoga-website Skill

This skill guides Claude Code when working with the `yoga-website` repository — a static HTML/CSS landing page for the Body & Mind yoga, pilates, and meditation studio.

## Project Overview

- **Type:** Static single-page website (landing page)
- **Stack:** HTML5, CSS3, Google Fonts
- **Entry point:** `index.html`
- **Styles:** `style.css`
- **No build step** required
- **Live demo:** http://u3554010.isp.regruhosting.ru/ (hosted on Reg.ru; HTTPS is unavailable because the subdomain `*.isp.regruhosting.ru` is a shared hosting domain and cannot be validated for an SSL certificate)
- **Target audience:** Yoga and wellness studios, private instructors, wellness spaces

## Repository Structure

```
yoga-website/
├── index.html                  # Main landing page
├── style.css                   # Custom CSS with variables, animations, responsive design
├── README.md                   # Project description, tagline, usage instructions
├── yoga.jpg                    # Hero background image
├── yoga2.jpg                   # About section image
├── take-your-time.ru_.png      # Reference / moodboard screenshot
├── yoga.txt.txt                # Original description text (source material)
└── .claude/skills/yoga-website/SKILL.md   # This file
```

## Design Direction

- **Tone:** Calm, warm, minimal, organic, refined
- **Aesthetic:** Soft beige/olive palette, elegant serif display font (Cormorant Garamond) + clean sans-serif body (Outfit)
- **Features:** Full-screen hero, smooth reveal animations, grain overlay, asymmetric organic shapes, responsive layout
- **Never use:** Generic fonts (Inter, Roboto, Arial), cliché purple gradients, cookie-cutter layouts

## Common Tasks

### Understand the Project

When the user asks about the project, summarize:
1. What it is (Body & Mind landing page)
2. Stack and structure
3. Design direction
4. Link to GitHub: https://github.com/NataKl/yoga-website
5. Link to live demo: http://u3554010.isp.regruhosting.ru/ (Reg.ru hosting; HTTPS not available for shared hosting subdomain)

### Launch the Site

Since this is static HTML/CSS, launch by opening the file in the default browser:

- **Windows:** `start index.html`
- **macOS:** `open index.html`
- **Linux:** `xdg-open index.html`

For a quick local server (optional):
```bash
python -m http.server 8000
```

### Make Changes

1. Read `index.html` and `style.css` before editing.
2. Preserve the existing design system (CSS variables, fonts, spacing scale, animations).
3. Keep edits focused and minimal unless a redesign is explicitly requested.
4. Validate HTML/CSS after changes.

### Update README.md

When updating the README:
1. Keep the tagline at the top.
2. Reflect any new sections, features, or technologies.
3. Update usage instructions if the launch process changes.
4. Maintain Russian language (primary language of the project).

### Check for Issues

Before considering work complete:
1. Check that `index.html` and `style.css` exist and are linked.
2. Verify all image paths (`yoga.jpg`, `yoga2.jpg`) are correct.
3. Ensure no broken links or missing assets.
4. Validate HTML with a linter or quick browser open.
5. Check responsive breakpoints (900px, 768px).

### Prepare for Publication

When the user asks to publish or prepare the project:
1. Confirm README is up to date.
2. Ensure all changes are committed with clear messages.
3. Push to origin/main.
4. The site is also deployed at http://u3554010.isp.regruhosting.ru/ via Reg.ru hosting. HTTPS is not available for this shared hosting subdomain.
5. Optional: suggest GitHub Pages deployment with these settings:
   - Source: Deploy from a branch → `main` → `/ (root)`
   - URL will be `https://NataKl.github.io/yoga-website`

## Commit Message Conventions

Use concise, descriptive messages:
- `Update hero section copy`
- `Fix mobile navigation spacing`
- `Add README section for GitHub Pages`
- `Replace yoga hero image`

## Guardrails

- **Do not delete** original assets (`yoga.jpg`, `yoga2.jpg`, `yoga.txt.txt`) unless explicitly asked.
- **Do not rename** the repository or main files without confirmation.
- **Do not publish** to external services without explicit user approval.
- Keep the project inside the working folder.

## Quick Reference

| Task | Command / Action |
|------|------------------|
| Open site | `start index.html` (Windows) / `open index.html` (macOS) |
| Run local server | `python -m http.server 8000` |
| Check status | `git status` |
| Push changes | `git add . && git commit -m "..." && git push origin main` |
| GitHub repo | https://github.com/NataKl/yoga-website |
