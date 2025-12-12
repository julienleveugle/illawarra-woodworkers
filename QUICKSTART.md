# Quick Start Guide

## What You Have

A complete Jekyll website ready to deploy to GitHub Pages with:
- ✅ All content from the original site converted to Markdown
- ✅ Mobile-responsive design
- ✅ Clean, modern layout
- ✅ Easy to maintain and update

## Fastest Way to Get Online

### Option 1: Deploy to GitHub Pages (5 minutes)

1. **Create a GitHub account** (if you don't have one): https://github.com/join

2. **Create a new repository:**
   - Go to https://github.com/new
   - Name: `illawarra-woodworkers`
   - Public repository
   - Click "Create repository"

3. **Upload your files:**
   ```bash
   cd /Users/julien/Documents/code/IWG
   git init
   git add .
   git commit -m "Initial commit"
   git remote add origin https://github.com/YOUR-USERNAME/illawarra-woodworkers.git
   git branch -M main
   git push -u origin main
   ```

4. **Enable GitHub Pages:**
   - Go to repository Settings > Pages
   - Source: Deploy from branch "main" / (root)
   - Save

5. **Done!** Your site will be at:
   `https://YOUR-USERNAME.github.io/illawarra-woodworkers/`

### Option 2: Test Locally First

```bash
# Install dependencies
cd /Users/julien/Documents/code/IWG
bundle install

# Run local server
bundle exec jekyll serve

# Open http://localhost:4000
```

## File Structure Overview

```
IWG/
├── _config.yml          ← Site settings (edit site title, contact info, etc.)
├── _layouts/            ← HTML templates (rarely need to edit)
├── _includes/           ← Header and footer (rarely need to edit)
├── assets/css/          ← Styles (edit to change colors/fonts)
├── index.md             ← Home page content
├── about-us.md          ← About page content
├── location.md          ← Location page content
├── woodwork-for-sale.md ← Products page content
├── newsletters.md       ← Newsletter archive
├── web-links.md         ← Web links page
├── donations.md         ← Donations page
└── Gemfile             ← Dependencies
```

## Common Tasks

### Update Text Content

1. Open the relevant `.md` file
2. Edit the text (it's just plain text/Markdown)
3. Save
4. Commit and push:
   ```bash
   git add .
   git commit -m "Updated content"
   git push
   ```

### Change Colors

Edit `assets/css/style.css` at the top:

```css
:root {
    --primary-color: #0088cc;  /* Change this for main color */
    --text-color: #333;         /* Text color */
    --bg-color: #f4f6f7;       /* Background color */
}
```

### Add a New Page

1. Create `new-page.md`:
   ```markdown
   ---
   layout: page
   title: New Page
   permalink: /new-page
   ---

   Your content here...
   ```

2. Add to navigation in `_config.yml`:
   ```yaml
   navigation:
     - title: New Page
       url: /new-page
   ```

### Update Newsletter Links

Just edit `newsletters.md` and add new entries following the existing format.

## Important Files to Update

Before going live, update these:

1. **_config.yml** - Update contact email if needed
2. **README.md** - Replace YOUR-USERNAME with actual GitHub username
3. **If using custom domain** - Add CNAME file

## Getting Help

- See `DEPLOYMENT.md` for detailed deployment instructions
- See `README.md` for full documentation
- Jekyll docs: https://jekyllrb.com/docs/

## Next Steps After Deployment

1. Download images from old site to `assets/images/`
2. Update image paths in markdown files
3. Test all links
4. Add Google Analytics (optional)
5. Set up custom domain (optional)

---

**Questions?** Email: info@illawarrawoodworkers.org.au
