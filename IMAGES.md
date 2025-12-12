# Images Used in the Website

## Logo

**File:** `assets/images/IWG_logo.png`
- **Location:** Header (all pages)
- **Size:** Auto-scaled to 60px height (45px on mobile)
- **Source:** Your original IWG_logo.png file
- **File Size:** 2.8 MB

## Stock Images (Locally Hosted)

All beautiful woodworking images from Unsplash, now hosted locally for faster loading and offline development.

### 1. Homepage Hero Image
**File:** `assets/images/wood-shavings.jpg`
- **Original:** cristian-tarzi-XFcPxg6plfQ-unsplash.jpg
- **Description:** Wood shavings and scissors on a table
- **Credit:** Photo by Cristian Tarzi on [Unsplash](https://unsplash.com/photos/a-pair-of-scissors-and-some-wood-shavings-on-a-table-XFcPxg6plfQ)
- **Usage:** Large hero banner on homepage
- **Dimensions:** Responsive - 400px height (desktop) → 250px (mobile)
- **File Size:** 2.5 MB

### 2. About Us Page Header
**File:** `assets/images/workshop-tools.jpg`
- **Original:** cristian-tarzi-KV2KjOCSBB4-unsplash.jpg
- **Description:** Woodworking workshop with tools on the floor
- **Credit:** Photo by Cristian Tarzi on [Unsplash](https://unsplash.com/photos/a-room-that-has-a-bunch-of-tools-on-the-floor-KV2KjOCSBB4)
- **Usage:** Page header banner on About Us page
- **Dimensions:** Responsive - 300px height (desktop) → 150px (mobile)
- **File Size:** 3.3 MB

### 3. Woodwork for Sale Page Header
**File:** `assets/images/woodworking-bench.jpg`
- **Original:** dmitriy-demidov--gyOtQS4Yp4-unsplash.jpg
- **Description:** Beautiful woodworking workbench
- **Credit:** Photo by Dmitriy Demidov on Unsplash
- **Usage:** Page header banner on Woodwork for Sale page
- **Dimensions:** Responsive - 300px height (desktop) → 150px (mobile)
- **File Size:** 3.2 MB

### 4. Donations Page Header
**File:** `assets/images/wood-planks.jpg`
- **Original:** job-vermeulen-gJWlckmTeYc-unsplash.jpg
- **Description:** Natural wood planks and materials
- **Credit:** Photo by Job Vermeulen on Unsplash
- **Usage:** Page header banner on Donations page
- **Dimensions:** Responsive - 300px height (desktop) → 150px (mobile)
- **File Size:** 2.8 MB

## Image Distribution

```
Homepage:           wood-shavings.jpg (Hero section)
About Us:           workshop-tools.jpg (Header)
Woodwork for Sale:  woodworking-bench.jpg (Header)
Donations:          wood-planks.jpg (Header)
All Pages:          IWG_logo.png (Header logo)
```

## Image Styling

All images include:
- ✅ Local hosting (no external dependencies)
- ✅ Lazy loading for better performance
- ✅ Responsive sizing (scales on mobile)
- ✅ Blue overlay with transparency for brand consistency
- ✅ Text shadow on overlaid text for readability
- ✅ Smooth transitions and modern appearance

## Technical Details

### Image Formats
- **Format:** JPEG (optimized for photographs)
- **Color Space:** RGB
- **Quality:** High quality originals from Unsplash

### Loading Strategy
- **Lazy Loading:** Enabled on all images except logo
- **Above the fold:** Logo loads immediately
- **Below the fold:** Hero and header images lazy load

### Responsive Behavior
```css
Desktop (>768px):  Hero 400px, Headers 300px, Logo 60px
Tablet (≤768px):   Hero 300px, Headers 200px, Logo 50px
Mobile (≤480px):   Hero 250px, Headers 150px, Logo 45px
```

## File Structure

```
assets/images/
├── IWG_logo.png                    (2.8 MB)
├── wood-shavings.jpg              (2.5 MB) - Homepage hero
├── workshop-tools.jpg             (3.3 MB) - About Us
├── woodworking-bench.jpg          (3.2 MB) - Woodwork for Sale
└── wood-planks.jpg                (2.8 MB) - Donations
```

**Total Image Assets:** ~14.6 MB

## Adding More Images

### To add a header image to any page:

1. Place your image in `assets/images/`
2. Update the page's front matter:
   ```yaml
   ---
   layout: page-with-image
   title: Your Page Title
   header_image: "/assets/images/your-image.jpg"
   ---
   ```

### To replace an existing image:

1. Replace the file in `assets/images/`
2. Keep the same filename, or
3. Update the reference in the page/layout

## Optimization Tips

If you want to optimize images for web (reduce file size):

### Using ImageMagick (command line):
```bash
# Resize and optimize
convert input.jpg -resize 1200x -quality 85 output.jpg
```

### Using Online Tools:
- [TinyJPG](https://tinyjpg.com/) - Compress JPEG images
- [Squoosh](https://squoosh.app/) - Google's image optimizer
- [ImageOptim](https://imageoptim.com/) - Mac app

### Recommended Settings:
- **Max Width:** 1200-1600px (more than enough for hero images)
- **Quality:** 80-85% (good balance)
- **Format:** JPEG for photos, PNG for logos/graphics

## Attribution

All stock images are from [Unsplash](https://unsplash.com) and used under the [Unsplash License](https://unsplash.com/license):

- **Wood shavings:** Cristian Tarzi
- **Workshop tools:** Cristian Tarzi
- **Woodworking bench:** Dmitriy Demidov
- **Wood planks:** Job Vermeulen

Consider adding photo credits in the footer or a dedicated credits page.

## Future Enhancements

Consider adding:
- Member project gallery with thumbnails
- Product photos for "Woodwork for Sale" items
- Photo gallery from workshops and events
- Historical photos from the early years
- Committee member photos

---

**Note:** All images are now hosted locally in your repository. No external dependencies required!
