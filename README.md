# 🌸 The "Tech-Girlie" Modern Engineering Portfolio Guide

An ultra-modern, aesthetic engineering portfolio designed to showcase high-impact enterprise architecture, machine learning research, and open-source contributions—all styled in an ultra-realistic, futuristic cyber-rose aesthetic.

---

## 📖 How to Build a Modern Tech Portfolio: The Strategy

If you are an engineer looking to build or revamp your portfolio, standard developer templates with generic contribution graphs often fall short. This portfolio implements key architectural and UX patterns tailored to today's hiring landscape:

### 1. Solving the "Enterprise Engineer Paradox"
* **The Problem:** Once you enter enterprise environments or consult on proprietary systems, your daily commits live inside private enterprise tenants (Azure DevOps, GitLab, private repos). A public GitHub heatmap can make you look inactive when you are actually shipping high-scale code3].
* **The Solution:** Decouple your production work from open source.
  * **Flagship Spotlights:** Highlight multi-disciplinary wins (e.g., international hackathon placements, peer-reviewed publications)[cite: 1].
  * **Dedicated Enterprise Section:** Showcase closed-source projects with architectural breakdowns, workflow descriptions, and business outcomes without violating non-disclosure agreements.
  * **Dynamic GitHub Integration:** Feature a handpicked selection of key public repositories, backed by a live API query that fetches the rest of your public catalog on demand.

### 2. High-Converting Visual Identity
* **Personality + Technical Precision:** Blending clean typography (`Space Grotesk`, `Plus Jakarta Sans`, and `JetBrains Mono`) with subtle cyber-pink glassmorphism, animated ambient lighting orbs, and interactive background particle networks.
* **Instant Multi-Theme System:** Ships with three distinct themes toggled by CSS data-attributes (`Cyber Rose 💖`, `Orchid Dark 🔮`, and `Blush Silk 🌸`).
* **Direct Proof of Credentials:** Clean bento grids for corporate internships, certified learning paths (AWS, Oracle, McKinsey), and social impact initiatives.

---

## 📂 Information Architecture Overview

```text
├── Hero Section
│   ├── Production Role Badge & Identity
│   └── High-intent CTA buttons linking to Flagships & Enterprise Systems
├── Flagship Innovations
│   ├── UniPay (Campus Digital Banking — Citi Runner-Up)
│   ├── Enhancing Generative AI with RAG (Springer Publication)
│   └── Enterprise Process Automation & Copilot Orchestration (Computacenter)
├── Enterprise Projects
│   └── Dedicated cards for internal automation, ETL pipelines & ITSM tools
├── Open-Source Repositories (GitHub Dynamic Section)
│   ├── 3 Curated Spotlight Repositories (Standard Chartered assistant, Profanity Detector, Microfinance Dashboard)
│   └── "Show All Repositories & More" Button (live-loads remaining public repos via GitHub REST API)
├── Internships & Professional Roles
│   └── Timeline of production roles and industry internships
├── Certifications & Executive Programs
│   └── Verified credentials grid + deep link to LinkedIn certifications
├── Volunteer Work & Social Impact
│   └── Community outreach, NGO initiatives, and university societies
└── Contact & Socials

```

---

## 🚀 How to Set Up & Customize This Portfolio

### 1. Cloning or Saving the File

Save the provided HTML code as `index.html` in your project folder:

```bash
git init my-portfolio
cd my-portfolio
# Paste index.html into the root directory

```

### 2. Updating Personal & API Details

Open `index.html` and customize the data points:

* **GitHub Username:** Search for `Shrinjita` in the script tag and replace it with your GitHub handle to point the API fetcher to your public repos.


* **Spotlight Repositories:** In the `featuredRepoNames` JavaScript array, update the 3 repository slug names you want pinned by default:


```javascript
const featuredRepoNames = [
  'Your-Repo-One',
  'Your-Repo-Two',
  'Your-Repo-Three'
];

```

* **Enterprise Projects:** In the `enterpriseProjects` array, add or modify project cards as your corporate responsibilities grow:

```javascript
{
  badge: 'Enterprise Production · Company Name',
  title: 'Project Title',
  timeline: 'Date Range',
  desc: 'Description of your architecture, process optimization, and impact.',
  tech: 'Tools · Frameworks · Platforms'
}

```
* **Showcase Cards:** Edit the static cards under `#flagship` to reflect your top 3 career highlights.
* **Social Links:** Replace the LinkedIn, GitHub, Medium, and mailto URLs in the footer and navigation with your own profiles.

### 3. Deploying to Vercel or GitHub Pages

#### Option A: Vercel (Recommended)

1. Push your repository to GitHub.
2. Go to [Vercel](https://vercel.com/) and click **Add New > Project**.
3. Import your GitHub repository.
4. Leave all build settings default (Root Directory: `./`, Framework: `Other`).
5. Click **Deploy**. Your portfolio will be live on a custom `.vercel.app` URL with automatic SSL.

#### Option B: GitHub Pages

1. Push the codebase to a GitHub repository.
2. Go to **Settings > Pages**.
3. Under **Branch**, select `main` (or `master`) and folder `/ (root)`.
4. Click **Save**. Your site will be published at `https://<username>.github.io/<repo-name>/`.
