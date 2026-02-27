# 📂 Example Templates & Starter Files

This folder contains ready-to-use examples to help you quickly start your GitHub Pages project.

---

## 📄 Files Included

### 1. **starter-template-index.html**
A complete, beginner-friendly HTML template for your first GitHub Pages site.

**Features:**
- ✅ Clean, modern design with gradient background
- ✅ Fully responsive (mobile-friendly)
- ✅ SEO-ready with meta tags
- ✅ Social media preview tags (Open Graph)
- ✅ Embedded CSS styling
- ✅ Simple JavaScript example
- ✅ Ready to customize

**How to use:**
1. Copy `starter-template-index.html` to your repository root
2. Rename it to `index.html`
3. Replace placeholder text with your own:
   - `[Your Name]` → Your actual name
   - `[your interests]` → Your passions/hobbies
   - `yourusername` → Your GitHub username
   - Project descriptions, skills, links, etc.
4. Commit and push to GitHub
5. Your site will be live at `https://yourusername.github.io`!

---

### 2. **starter-config.yml**
A comprehensive Jekyll configuration file with detailed comments explaining every option.

**Features:**
- ✅ All essential Jekyll settings
- ✅ Theme configuration
- ✅ Plugin setup (SEO, sitemap, feed)
- ✅ Social media integration
- ✅ SEO optimization settings
- ✅ Custom variables
- ✅ Extensive comments explaining each setting

**How to use:**
1. Copy `starter-config.yml` to your repository root
2. Rename it to `_config.yml`
3. Customize the settings:
   - Update `title`, `description`, `author`, `email`
   - Set your `url` and `baseurl`
   - Add your social media usernames
   - Choose a theme
   - Configure plugins as needed
4. Commit and push to GitHub
5. GitHub Pages will automatically use these settings

---

## 🚀 Quick Start Guide

### Option 1: HTML-Only Site (No Jekyll)
**Best for:** Complete beginners, simple one-page sites

1. Use `starter-template-index.html` as your `index.html`
2. Customize the content
3. Push to GitHub
4. Done! Your site is live.

**Pros:**
- ✅ Simple and straightforward
- ✅ No build process
- ✅ Instant updates

**Cons:**
- ❌ No templating (harder to maintain multiple pages)
- ❌ No blog features
- ❌ No Markdown support

---

### Option 2: Jekyll-Powered Site
**Best for:** Blogs, multi-page sites, content-focused sites

1. Use both files:
   - `starter-config.yml` → rename to `_config.yml`
   - Create a basic `index.md` or use a theme's default
2. Choose a theme in `_config.yml`
3. Create posts in `_posts/` folder (format: `YYYY-MM-DD-title.md`)
4. Push to GitHub
5. GitHub Pages automatically builds your Jekyll site

**Pros:**
- ✅ Blog-awareness (automatic post listings)
- ✅ Markdown support (easier to write)
- ✅ Templating (reusable layouts, includes)
- ✅ Themes (instant professional design)

**Cons:**
- ❌ Slightly steeper learning curve
- ❌ Longer build times
- ❌ Configuration required

---

## 🎨 Customization Tips

### For `starter-template-index.html`:

#### Change Colors
Look for these lines in the `<style>` section:
```css
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
```
Replace `#667eea` and `#764ba2` with your preferred hex colors.

Try these color palettes:
- 🌊 Ocean: `#2E3192` → `#1BFFFF`
- 🔥 Fire: `#FF512F` → `#DD2476`
- 🌿 Nature: `#56AB2F` → `#A8E063`
- 🌸 Sunset: `#FA709A` → `#FEE140`

#### Add More Sections
Copy this template and insert it before the `<footer>`:
```html
<section>
    <h2>New Section Title</h2>
    <p>Your content here...</p>
</section>
```

#### Add Images
```html
<img src="your-image.jpg" alt="Description" style="max-width: 100%; border-radius: 10px;">
```

---

### For `starter-config.yml`:

#### Change Theme
Uncomment and modify:
```yaml
theme: jekyll-theme-cayman  # Choose from list in file
```

Or use a remote theme:
```yaml
remote_theme: pages-themes/architect@v0.2.0
```

#### Enable Google Analytics
Replace `UA-XXXXXXXXX-X` with your tracking ID:
```yaml
google_analytics: UA-XXXXXXXXX-X
```

#### Add Custom Variables
Use custom variables in your templates:
```yaml
custom_greeting: "Welcome to my site!"
```

Access in templates: `{{ site.custom_greeting }}`

---

## 📖 Next Steps

After setting up your starter template:

1. **Read the main guide** in [GUIDE.md](../GUIDE.md) for detailed instructions
2. **Learn HTML/CSS** if you want to customize beyond basics:
   - [MDN Web Docs](https://developer.mozilla.org/en-US/docs/Learn)
   - [freeCodeCamp](https://www.freecodecamp.org/)
3. **Learn Jekyll** (if using `_config.yml`):
   - [Jekyll Step-by-Step Tutorial](https://jekyllrb.com/docs/step-by-step/01-setup/)
4. **Explore themes**:
   - [GitHub Pages themes](https://pages.github.com/themes/)
   - [Jekyll Themes](https://jekyllrb.com/docs/themes/)

---

## 🆘 Common Issues

### My changes aren't showing up
- ⏰ Wait 5-10 minutes for GitHub Pages to rebuild
- 🔄 Hard refresh your browser: `Ctrl+Shift+R` (Windows) or `Cmd+Shift+R` (Mac)
- 🔍 Check the "Actions" tab in your repository for build errors

### Jekyll build failed
- Check `_config.yml` for syntax errors (YAML is whitespace-sensitive!)
- Ensure you're using 2 spaces for indentation, not tabs
- Validate YAML syntax: [YAML Lint](http://www.yamllint.com/)

### 404 Error
- Repository name must match `yourusername.github.io` exactly
- Check that `index.html` or `index.md` exists in your root folder

---

## 📝 License

These templates are part of the GitHub Pages Guide.

**Copyright (c) 2026 ShamShamsw / Jacob Haseman**

Licensed under the [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).

You're free to use, modify, and distribute these templates with attribution.

---

## 💡 Need More Help?

- Read the [full guide](../GUIDE.md)
- Check [GitHub's official documentation](../GITHUB_DOCS_REFERENCE.md)
- Open an issue if you find errors or have suggestions

Happy building! 🚀
