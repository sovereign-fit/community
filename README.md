# Sovereign Fit Community ⚡

The open-source community hub for fitness trainers and wellness professionals.

**[→ Visit the live site](https://sovereign-fit.github.io/community)**

---

## What Is This?

**Sovereign Fit** is a weekly newsletter and community designed for fitness trainers and wellness professionals who want to stop trading time for money. Each issue follows the **5-Reps Format**:

1. 🎯 **The Hook** — A real business problem, broken down fast
2. 💼 **Business Tip #1** — Tactical marketing, pricing, or automation advice
3. 💼 **Business Tip #2** — A second business play to implement this week
4. 🧠 **Coaching Concept #1** — Behavioral science for better client retention
5. 🧠 **Coaching Concept #2** — Longevity or wellness research insights

Plus a curated tool recommendation, an inspirational quote, and a feedback poll.

## Tech Stack

- **Jekyll** — Static site generator (GitHub Pages native)
- **GitHub Pages** — Free, fast hosting with HTTPS
- **Giscus** — GitHub-based commenting (anti-bot by design)
- **Systeme.io** — Email capture and welcome sequence

## Publishing Workflow

1. Write your issue using the template in `_templates/5-reps-template.md`
2. Save it to `_posts/` with the filename format: `YYYY-MM-DD-your-title.md`
3. **VIP Delay Rule**: Only publish to GitHub **one week after** sending to your Systeme.io email list
4. Commit and push — GitHub Pages builds automatically

## Commenting System

Comments use [Giscus](https://giscus.app/), which requires commenters to sign in with a free GitHub account. This acts as a natural anti-bot filter while keeping content fully accessible to all readers.

## Setup Instructions

### 1. Enable GitHub Pages
- Go to **Settings → Pages** in this repository
- Set the source to **Deploy from a branch** → `main` / `/ (root)`
- Save

### 2. Connect Systeme.io
- Create your opt-in form in Systeme.io
- Copy the form action URL
- Replace the `action="#"` in `index.html` (both subscribe forms) with your Systeme.io endpoint

### 3. Enable Giscus Comments
1. Visit [giscus.app](https://giscus.app/)
2. Enter `sovereign-fit/community` as the repository
3. Enable **Discussions** on this repo (Settings → General → Features → Discussions)
4. Create a discussion category called "Newsletter Discussion"
5. Copy the `repo-id` and `category-id` from giscus.app
6. Update `_config.yml` with those values

### 4. Custom Domain (Optional)
- Purchase a domain from Namecheap or GoDaddy
- Add a `CNAME` file with your domain name
- Configure DNS to point to GitHub Pages
- HTTPS is auto-provisioned

## File Structure

```
community/
├── _config.yml          # Jekyll configuration
├── _layouts/
│   ├── default.html     # Base layout (nav, footer)
│   └── post.html        # Newsletter issue layout (poll, comments)
├── _posts/              # Published newsletter issues
│   └── 2026-03-08-why-most-fitness-businesses-plateau.md
├── _templates/
│   └── 5-reps-template.md  # Template for new issues
├── assets/
│   ├── css/main.css     # Complete design system
│   └── img/favicon.svg  # Site favicon
├── index.html           # Homepage with subscribe form
├── archive.html         # Newsletter archive page
├── about.html           # About page
├── Gemfile              # Ruby dependencies
└── README.md            # This file
```

## License

CC0-1.0 — Public Domain

---

Built with ⚡ by the Sovereign Fit community.
