# The Critical Pixels - Image Management Guide

## Adding Images to Posts

### Quick Start
1. **Add your image** to `assets/images/posts/` (e.g., `my-post-hero.jpg`)
2. **Add to post front matter:**
   ```yaml
   ---
   layout: post
   title: "My Post Title"
   featured_image: my-post-hero.jpg
   ---
   ```
3. **Done!** The image will automatically appear in the hero section, post cards, and post header.

### Folder Structure
```
assets/images/
├── posts/           # All post images go here
│   ├── hollow-echoes-hero.jpg
│   ├── chrono-nexus-hero.jpg
│   ├── ludonarrative-mechanics-hero.jpg
│   └── ... (any filename you want)
├── hero/            # Backup/fallback hero images
└── categories/      # Category icons (optional)
```

### Image Guidelines

#### File Names
- Use descriptive names: `game-title-hero.jpg`, `review-name-main.jpg`
- No spaces: use hyphens: `hollow-echoes-review.jpg`
- Keep it simple and memorable

#### Image Sizes
- **Hero images**: 1920×600px (landscape, will be cropped to fit)
- **Post thumbnails**: 600×400px (landscape)
- **High quality**: Use JPG/WebP for photos, PNG for graphics

#### Supported Formats
- JPG/JPEG (recommended for photos)
- PNG (for transparency)
- WebP (modern format, smaller files)

### Examples

#### Post with Image
```yaml
---
layout: post
title: "Game Review: Amazing Adventure"
date: 2025-12-01
categories: review
score: 9
featured_image: amazing-adventure-hero.jpg
---
```

#### Post without Image (uses gradients)
```yaml
---
layout: post
title: "Essay: Game Design Philosophy"
date: 2025-12-01
categories: essay
# No featured_image = automatic gradients
---
```

### Automatic Features

- **Fallbacks**: Missing images automatically show beautiful gradient placeholders
- **Categories**: Gradients change color based on category (review=blue, essay=pink, philosophy=teal)
- **Responsive**: Images automatically scale for mobile/tablet/desktop
- **Performance**: Images are lazy-loaded and optimized

### Tips

1. **Naming**: Use consistent naming like `{post-slug}-hero.jpg`
2. **Organization**: Keep all post images in one folder for easy management
3. **Quality**: High-resolution images look best (2x for retina displays)
4. **SEO**: Descriptive filenames help with search engines

### Troubleshooting

- **Image not showing?** Check the filename matches exactly in front matter
- **Wrong size?** Images are cropped to fit containers
- **Slow loading?** Optimize images or use WebP format

That's it! Just drop your image in the folder and reference the filename in the post.
