# Visual Updates Summary

## 🎨 What's Been Added

Your Jekyll website now includes beautiful visual elements to make it more engaging and professional!

## ✨ New Features

### 1. Logo in Header
- **Your IWG Logo** now appears in the header of every page
- Automatically scales for mobile devices
- Links back to homepage when clicked
- Professional branding throughout the site

### 2. Hero Section on Homepage
- **Stunning hero image** with wood shavings and tools from Unsplash
- Blue gradient overlay matching your brand colors
- Large welcome title: "Welcome to Illawarra Woodworkers Group"
- Subtitle: "Promoting fine craftsmanship and traditional woodworking skills since 1988"
- Fully responsive on all devices

### 3. Image Header on About Us Page
- **Workshop photo** showing woodworking tools
- Similar blue overlay for consistency
- Makes the page more visually interesting
- Professional presentation

### 4. Mobile-Optimized Images
- All images scale perfectly on phones and tablets
- Reduced height on smaller screens for better UX
- Fast loading with lazy loading enabled
- Touch-friendly design

## 🎯 Visual Design Features

### Color Overlay
- Semi-transparent blue gradient over images
- Matches your primary brand color (#0088cc)
- Ensures text is always readable
- Professional, cohesive look

### Typography on Images
- White text with shadow for contrast
- Easy to read on all backgrounds
- Scalable font sizes for different devices
- Professional hierarchy

### Responsive Breakpoints
- **Desktop (>768px):** Full-size hero (400px height)
- **Tablet (≤768px):** Medium hero (300px height)
- **Mobile (≤480px):** Compact hero (250px height)
- Logo scales from 60px to 45px on mobile

## 📱 How It Looks

### Homepage
```
┌─────────────────────────────────────┐
│  [LOGO]              [NAVIGATION]   │
├─────────────────────────────────────┤
│                                     │
│    Beautiful Workshop Image         │
│    with Blue Overlay                │
│                                     │
│    Welcome to Illawarra             │
│    Woodworkers Group                │
│    Promoting fine craftsmanship...  │
│                                     │
├─────────────────────────────────────┤
│  Introduction content...            │
│  Latest News...                     │
│  Bendigo Support...                 │
└─────────────────────────────────────┘
```

### Other Pages (e.g., About Us)
```
┌─────────────────────────────────────┐
│  [LOGO]              [NAVIGATION]   │
├─────────────────────────────────────┤
│                                     │
│    Workshop Tools Image             │
│    with Blue Overlay                │
│    About Us                         │
│                                     │
├─────────────────────────────────────┤
│  Page content...                    │
└─────────────────────────────────────┘
```

## 🔧 Easy Customization

### Want to add an image to another page?

Just edit the page's front matter:

```yaml
---
layout: page-with-image
title: Your Page Name
header_image: "https://images.unsplash.com/photo-ID?w=1200&q=80"
---
```

### Want to change the overlay color?

Edit `assets/css/style.css` and change:

```css
.hero-overlay {
    background: linear-gradient(135deg, rgba(0, 136, 204, 0.85), rgba(0, 136, 204, 0.65));
}
```

Change the `0, 136, 204` values to your desired RGB color.

### Want to use different images?

1. Browse [Unsplash](https://unsplash.com)
2. Search for "woodworking" or "carpentry"
3. Copy the image URL
4. Format as: `https://images.unsplash.com/photo-ID?w=1200&q=80`
5. Use in your page front matter

## 📸 Current Images

1. **Homepage Hero**
   - Wood shavings and scissors on a table
   - Creates welcoming, artisanal feel
   - Full-width banner

2. **About Us Header**
   - Workshop with tools on the floor
   - Shows authentic working environment
   - Connects with woodworking theme

## 🚀 Next Steps

To see your updated site with images:

```bash
cd /Users/julien/Documents/code/IWG
bundle exec jekyll serve
```

Then open http://localhost:4000 in your browser!

## 💡 Tips

- Images load from Unsplash CDN (fast and free)
- You can download and host locally if preferred (see IMAGES.md)
- Add more images to other pages using the same pattern
- Consider adding a gallery page for member projects
- Product photos can go on the "Woodwork for Sale" page

---

**Your site now has:**
- ✅ Professional logo placement
- ✅ Stunning hero images
- ✅ Mobile-responsive design
- ✅ Brand-consistent colors
- ✅ Fast loading times
- ✅ Modern, engaging appearance

**Ready to deploy!** 🎉
