# 📘 Beginner's Guide to Setting Up GitHub Pages

> **Purpose:** A complete, beginner-friendly walkthrough for creating your first GitHub Pages website — no coding experience required!

---

## 📑 Table of Contents

- [🏷️ Welcome!](#️-welcome)
- [✅ SECTION 1 — What is GitHub Pages?](#-section-1--what-is-github-pages)
- [🛠️ SECTION 2 — Creating Your First GitHub Pages Site](#️-section-2--creating-your-first-github-pages-site-step-by-step)
  - [Step 1 — Create a New Repository](#step-1--create-a-new-repository)
  - [Step 2 — Enable GitHub Pages](#step-2--enable-github-pages)
  - [Step 3 — Visit Your Live Site](#step-3--visit-your-live-site)
- [✏️ SECTION 3 — Customizing Your Site](#️-section-3--customizing-your-site)
  - [3A. Changing the Title & Description](#3a-changing-the-title--description)
  - [3B. Adding a Custom index.html](#3b-adding-a-custom-indexhtml)
  - [3C. Choosing a Jekyll Theme](#3c-choosing-a-jekyll-theme-no-coding-required)
- [🌐 SECTION 4 — (Optional) Setting Up a Custom Domain](#-section-4--optional-setting-up-a-custom-domain)
- [❓ SECTION 5 — Frequently Asked Questions (FAQ)](#-section-5--frequently-asked-questions-faq)
- [🔒 SECTION 6 — Licensing & Intellectual Property](#-section-6--licensing--intellectual-property-important)
- [💻 SECTION 7 — Recommended Languages & Technologies](#-section-7--recommended-languages--technologies-for-github-pages)
  - [Core Languages](#core-languages-essential)
  - [Static Site Generators](#static-site-generators-advanced)
  - [Front-End Frameworks & Libraries](#front-end-frameworks--libraries-client-side-only)
  - [What GitHub Pages Does NOT Support](#what-github-pages-does-not-support)
- [🎨 SECTION 8 — Cool Add-Ons, Tools & Integrations](#-section-8--cool-add-ons-tools--integrations-for-github-pages)
  - [Content Management Systems](#content-management-systems-cms)
  - [Analytics & Metrics](#analytics--metrics)
  - [Forms & User Input](#forms--user-input)
  - [Search Functionality](#search-functionality)
  - [Comments & Community](#comments--community)
  - [SEO & Performance](#seo--performance)
  - [Design Resources](#design-resources)
- [📚 SECTION 9 — Official GitHub Documentation & Resources](#-section-9--official-github-documentation--resources)
- [🎉 Congratulations!](#-congratulations)
- [📝 License & Attribution](#-license--attribution)

---

## 🏷️ Welcome!

**GitHub Pages** is a free hosting service by GitHub that lets you turn a repository into a live website, accessible at `https://yourusername.github.io`.

### What You'll Learn
By the end of this guide, you'll know how to:
- ✅ Create a GitHub Pages site from scratch
- ✅ Customize your site with themes and HTML
- ✅ Configure a custom domain (optional)
- ✅ Troubleshoot common issues

### Who This Guide Is For
Complete beginners! No coding, web development, or Git experience required.

### Prerequisites
- A **GitHub account** (free at [github.com](https://github.com))
- A **web browser**
- *(Optional for advanced sections)*: Git installed locally

---

## ✅ SECTION 1 — What is GitHub Pages?

**GitHub Pages** hosts static websites directly from a GitHub repository.

### Common Use Cases
- 📁 **Portfolios** — Showcase your work and projects
- 📝 **Project Documentation** — Host docs for open-source projects
- ✍️ **Blogs** — Share your thoughts and tutorials
- 📄 **Resumes** — Create an online CV
- 🎨 **Landing Pages** — Build simple promotional sites

### Key Features
- ✅ **100% Free** for public repositories on GitHub Free plans
- ✅ Works with private repositories on **GitHub Pro, Team, Enterprise Cloud/Server**
- ✅ Default URL format: `https://username.github.io`
- ✅ Supports custom domains (e.g., `www.yourname.com`)

> 📝 **Note:** GitHub Pages only hosts **static** content (HTML, CSS, JavaScript). It does not support server-side languages like PHP or Python backends.

---

## 🛠️ SECTION 2 — Creating Your First GitHub Pages Site (Step-by-Step)

### Step 1 — Create a New Repository

1. In the upper-right corner of GitHub, click the **"+"** button → **"New repository"**
2. **Repository name:** Enter `yourusername.github.io`
   - Replace `yourusername` with your actual GitHub username
   - **Example:** If your username is `shamshamsw`, name it `shamshamsw.github.io`
3. Set visibility to **Public**
4. ✅ Check **"Add a README file"**
5. Click **"Create repository"**

> 📝 **Note:** The repository name **must exactly match** your username followed by `.github.io` — otherwise GitHub Pages won't activate it as a user site.

---

### Step 2 — Enable GitHub Pages

1. Go to your new repository
2. Click **"Settings"** (gear icon in the top menu)
3. In the left sidebar, under **"Code and automation"**, click **"Pages"**
4. Under **"Build and deployment"** → **"Source"**, select **"Deploy from a branch"**
5. Under **"Branch"**, select `main` (or `master`) and click **"Save"**

> 📝 **Note:** It can take **up to 10 minutes** for your site to go live after saving. Be patient!

---

### Step 3 — Visit Your Live Site

1. After saving, go back to **Settings → Pages**
2. You'll see a banner: *"Your site is live at `https://yourusername.github.io`"*
3. Click the link or open it in a new tab

> 📝 **Note:** By default, your site will display the content of your `README.md` file. You can later replace this with a custom `index.html`.

---

## ✏️ SECTION 3 — Customizing Your Site

### 3A. Changing the Title & Description

1. In your repository, click **"Add file"** → **"Create new file"**
2. Name the file `_config.yml`
3. Add the following content:

```yaml
theme: jekyll-theme-minimal
title: Your Name's Website
description: Welcome to my personal GitHub Pages site!
```

4. Click **"Commit changes"** and wait for the site to rebuild (up to 10 minutes)

> 📝 **Note:** `_config.yml` uses a format called **YAML**. Indentation and spacing matter — use exactly 2 spaces, not tabs.

---

### 3B. Adding a Custom `index.html`

1. In your repository, click **"Add file"** → **"Create new file"**
2. Name the file `index.html`
3. Add basic HTML:

```html
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My GitHub Page</title>
</head>
<body>
    <h1>Hello World! 👋</h1>
    <p>Welcome to my GitHub Pages site.</p>
</body>
</html>
```

4. Click **"Commit changes"**

> 📝 **Note:** Once you add an `index.html`, it will take priority over the `README.md` as your homepage.

---

### 3C. Choosing a Jekyll Theme (No Coding Required)

1. Go to **Settings → Pages**
2. Click **"Choose a theme"**
3. Browse the available themes and click on one you like
4. Click **"Select theme"**
5. GitHub will automatically update your `_config.yml`

> 📝 **Note:** Jekyll themes are pre-built designs. You don't need to know how to code to use one. They work like website templates.

---

## 🌐 SECTION 4 — (Optional) Setting Up a Custom Domain

**For users who want `www.yourname.com` instead of `yourname.github.io`:**

### Prerequisites
- Purchase a domain from a registrar (e.g., Namecheap, Google Domains, GoDaddy, Cloudflare)

### Steps

1. Go to **Settings → Pages** in your repository
2. Under **"Custom domain"**, type your domain (e.g., `www.yourname.com`) and click **"Save"**
3. In your domain registrar's DNS settings, add a **CNAME record**:
   - **Name/Host:** `www`
   - **Value/Points to:** `yourusername.github.io`
   - **TTL:** Automatic (or 3600)

4. **For apex domains** (`yourname.com` without `www`), add **A records** pointing to:
   ```
   185.199.108.153
   185.199.109.153
   185.199.110.153
   185.199.111.153
   ```

5. Wait up to **24–48 hours** for DNS to propagate
6. Once verified, enable **"Enforce HTTPS"** in Settings → Pages

> 📝 **Note:** Do not use wildcard DNS records (e.g., `*.yourname.com`) — these create security vulnerabilities and risk of domain takeover.

> 📝 **Note:** HTTPS may take up to **1 hour** to activate after DNS is configured.

---

## ❓ SECTION 5 — Frequently Asked Questions (FAQ)

| Question | Answer |
|----------|--------|
| **Is GitHub Pages free?** | Yes, for public repositories on GitHub Free. Private repos need GitHub Pro or higher. |
| **How long does it take for my site to go live?** | Up to 10 minutes after your first push or settings change. |
| **Why does my site show a 404 error?** | Make sure your repository is named `yourusername.github.io` exactly, Pages is enabled in Settings, and a valid `index.html` or `README.md` exists. |
| **Can I use my own domain name?** | Yes! You can set a custom domain in Settings → Pages and configure your DNS provider. |
| **Can I use JavaScript or CSS?** | Yes! GitHub Pages fully supports HTML, CSS, and JavaScript. |
| **Can I use a backend/server (PHP, Python, etc.)?** | No. GitHub Pages only serves **static** files. For backend needs, consider services like Vercel, Netlify, or Railway. |
| **My changes aren't showing up — why?** | Wait up to 10 minutes. Also try clearing your browser cache (Ctrl+Shift+R / Cmd+Shift+R). |
| **What is Jekyll?** | Jekyll is a static site generator supported by GitHub Pages. It lets you build blogs and sites using Markdown without writing raw HTML. |
| **Can I have multiple GitHub Pages sites?** | Each account gets one user site (`username.github.io`). But every repository can have its own **project site** at `username.github.io/repo-name`. |
| **Is my site visible to everyone?** | Yes — GitHub Pages sites are **public on the internet**, even if your repository is private (on supported plans). |

---

## 🔒 SECTION 6 — Licensing & Intellectual Property (IMPORTANT)

### Why a License Matters

> Without a license, **all rights are reserved by default** under copyright law. No one can legally use, copy, or modify your work. Adding a license makes your intent clear.

### ✅ Best License Choice for a Guide/Documentation Repo

**Creative Commons Attribution 4.0 International (CC BY 4.0)**

- ✅ Others **can** share, adapt, and build upon the work
- ✅ They **must credit** the original creator (you)
- ✅ Perfect for written guides, documentation, and educational content
- License keyword: `CC-BY-4.0`

### How to Add the License to Your Repository

1. Go to your repository's main page
2. Click **"Add file"** → **"Create new file"**
3. Name the file: `LICENSE` (all caps, no extension)
4. Click **"Choose a license template"**
5. Select **"Creative Commons Attribution 4.0 International"** (or your preferred license)
6. Fill in the year and your name
7. Click **"Commit changes"**

> 📝 **Note:** GitHub will automatically detect your license and display it in your repository's sidebar — making your IP protection visible to all visitors.

### Add a License Badge to Your README

```markdown
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
```

### Attribution Notice to Include in README

```
© 2026 ShamShamsw. This guide is licensed under the
Creative Commons Attribution 4.0 International License.
To view a copy of this license, visit https://creativecommons.org/licenses/by/4.0/
```

---

## � SECTION 7 — Recommended Languages & Technologies for GitHub Pages

GitHub Pages natively supports **static web technologies**. Here are the most popular and recommended options:

### Core Languages (Essential)

#### 1. **HTML (HyperText Markup Language)**
- ✅ **Required** for all websites
- Purpose: Structure and content
- Difficulty: ⭐ Beginner-friendly
- Example use: Creating pages, headings, paragraphs, links, images

#### 2. **CSS (Cascading Style Sheets)**
- ✅ **Highly recommended**
- Purpose: Styling, colors, layout, responsive design
- Difficulty: ⭐⭐ Easy to learn, powerful when mastered
- Example use: Custom fonts, colors, animations, mobile responsiveness

#### 3. **JavaScript (JS)**
- ✅ **Recommended** for interactivity
- Purpose: Dynamic behavior, user interactions, animations
- Difficulty: ⭐⭐⭐ Moderate learning curve
- Example use: Form validation, interactive galleries, dynamic content loading

### Static Site Generators (Advanced)

#### 1. **Jekyll** ⭐ Native GitHub Pages Support
- ✅ **Built-in** — no setup required on GitHub Pages
- Language: Ruby-based, uses Liquid templating
- Best for: Blogs, documentation, portfolios
- Features: Markdown support, themes, blog-aware
- Official docs: https://jekyllrb.com/docs/

#### 2. **Hugo** (Manual deployment required)
- Language: Go-based
- Best for: Lightning-fast site generation, large sites
- Difficulty: ⭐⭐⭐
- Note: Requires building locally and pushing to GitHub

#### 3. **Next.js Static Export** (Manual deployment)
- Language: React (JavaScript)
- Best for: Modern React apps, portfolios, single-page apps
- Difficulty: ⭐⭐⭐⭐
- Note: Export static HTML via `next export`

#### 4. **Gatsby** (Manual deployment)
- Language: React (JavaScript)
- Best for: Blazing-fast modern websites, portfolios
- Difficulty: ⭐⭐⭐⭐
- Note: Requires build step

### Front-End Frameworks & Libraries (Client-Side Only)

These work with GitHub Pages since they run in the browser:

- **React.js** — Component-based UI library
- **Vue.js** — Progressive JavaScript framework
- **Svelte** — Compiled framework, smaller bundles
- **Alpine.js** — Lightweight JavaScript framework
- **Tailwind CSS** — Utility-first CSS framework
- **Bootstrap** — Popular CSS framework for responsive design

### Markup Languages

- **Markdown** (.md) — Simple text formatting (supported by Jekyll)
- **MDX** — Markdown + JSX components (requires build tools)

### What GitHub Pages Does NOT Support

❌ **Server-side languages** (these require a backend server):
- PHP
- Python (Django, Flask)
- Ruby on Rails (backend)
- Node.js backend (Express.js, etc.)
- Java servlets
- ASP.NET backend

> **Workaround:** Use serverless functions (Netlify Functions, Vercel Edge Functions) or deploy backends separately (Railway, Render, Heroku)

---

## 🎨 SECTION 8 — Cool Add-Ons, Tools & Integrations for GitHub Pages

### Content Management Systems (CMS)

#### 1. **Netlify CMS** / **Decap CMS**
- Purpose: Add a visual editor to manage content (no code)
- Best for: Non-technical content editors
- Integration: Add config file + authentication
- Free tier: Yes
- Docs: https://decapcms.org/docs/

#### 2. **Forestry.io** (Now Tina CMS)
- Purpose: Git-based headless CMS
- Best for: Markdown-based sites (Jekyll, Hugo)
- Free tier: Yes
- Docs: https://tina.io/docs/

#### 3. **Sanity.io**
- Purpose: Structured content management
- Best for: Complex content models
- Free tier: Yes
- Docs: https://www.sanity.io/docs/

### Analytics & Metrics

#### 1. **Google Analytics 4 (GA4)**
- Track visitors, page views, user behavior
- Free tier: Yes (generous limits)
- Setup: Add tracking code to HTML `<head>`

#### 2. **Plausible Analytics**
- Privacy-friendly, lightweight alternative to Google Analytics
- Free tier: No (paid, but affordable)
- Docs: https://plausible.io/docs/

#### 3. **Umami**
- Self-hosted, open-source analytics
- Free tier: Yes (self-hosted)
- GitHub: https://github.com/umami-software/umami

### Forms & User Input

#### 1. **Formspree**
- Purpose: Add working contact forms without backend
- Free tier: 50 submissions/month
- Docs: https://formspree.io/

#### 2. **Netlify Forms**
- Purpose: Form handling (requires Netlify deployment)
- Free tier: 100 submissions/month
- Docs: https://docs.netlify.com/forms/setup/

#### 3. **Google Forms**
- Embed Google Forms directly into your page
- 100% free
- Docs: https://www.google.com/forms/about/

### Search Functionality

#### 1. **Algolia DocSearch**
- Purpose: Add instant search to documentation
- Free tier: Yes (for open-source projects)
- Best for: Documentation sites
- Docs: https://docsearch.algolia.com/

#### 2. **Lunr.js**
- Client-side search library (no backend needed)
- 100% free, open-source
- Best for: Small to medium sites
- GitHub: https://github.com/olivernn/lunr.js

### Comments & Community

#### 1. **Giscus**
- Purpose: Comments powered by GitHub Discussions
- Free tier: Yes (100% free)
- Best for: Developer blogs, open-source projects
- Docs: https://giscus.app/

#### 2. **Utterances**
- Purpose: Comments using GitHub Issues
- Free tier: Yes (100% free)
- Best for: Blogs, technical content
- GitHub: https://github.com/utterance/utterances

#### 3. **Disqus**
- Traditional comment system
- Free tier: Yes (with ads)
- Docs: https://disqus.com/

### SEO & Performance

#### 1. **Schema.org Markup**
- Purpose: Structured data for better search results
- Free: Yes
- Docs: https://schema.org/docs/gs.html

#### 2. **Open Graph Tags**
- Purpose: Better social media sharing previews
- Free: Yes
- Docs: https://ogp.me/

#### 3. **Cloudflare Pages**
- Alternative hosting with CDN, analytics, and performance boosts
- Free tier: Generous
- Docs: https://developers.cloudflare.com/pages/

### Icon Libraries

- **Font Awesome** — 2,000+ free icons
- **Bootstrap Icons** — Official Bootstrap icon library
- **Heroicons** — Tailwind-designed icons
- **Feather Icons** — Minimalist icon set

### Animation Libraries

- **AOS (Animate On Scroll)** — Scroll-triggered animations
- **GSAP** — Professional animation library
- **Animate.css** — Simple CSS animations
- **Lottie** — After Effects animations for web

### Utilities

#### 1. **giscus/utterances** (GitHub-based comments)
- See "Comments" section above

#### 2. **GitHub Actions for Automated Builds**
- Purpose: Automate deployments, testing, builds
- Free tier: 2,000 minutes/month (public repos unlimited)
- Docs: https://docs.github.com/en/actions

#### 3. **Shields.io Badges**
- Purpose: Add dynamic badges (build status, license, etc.)
- Free: Yes
- Docs: https://shields.io/

### Design Resources

- **Unsplash** — Free high-quality images
- **Pexels** — Free stock photos and videos
- **Google Fonts** — Free web fonts
- **Coolors.co** — Color palette generator

---

## 📚 SECTION 9 — Official GitHub Documentation & Resources

### 📖 Official GitHub Documentation (GitHub, Inc.)

> **Note:** All links below are official documentation from GitHub, Inc. and are subject to GitHub's copyright and terms of service.

#### Getting Started
- [Quickstart for GitHub Pages](https://docs.github.com/en/pages/quickstart) — Fast track to your first site
- [About GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/about-github-pages) — Core concepts and features
- [Creating a GitHub Pages site](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site) — Detailed setup guide

#### Jekyll & Themes
- [About GitHub Pages and Jekyll](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/about-github-pages-and-jekyll) — How Jekyll works with Pages
- [Creating a GitHub Pages site with Jekyll](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/creating-a-github-pages-site-with-jekyll) — Step-by-step Jekyll setup
- [Adding a theme to your GitHub Pages site using Jekyll](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/adding-a-theme-to-your-github-pages-site-using-jekyll) — Theme customization
- [Supported themes](https://pages.github.com/themes/) — Official theme gallery

#### Custom Domains & HTTPS
- [Configuring a custom domain for your GitHub Pages site](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site) — Complete domain setup guide
- [Managing a custom domain for your GitHub Pages site](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site) — DNS configuration
- [Verifying your custom domain for GitHub Pages](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/verifying-your-custom-domain-for-github-pages) — Domain verification
- [Troubleshooting custom domains and GitHub Pages](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/troubleshooting-custom-domains-and-github-pages) — Fix common DNS issues
- [Securing your GitHub Pages site with HTTPS](https://docs.github.com/en/pages/getting-started-with-github-pages/securing-your-github-pages-site-with-https) — Enable SSL certificates

#### Repository Management & Licensing
- [Licensing a repository](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/licensing-a-repository) — Choose the right license
- [Adding a license to a repository](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/adding-a-license-to-a-repository) — How to add LICENSE file

#### Advanced Configuration
- [Configuring a publishing source for your GitHub Pages site](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site) — Branch and folder options
- [Creating a custom 404 page for your GitHub Pages site](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-custom-404-page-for-your-github-pages-site) — User-friendly error pages
- [Unpublishing a GitHub Pages site](https://docs.github.com/en/pages/getting-started-with-github-pages/unpublishing-a-github-pages-site) — Take your site offline

#### GitHub Actions & Automation
- [GitHub Actions documentation](https://docs.github.com/en/actions) — Automate your workflow
- [Deploying to GitHub Pages](https://docs.github.com/en/actions/deployment/github-pages) — CI/CD for Pages

#### Limits & Best Practices
- [About GitHub Pages usage limits](https://docs.github.com/en/pages/getting-started-with-github-pages/about-github-pages#usage-limits) — Bandwidth, size restrictions
- [GitHub Pages best practices](https://docs.github.com/en/pages/getting-started-with-github-pages/about-github-pages#best-practices) — Performance and SEO tips

### Other Helpful Resources
- [choosealicense.com](https://choosealicense.com) — Help choosing the right license
- [Jekyll Documentation](https://jekyllrb.com/docs/) — Learn more about Jekyll
- [Markdown Guide](https://www.markdownguide.org/) — Master Markdown syntax

---

## 🎉 Congratulations!

You've completed the guide! You now have the knowledge to:
- ✅ Create and deploy a GitHub Pages site
- ✅ Customize it with themes and custom HTML
- ✅ Configure custom domains
- ✅ Protect your work with proper licensing

**Ready to build something amazing? Start creating!** 🚀

---

## 📝 License & Attribution

**Copyright (c) 2026 ShamShamsw / Jacob Haseman**

This guide is licensed under the [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

You are free to:
- **Share** — copy and redistribute the material
- **Adapt** — remix, transform, and build upon the material

Under the following terms:
- **Attribution** — You must give appropriate credit, provide a link to the license, and indicate if changes were made.

---

### Important Disclaimers

**GitHub Intellectual Property Notice:**
GitHub, GitHub Pages, GitHub Actions, and all related trademarks, service marks, and logos are the intellectual property of GitHub, Inc. This guide is independently created educational content about using GitHub Pages and is not affiliated with, endorsed by, or sponsored by GitHub, Inc.

The copyright claim above applies solely to the original written content of this guide, not to GitHub's technology, documentation, or intellectual property.

**Official GitHub Documentation:**
All links to docs.github.com and pages.github.com are copyrighted by GitHub, Inc. and subject to GitHub's Terms of Service. Visit https://docs.github.com/en/site-policy for GitHub's official policies.
