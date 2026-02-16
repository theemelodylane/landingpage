# Melody Lane Landing Page - Setup Notes

## Overview
Single-page landing site for Melody Lane (theemelodylane.com) linking to socials and Telegram bot.

---

## Domain
- **URL**: https://theemelodylane.com
- **Registrar**: (your registrar - Cloudflare managing DNS)

---

## GitHub Repository
- **Repo**: https://github.com/theemelodylane/landingpage
- **Branch**: main
- **GitHub Pages**: Enabled, deploying from main branch root

---

## DNS Configuration (Cloudflare)
**A Records pointing to GitHub Pages:**
```
theemelodylane.com → 185.199.108.153
theemelodylane.com → 185.199.109.153
theemelodylane.com → 185.199.110.153
theemelodylane.com → 185.199.111.153
```

**SSL/TLS Setting**: Full (not Full Strict - needed for GitHub Pages compatibility)

---

## File Structure
```
melodylane-landing/
├── index.html              # Main landing page
└── images/
    ├── melody-profile.jpg  # Hero image (your Instagram photo)
    └── telegram-...jpg     # Additional image asset
```

---

## Page Sections
1. **Hero**: Profile image, name, tagline, description, CTAs
2. **Social Links**: YouTube, Instagram, Twitter/X, Threads (2x2 grid)
3. **Telegram CTA**: Prominent bot link section
4. **Footer**: Copyright, quick links

---

## Active Links (all open in new tab)
| Platform | URL |
|----------|-----|
| YouTube | https://www.youtube.com/@TheeMelodyLane |
| Instagram | https://www.instagram.com/theemelodylane/ |
| Twitter/X | https://x.com/Theemelodylane |
| Threads | https://www.threads.com/@theemelodylane |
| Telegram Bot | https://t.me/theemelodylanebot |

---

## Content
- **Tagline**: "CLE born & raised. Sports fanatic. Horror movie lover. Music enthusiast. Let's chat!"
- **Description**: "Subscribe for exclusive content you won't find anywhere else. Spoiler-free reviews, hot takes, and a peek behind the curtain."

---

## Design
- Dark gradient background (#1a1a2e → #16213e → #0f3460)
- Pink accent color (#ff006e)
- Circular hero image (280x280px, 1:1 ratio)
- Responsive grid layout

---

## SSH Key for GitHub
- Location: `~/.ssh/id_theemelodylane`
- Added to GitHub account: theemelodylane
- Used for pushing updates to repo

---

## How to Update
```bash
cd ~/melodylane-landing
# Edit files...
git add .
git commit -m "Description of changes"
GIT_SSH_COMMAND="ssh -i ~/.ssh/id_theemelodylane" git push
```
Changes go live in ~1-2 minutes automatically via GitHub Pages.

---

## Future Additions
- Polls folder: `melodylane-landing/polls/poll-001.html`
- Newsletter signup page
- Links page (Linktree style)
- All pages should include Telegram CTA at bottom

---

## Notes
- Images: Use 1:1 square ratio for hero, min 280x280px
- All external links have `target="_blank" rel="noopener"` 
- Copyright year: 2026
- Created: Feb 15, 2025
