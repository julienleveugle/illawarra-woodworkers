# Illawarra Woodworkers Group Website

This is the official website for the Illawarra Woodworkers Group, a non-profit volunteer organization located in the Illawarra region of New South Wales, Australia.

## About

The Illawarra Woodworkers Group promotes fine craftsmanship and maintains traditional woodworking skills. This website is built with Jekyll and hosted on GitHub Pages.

## Local Development

### Prerequisites

- Ruby (version 2.7 or higher)
- Bundler

### Setup

1. Clone this repository
2. Install dependencies:
   ```bash
   bundle install
   ```

3. Run the local server:
   ```bash
   bundle exec jekyll serve
   ```

4. Open your browser to `http://localhost:4000`

### Building the Site

To build the site for production:

```bash
bundle exec jekyll build
```

The built site will be in the `_site` directory.

## Deployment to GitHub Pages

This site is configured to deploy automatically to GitHub Pages.

### Setup Instructions

1. Create a new repository on GitHub (e.g., `illawarra-woodworkers-website`)

2. Initialize git and push this code:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git
   git push -u origin main
   ```

3. Enable GitHub Pages:
   - Go to your repository settings
   - Navigate to "Pages" in the left sidebar
   - Under "Source", select "Deploy from a branch"
   - Select the "main" branch and "/ (root)" folder
   - Click "Save"

4. Your site will be available at:
   `https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/`

### Custom Domain (Optional)

To use a custom domain:

1. Add a `CNAME` file to the root of your repository with your domain name
2. Configure your DNS provider to point to GitHub Pages
3. In repository settings > Pages, add your custom domain

## Structure

```
.
├── _config.yml           # Site configuration
├── _layouts/             # HTML layouts
│   ├── default.html
│   └── page.html
├── _includes/            # Reusable components
│   ├── header.html
│   └── footer.html
├── assets/
│   └── css/
│       └── style.css     # Main stylesheet (mobile-responsive)
├── *.md                  # Page content files
└── Gemfile              # Ruby dependencies
```

## Pages

- **Home** (`index.md`) - Welcome page with latest news
- **About Us** (`about-us.md`) - Group history and information
- **Location** (`location.md`) - Workshop location and contact details
- **Woodwork for Sale** (`woodwork-for-sale.md`) - Items available for purchase
- **Newsletters** (`newsletters.md`) - Archive of past newsletters
- **Web Links** (`web-links.md`) - Useful woodworking resources
- **Donations** (`donations.md`) - Information about charitable donations

## Features

- ✅ Mobile-responsive design
- ✅ Clean, accessible layout
- ✅ Easy content management with Markdown
- ✅ Automatic deployment with GitHub Pages
- ✅ SEO-friendly structure
- ✅ Fast loading times

## Making Changes

### Adding a New Page

1. Create a new `.md` file in the root directory
2. Add front matter at the top:
   ```yaml
   ---
   layout: page
   title: Your Page Title
   permalink: /your-page-url
   ---
   ```
3. Write your content in Markdown
4. Add the page to navigation in `_config.yml`

### Updating Content

Simply edit the relevant `.md` file and commit your changes. GitHub Pages will automatically rebuild the site.

### Customizing Styles

Edit `assets/css/style.css` to modify the appearance. The CSS uses CSS variables for easy color customization.

## Contact

- **Email:** info@illawarrawoodworkers.org.au
- **Postal:** PO Box 121, CORRIMAL NSW 2518

## License

© 2025 Illawarra Woodworkers Group. All rights reserved.
