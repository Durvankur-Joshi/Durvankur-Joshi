# 🛠️ GitHub Profile Setup & Customization Guide

Welcome to your redesigned, modern futuristic GitHub profile README! This guide explains how to deploy your profile, customize placeholders, configure the contribution snake workflow, and maintain stats.

---

## 📋 Table of Contents
1. [Repository Setup](#1-repository-setup)
2. [Replacing Placeholders](#2-replacing-placeholders)
3. [Enabling the Contribution Snake Workflow](#3-enabling-the-contribution-snake-workflow)
4. [Customizing the Hero Banner](#4-customizing-the-hero-banner)
5. [Customizing Tech Stack & Badges](#5-customizing-tech-stack--badges)
6. [Updating GitHub Analytics & Activity Graph](#6-updating-github-analytics--activity-graph)
7. [Deploying & Syncing Profile Changes](#7-deploying--syncing-profile-changes)

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
   git commit -m "feat: redesign modern futuristic GitHub profile"
   git branch -M main
   git remote add origin https://github.com/<YOUR_GITHUB_USERNAME>/<YOUR_GITHUB_USERNAME>.git
   git push -u origin main
   ```

---

## 2. Replacing Placeholders

Search and replace the following placeholder strings across `README.md`:

| Placeholder | Description | Example |
|---|---|---|
| `YOUR_GITHUB_USERNAME` | Your exact GitHub username | `Durvankur-Joshi` |
| `YOUR_LINKEDIN` | Your LinkedIn username/handle | `durvankur-joshi` |
| `YOUR_PORTFOLIO` | Your personal portfolio URL | `durvankur.dev` |
| `YOUR_EMAIL` | Your professional contact email | `joshidurvankur.29@gmail.com` |
| `YOUR_LIVE_DEMO_LINK` | Live demo URL for MedVault | `https://medvault-demo.vercel.app` |

> 💡 **Quick search & replace in VS Code / IDE:**
> Press `Ctrl + Shift + H` (or `Cmd + Shift + H` on Mac), search for `YOUR_GITHUB_USERNAME`, and replace with your actual username across all files.

---

## 3. Enabling the Contribution Snake Workflow

The contribution snake animation runs automatically every 24 hours via GitHub Actions and commits the generated SVG to the `output` branch.

### Step 1: Enable GitHub Actions Permissions
1. In your profile repository on GitHub, go to **Settings** &rarr; **Actions** &rarr; **General**.
2. Under **Workflow permissions**, select **Read and write permissions**.
3. Check the box **Allow GitHub Actions to create and approve pull requests**.
4. Click **Save**.

### Step 2: Trigger the Workflow Manually
1. Go to the **Actions** tab in your repository.
2. Select **Generate Contribution Snake Animation** in the left sidebar.
3. Click the **Run workflow** dropdown button on the right &rarr; click **Run workflow**.
4. Once completed (approx 30–45 seconds), it will automatically create the `output` branch with the generated snake SVGs.
5. Refresh your GitHub profile page — your contribution snake is now live!

---

## 4. Customizing the Hero Banner

The hero banner is located at [`assets/hero.svg`](assets/hero.svg).

- **Animated Typing Line**: Contains smooth cycling SVG animations for:
  - *Agentic AI Engineer*
  - *Generative AI & RAG Systems*
  - *Full-Stack Applications*
  - *Web3 & Smart Contracts*
  - *🏆 Hackathon Winner & Builder*
- **Theme Colors**:
  - `#00F7FF` &rarr; Electric Cyan (Primary)
  - `#7F00FF` &rarr; Cyber Purple (Secondary)
  - `#00FFA3` &rarr; Mint Accent (Accent)
  - `#050816` &rarr; Deep Space Background

---

## 5. Customizing Tech Stack & Badges

The Tech Stack section uses [Skill Icons](https://skillicons.dev) and curated shields.io badges:
- To add or remove icons from the skillicons URL, simply modify the `i=` query parameter (e.g. `i=python,js,ts,react,nextjs,tailwind,fastapi,postgres,docker`).

---

## 6. Updating GitHub Analytics & Activity Graph

The GitHub Analytics cards are styled with Tokyo-Night matching the cyber dark theme:
- `github-readme-stats` &rarr; Stats card & top languages
- `github-readme-streak-stats` &rarr; Continuous streak tracker
- `github-readme-activity-graph` &rarr; Interactive activity visualizer

---

## 7. Deploying & Syncing Profile Changes

Whenever you update `README.md`, assets, or projects:

```bash
git add .
git commit -m "update: refresh profile metrics and project showcase"
git push origin main
```

Your GitHub profile updates instantly upon pushing to `main`! 🚀
