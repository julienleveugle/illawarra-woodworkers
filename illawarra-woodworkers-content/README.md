# Illawarra Woodworkers Group - Website Content

This directory contains the extracted content from the Illawarra Woodworkers Group website (https://illawarrawoodworkers.org.au/) for rebuilding as a static website.

## Directory Structure

```
illawarra-woodworkers-content/
├── README.md                    # This file
├── site-structure.json          # Overall site structure, navigation, and metadata
├── pages/                       # Markdown files for each page
│   ├── home.md
│   ├── about-us.md
│   ├── location.md
│   ├── woodwork-for-sale.md
│   ├── newsletters.md
│   ├── web-links.md
│   └── donations.md
└── assets/                      # Placeholder for images and other assets
```

## Content Overview

### Pages

1. **Home** (`home.md`)
   - Introduction to the Illawarra Woodworkers Group
   - Latest news and events
   - Bendigo Bank support information

2. **About Us** (`about-us.md`)
   - Group history and mission
   - Committee members (2023)
   - Meeting and workshop information
   - Brief history since 1988

3. **Location** (`location.md`)
   - Physical address and directions
   - GPS coordinates
   - Contact information (email and postal address)

4. **Woodwork for Sale** (`woodwork-for-sale.md`)
   - Children's table & chairs
   - Toy garage
   - Butcher's block chopping boards
   - Cutting boards

5. **Newsletters** (`newsletters.md`)
   - Archive of newsletters from 2005-2024
   - Links to PDF files

6. **Web Links** (`web-links.md`)
   - Categorized links for woodworkers
   - 12 categories of resources

7. **Donations** (`donations.md`)
   - History of charitable toy donations
   - Photos of past donations

## Key Information

### Contact Details
- **Email:** info@illawarrawoodworkers.org.au
- **Postal Address:** PO Box 121, CORRIMAL NSW 2518

### Location
- **Address:** Fairy Meadow Primary School, Balgownie Road, Fairy Meadow, NSW
- **Coordinates:** -34.390136, 150.892323

### Workshop Times
- **Days:** Thursday and Saturday
- **Time:** 8:00 AM to Midday
- **Closed:** Late December to end of January

### Monthly Meetings
- **When:** 9:00 AM on the second Saturday of each month
- **Exception:** No meeting in January

### Membership
- **Annual Fee:** $50 per person
- **Visitor Policy:** Welcome for up to 3 meetings before joining

## Assets to Download

The following assets are referenced in the content and should be downloaded from the original site:

### Images
- `/images/banners/IWG Web Logo 706x170 R3 Final.png` - Main logo
- `/images/stories/bendigo_logo.jpg` - Bendigo Bank logo
- `/images/earlyworkshop/*.jpg` - Early workshop photos (8 images)
- `/images/stories/products/*.png` - Product images for sale
- `/images/stories/donations/*.jpg` - Donation photos

### PDFs
- Newsletter PDFs from 2005-2024 (located in `/images/stories/documents/news/` and `/images/stories/documents/members/newsletter/`)

## Next Steps for Rebuilding

1. **Download Assets:** Retrieve all images and PDF files from the original site
2. **Choose Static Site Generator:** Consider Jekyll, Hugo, or Next.js
3. **Design Theme:** Create a clean, accessible design
4. **Implement Navigation:** Use the navigation structure from `site-structure.json`
5. **Host on GitHub Pages:** Deploy the static site

## Original Site Information

- **Original URL:** https://illawarrawoodworkers.org.au/
- **CMS:** Joomla
- **Template:** Protostar
- **Copyright:** © 2025 Illawarra Woodworkers Group

## Notes

- The Events Calendar page was not fully extracted as it appears to be dynamic
- Web Links categories are listed but individual links within each category would need to be extracted from sub-pages
- All content is in Markdown format for easy conversion to HTML
- Image paths reference the original site structure and will need to be updated once assets are downloaded
