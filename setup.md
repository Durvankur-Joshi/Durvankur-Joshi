# 🛠️ GitHub Profile Setup & Deployment Guide

Welcome to your redesigned developer landing page README for **Durvankur Joshi** (`AI Engineer & Full-Stack Developer`).

---

## 📋 Table of Contents
1. [Repository Setup](#1-repository-setup)
2. [Section Hierarchy](#2-section-hierarchy)
3. [Configuring GitHub Actions Workflows](#3-configuring-github-actions-workflows)
   - [A. Contribution Snake Animation (`snake.yml`)](#a-contribution-snake-animation-snakeyml)
   - [B. 3D Contribution Matrix (`3d-contrib.yml`)](#b-3d-contribution-matrix-3d-contribyml)
4. [Replacing Placeholders](#4-replacing-placeholders)
5. [Deploying & Syncing Profile Changes](#5-deploying--syncing-profile-changes)

---

## 1. Repository Setup

GitHub displays your profile README when it is located in a special public repository with the exact same name as your GitHub username (`Durvankur-Joshi/Durvankur-Joshi`).

1. Go to [GitHub New Repository](https://github.com/new).
2. Set **Repository name** to `Durvankur-Joshi`.
3. Set visibility to **Public**.
4. Check **Add a README file** (or leave it unchecked if pushing this existing workspace).
5. Push this workspace:
   ```bash
   git init
   git add .
   git commit -m "feat: launch redesigned AI engineer landing page"
   git branch -M main
   git remote add origin https://github.com/Durvankur-Joshi/Durvankur-Joshi.git
   git push -u origin main
   ```

---

## 2. Section Hierarchy

Your README follows a clean 10-step landing page hierarchy:

1. **HERO** &rarr; Centered name focal point, typing line (`readme-typing-svg`), domain pills, HUD telemetry.
2. **ABOUT / CURRENT MISSION** &rarr; Core background + compact `BUILD → EXPLORE → LEARN → SHIP` mission row.
3. **FEATURED PROJECTS** &rarr; Product cards for **MedVault**, **AI Debugging Agent**, **AI Software Compiler**, **ChatFusion**, and **CodeX**.
4. **TECH STACK** &rarr; Categorized stack (*Languages, AI/GenAI, Frontend, Backend, Database/Cloud, Web3, Tools*).
5. **SYSTEM ARCHITECTURE** &rarr; Clean ASCII architecture diagram modeling your engineering approach.
6. **HACKATHONS & ACHIEVEMENTS** &rarr; Web Wizard Hackathon Winner, HackNexus'26, and Web Development Domain Head.
7. **GITHUB COMMAND CENTER** &rarr; Tokyo-night themed Stats, Streaks, and Top Languages.
8. **3D CONTRIBUTION + SNAKE** &rarr; Automated 3D contribution matrix and Snake game animation.
9. **CURRENTLY BUILDING** &rarr; Active product development focus block.
10. **CONNECT** &rarr; Social action buttons and profile view counter.

---

## 3. Configuring GitHub Actions Workflows

### Enable Workflow Permissions
1. In your GitHub repository, go to **Settings** &rarr; **Actions** &rarr; **General**.
2. Scroll to **Workflow permissions**.
3. Select **Read and write permissions**.
4. Check **Allow GitHub Actions to create and approve pull requests**.
5. Click **Save**.

### A. Contribution Snake Animation (`snake.yml`)
- Located at `.github/workflows/snake.yml`.
- Runs automatically daily at 00:00 UTC and generates the snake SVG to the `output` branch.
- To trigger manually: Go to **Actions** tab &rarr; select **Generate Contribution Snake Animation** &rarr; click **Run workflow**.

### B. 3D Contribution Matrix (`3d-contrib.yml`)
- Located at `.github/workflows/3d-contrib.yml`.
- Runs automatically daily at 00:00 UTC and generates 3D contribution SVGs into the `profile-3d-contrib/` folder.
- To trigger manually: Go to **Actions** tab &rarr; select **Generate 3D Contribution Matrix** &rarr; click **Run workflow**.

---

## 4. Replacing Placeholders

Search and replace the following placeholder strings across `README.md` if needed:

| Placeholder | Description | Example |
|---|---|---|
| `Durvankur-Joshi` | Your LinkedIn handle | `durvankur-joshi` |
| `YOUR_PORTFOLIO` | Your personal portfolio URL | `durvankur.dev` |
| `joshidurvankur.29@gmail.com` | Your professional contact email | `joshidurvankur.29@gmail.com` |
| `medvault-umber.vercel.app` | Live demo URL for MedVault | `https://medvault-demo.vercel.app` |

---

## 5. Deploying & Syncing Profile Changes

```bash
git add .
git commit -m "update: refresh developer profile metrics and projects"
git push origin main
```

Your GitHub profile updates immediately upon push! 🚀
