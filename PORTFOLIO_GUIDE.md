# Portfolio Website Guide

## Overview
Your portfolio website is now set up with a professional structure that matches modern portfolio sites like the reference you provided. The site features beautiful card layouts with hover effects and individual detailed project pages.

## File Structure
```
├── index.html          # Home page with project grid
├── projects.html       # All projects listing
├── project1.html       # Synthetic Data Generator (completed)
├── project2.html       # AI Systems Project (template)
├── project3.html       # Data Science Project (template)
├── style.css           # All styling (responsive design)
├── images/             # Project images folder
│   ├── project1.png
│   ├── project2.png
│   └── project3.png
└── README.md           # This file
```

## How to Use

### 1. Adding Project Images
- Place your project images in the `images/` folder
- Name them: `project1.png`, `project2.png`, `project3.png`, etc.
- Recommended size: 400x400px or larger square images
- Supported formats: PNG, JPG, WebP

### 2. Creating New Project Pages

To add a new project, follow this template structure:

**HTML Structure (create `projectX.html`):**
```html
<div class="project-header">
  <div class="category">Your Category</div>
  <h1>Project Title</h1>
</div>

<img src="images/projectX.png" alt="Description" class="project-image">

<div class="project-section">
  <h2>Section Title</h2>
  <p>Your content here</p>
</div>

<div class="project-tech">
  <strong>Technologies & Tools:</strong>
  <div class="tech-tags">
    <span class="tech-tag">Tech1</span>
    <span class="tech-tag">Tech2</span>
  </div>
</div>
```

### 3. Updating Project Grid on Home Page

Add new cards to `index.html`:
```html
<div class="card" data-category="your-category" onclick="location.href='projectX.html'">
  <img src="images/projectX.png" alt="Description">
  <div class="overlay">
    <h4>Project Title</h4>
    <p>Short description</p>
  </div>
</div>
```

### 4. Adding Projects to Projects List

Update `projects.html` with new project entries in the same format shown there.

## Customization

### Colors
- Primary Red: `#ef4444` (accent color for lines/underlines)
- Yellow Bar: `#facc15` (filter/category bar)
- Dark Text: `#111` (main text)
- Gray Text: `#666` (secondary text)

To change colors, edit `style.css` and update these hex values.

### Fonts
Currently using: `'Segoe UI', Tahoma, Geneva, Verdana, sans-serif`

To change the font family, update the `font-family` property in the `body` selector in `style.css`.

### Layout
- Grid adjusts from 3 columns on desktop to 1-2 columns on mobile
- Container width is 85% with max-width of 1200px
- All spacing, sizes, and padding can be modified in `style.css`

## Features Included

✅ **Responsive Design** - Works on desktop, tablet, and mobile
✅ **Smooth Hover Effects** - Cards zoom on hover with overlay text
✅ **Category Filtering** - Filter projects by category (currently Data Science, AI Systems)
✅ **Detailed Project Pages** - Each project has its own detailed page
✅ **Professional Styling** - Modern typography and spacing
✅ **Tech Tags** - Highlight technologies used in projects
✅ **Navigation** - Easy navigation between pages

## Adding Categories

To add new categories to the filter bar:

1. Edit the filter buttons in `index.html`:
```html
<button onclick="filterProjects('new-category')">NEW CATEGORY</button>
```

2. Add `data-category="new-category"` to project cards in the grid

3. Update the JavaScript filter function if needed (it's already dynamic)

## SEO & Meta Tags

Each page includes:
- Proper `<title>` tags
- Meta charset: UTF-8
- Viewport for mobile responsiveness

To improve SEO further, consider adding:
```html
<meta name="description" content="Your portfolio description">
<meta name="keywords" content="data science, AI, machine learning">
<meta name="author" content="Your Name">
```

## Deployment

This is a static website ready to deploy on:
- GitHub Pages (free)
- Netlify (free)
- Vercel (free)
- Any web hosting service

Simply push your files to the repository or upload to your hosting provider.

## Next Steps

1. **Add Project Images**: Replace placeholder images with your actual project screenshots
2. **Write Project Content**: Update project2.html and project3.html with real project details
3. **Add More Projects**: Copy the project template to create additional project pages
4. **Customize Colors/Fonts**: Adjust `style.css` to match your personal brand
5. **Deploy**: Push to GitHub Pages or your hosting provider

---

Need help? Feel free to modify any section to better match your brand and add more projects!
