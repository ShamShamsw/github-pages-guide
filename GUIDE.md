# 📘 Beginner's Guide to Setting Up GitHub Pages

> **Purpose:** A complete, beginner-friendly walkthrough for creating your first GitHub Pages website — no coding experience required!

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

## 📚 SECTION 7 — Additional Resources

### Official GitHub Documentation
- [Quickstart for GitHub Pages](https://docs.github.com/en/pages/quickstart)
- [Creating a GitHub Pages site with Jekyll](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/creating-a-github-pages-site-with-jekyll)
- [Configuring a custom domain for your GitHub Pages site](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)
- [Troubleshooting custom domains and GitHub Pages](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/troubleshooting-custom-domains-and-github-pages)
- [Licensing a repository](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/licensing-a-repository)
- [Adding a license to a repository](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/adding-a-license-to-a-repository)

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

© 2026 ShamShamsw / Jacob Haseman. This guide is licensed under the [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

You are free to:
- **Share** — copy and redistribute the material
- **Adapt** — remix, transform, and build upon the material

Under the following terms:
- **Attribution** — You must give appropriate credit, provide a link to the license, and indicate if changes were made.
