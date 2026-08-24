# 🛠️ GitHub Profile Setup & Deployment Guide

Welcome to your custom, high-tech GitHub profile README! This guide details how to deploy your profile, customize parameters, enable automated animations, and personalize all links.

---

## 📋 Table of Contents
1. [Repository Setup (Special Profile Repo)](#1-repository-setup)
2. [Profile Structure Overview](#2-profile-structure-overview)
3. [Replacing Placeholders](#3-replacing-placeholders)
4. [Enabling the Contribution Snake Animation](#4-enabling-the-contribution-snake-animation)
5. [Customizing the 3D Tech Sphere SVG](#5-customizing-the-3d-tech-sphere-svg)
6. [Customizing the Hero Banner & Header](#6-customizing-the-hero-banner--header)
7. [Updating & Customizing GitHub Stats](#7-updating--customizing-github-stats)
8. [Deploying & Syncing Profile Changes](#8-deploying--syncing-profile-changes)

---

## 1. Repository Setup

GitHub displays your profile README when it is located in a special public repository with the exact same name as your GitHub username.

1. Go to [GitHub New Repository](https://github.com/new).
2. Set **Repository name** to your exact GitHub username (e.g. `Durvankur-Joshi`).
3. Set visibility to **Public**.
4. Check **Add a README file** (or leave it unchecked if pushing this existing folder).
5. Clone or push this workspace repository to your GitHub repository:
   ```bash
   git init
   git add .
   git commit -m "feat: initialize futuristic cyber GitHub profile"
   git branch -M main
   git remote add origin https://github.com/<YOUR_GITHUB_USERNAME>/<YOUR_GITHUB_USERNAME>.git
   git push -u origin main
   ```

---

## 2. Profile Structure Overview

Your profile is organized into 10 structured sections:

```text
HERO
 ↓
ABOUT ME
 ↓
WHAT I BUILD
 ↓
TECH STACK
 ↓
FEATURED PROJECTS
 ↓
HACKATHON / ACHIEVEMENTS
 ↓
GITHUB CONTRIBUTIONS
 ↓
GITHUB STATS
 ↓
CURRENTLY LEARNING
 ↓
CONNECT WITH ME
```

---

## 3. Replacing Placeholders

Search and replace the following placeholder strings across `README.md` and `.github/workflows/snake.yml`:

| Placeholder | Description | Example |
|---|---|---|
| `YOUR_GITHUB_USERNAME` | Your exact GitHub username | `Durvankur-Joshi` |
| `YOUR_LINKEDIN` | Your LinkedIn profile handle or URL | `durvankur-joshi` |
| `YOUR_PORTFOLIO` | Your personal portfolio URL | `durvankur.dev` or `durvankurjoshi.vercel.app` |
| `YOUR_EMAIL` | Your professional contact email | `joshidurvankur.29@gmail.com` |

> 💡 **Quick search & replace in VS Code / IDE:**
> Press `Ctrl + Shift + H` (or `Cmd + Shift + H` on Mac), search for `YOUR_GITHUB_USERNAME`, and replace with your actual username across all files.

---

## 4. Enabling the Contribution Snake Animation

The contribution snake game eats your green contribution tiles and automatically compiles an SVG image every 24 hours via GitHub Actions.

### Step 1: Enable GitHub Actions Workflow Permissions
1. Go to your profile repository on GitHub (`https://github.com/<YOUR_GITHUB_USERNAME>/<YOUR_GITHUB_USERNAME>`).
2. Click **Settings** (top tab) &rarr; **Actions** (left sidebar) &rarr; **General**.
3. Scroll down to **Workflow permissions**.
4. Select **Read and write permissions**.
5. Check the box **Allow GitHub Actions to create and approve pull requests**.
6. Click **Save**.

### Step 2: Trigger the Workflow Manually
1. Go to the **Actions** tab in your repository.
2. Select **Generate Contribution Snake Animation** in the left sidebar.
3. Click the **Run workflow** dropdown button on the right &rarr; click **Run workflow**.
4. Once the action finishes running (approx 30–60 seconds), it will automatically create an `output` branch with the generated SVGs (`github-contribution-grid-snake-dark.svg`).
5. Refresh your GitHub profile page — your contribution snake will now be live!

---

## 5. Customizing the 3D Tech Sphere SVG

The 3D orbital tech sphere is located at [`assets/tech-sphere.svg`](assets/tech-sphere.svg).

### Modifying Technology Labels
Open `assets/tech-sphere.svg` in your editor and look for the orbital node groups:
- Lines with `<text ...>PYTHON</text>`, `REACT`, `NEXT.JS`, `FASTAPI`, `LANGCHAIN`, `SOLIDITY`, `SUPABASE`, `NODE.JS`.
- You can change the text content to any technology you want (e.g. `PYTORCH`, `GRAPHQL`, `RUST`, `GO`, `DOCKER`).

### Adjusting Colors & Theme
The color palette is defined in the `<defs>` section of `assets/tech-sphere.svg`:
- `#00F7FF` &rarr; Electric Cyan (Primary)
- `#7F00FF` &rarr; Neon Cyber Purple (Secondary)
- `#00FFA3` &rarr; Neon Mint Green (Accent)
- `#050816` &rarr; Deep Space Background

### Adjusting Orbital Speed
Look for `dur="24s"` in `<animateTransform>` tags.
- Decreasing the duration (e.g. `dur="16s"`) makes the orbit faster.
- Increasing the duration (e.g. `dur="36s"`) makes the orbit slower and smoother.

---

## 6. Customizing the Hero Banner & Header

The dynamic animated header is located at [`assets/hero-banner.svg`](assets/hero-banner.svg).

- **Typing / Role Switcher**: Contains cycling animated SVG text spans for your roles:
  - *Building Autonomous AI Agents & RAG*
  - *Deploying Web3 & Zero-Knowledge DApps*
  - *Crafting Full-Stack & Real-time Systems*
  - *🏆 Winner: Web Wizard Hackathon*
- **Status Telemetry**: You can edit the top and bottom telemetry pills to reflect your active graduation year or university department.

---

## 7. Updating & Customizing GitHub Stats

The stats cards in `README.md` are powered by `github-readme-stats` and `github-readme-streak-stats` with matching custom hex parameters:

```markdown
https://github-readme-stats.vercel.app/api?username=YOUR_GITHUB_USERNAME&show_icons=true&theme=tokyonight&bg_color=050816&title_color=00F7FF&text_color=F5F7FF&icon_color=00FFA3&border_color=1f2d6e&hide_border=false&count_private=true&include_all_commits=true
```

### Options:
- **Private Contributions**: By default, `count_private=true` is set.
- **Hide Specific Repos / Languages**: Add `&hide=html,css` to the `top-langs` URL if you only want to highlight backend / smart-contract languages.
- **Self-Hosting (Recommended for 100% uptime)**: If GitHub's public API rate-limits the stats cards, you can deploy your own 1-click Vercel instance following the [github-readme-stats deployment guide](https://github.com/anuraghazra/github-readme-stats#deploy-on-your-own-vercel-instance).

---

## 8. Deploying & Syncing Profile Changes

Whenever you update `README.md`, assets, or projects:

```bash
git add .
git commit -m "update: refresh profile metrics and project showcase"
git push origin main
```

Your GitHub profile updates instantly upon pushing to `main`! 🚀
