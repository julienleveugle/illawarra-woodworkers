# Deployment Guide

This guide will walk you through deploying your Jekyll site to GitHub Pages.

## Step 1: Install Jekyll Locally (Optional but Recommended)

Before deploying, you can test the site locally.

### Install Ruby and Bundler

**macOS:**
```bash
# Ruby should be pre-installed on macOS
# Install bundler
gem install bundler
```

**Windows:**
- Download and install Ruby from [RubyInstaller](https://rubyinstaller.org/)
- Install bundler: `gem install bundler`

**Linux (Ubuntu/Debian):**
```bash
sudo apt-get update
sudo apt-get install ruby-full build-essential
gem install bundler
```

### Run Locally

```bash
# Navigate to the project directory
cd /Users/julien/Documents/code/IWG

# Install dependencies
bundle install

# Start the local server
bundle exec jekyll serve

# Open http://localhost:4000 in your browser
```

## Step 2: Create a GitHub Repository

1. Go to [GitHub](https://github.com) and sign in
2. Click the "+" icon in the top right and select "New repository"
3. Name your repository (e.g., `illawarra-woodworkers`)
4. Choose "Public" (required for free GitHub Pages)
5. **Do NOT** initialize with README, .gitignore, or license
6. Click "Create repository"

## Step 3: Push Your Code to GitHub

```bash
# Navigate to your project directory
cd /Users/julien/Documents/code/IWG

# Initialize git (if not already done)
git init

# Add all files
git add .

# Create initial commit
git commit -m "Initial commit - Jekyll site for Illawarra Woodworkers Group"

# Add your GitHub repository as remote
# Replace YOUR-USERNAME and YOUR-REPO-NAME with your actual values
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git

# Rename branch to main
git branch -M main

# Push to GitHub
git push -u origin main
```

## Step 4: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click on "Settings" tab
3. In the left sidebar, click "Pages"
4. Under "Source":
   - Select "Deploy from a branch"
   - Choose branch: `main`
   - Choose folder: `/ (root)`
5. Click "Save"

GitHub will now build and deploy your site!

## Step 5: Access Your Site

After a few minutes, your site will be available at:

```
https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/
```

You'll see a green checkmark and the URL in the Pages settings when it's ready.

## Step 6: Update the Base URL (If Using Subdirectory)

If your site is in a subdirectory (not at the root like `username.github.io`), you need to update `_config.yml`:

```yaml
# Change this line:
baseurl: ""

# To this (use your repository name):
baseurl: "/YOUR-REPO-NAME"
```

Then commit and push:

```bash
git add _config.yml
git commit -m "Update baseurl for GitHub Pages"
git push
```

## Making Updates

Every time you make changes:

```bash
# Make your edits to .md files or CSS
git add .
git commit -m "Description of your changes"
git push
```

GitHub Pages will automatically rebuild and deploy your changes within a few minutes.

## Using a Custom Domain (Optional)

### If you own a domain (e.g., illawarrawoodworkers.org.au):

1. **Add CNAME file:**
   ```bash
   echo "illawarrawoodworkers.org.au" > CNAME
   git add CNAME
   git commit -m "Add custom domain"
   git push
   ```

2. **Configure DNS with your domain provider:**

   Add these DNS records:

   **For apex domain (illawarrawoodworkers.org.au):**
   ```
   A     @     185.199.108.153
   A     @     185.199.109.153
   A     @     185.199.110.153
   A     @     185.199.111.153
   ```

   **For www subdomain:**
   ```
   CNAME www   YOUR-USERNAME.github.io
   ```

3. **Enable HTTPS in GitHub Pages settings**
   - Go to Settings > Pages
   - Check "Enforce HTTPS" (may take up to 24 hours)

## Troubleshooting

### Site not showing up?

1. Check the "Actions" tab in your repository to see if the build succeeded
2. Make sure GitHub Pages is enabled in Settings
3. Wait 5-10 minutes for the first deployment

### Styles not loading?

1. Check that `baseurl` in `_config.yml` matches your repository name
2. Make sure CSS file paths use `{{ '/assets/css/style.css' | relative_url }}`

### Changes not appearing?

1. Hard refresh your browser (Cmd+Shift+R on Mac, Ctrl+Shift+R on Windows)
2. Wait a few minutes for GitHub to rebuild
3. Check the Actions tab for build status

## Need Help?

- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- Email: info@illawarrawoodworkers.org.au
