# The Pulse UBC - Website Documentation

A professional, clean economics journalism website for weekly student reporting on economics, inequality, and policy.

## What's Included

- **index.html** - Homepage with featured and recent articles
- **articles.html** - Archive page showing all articles
- **podcast.html** - Podcast page (currently "Coming Soon" placeholder)
- **about.html** - About page with mission statement and writer bios
- **article1.html** - Sample full article page showing ~1000 word format
- **styles.css** - All styling and design
- **README.md** - This file

## Design Features

- **Dark forest green + cream color scheme** - Distinctive, professional, Pacific Northwest aesthetic
- **Sophisticated typography** - Crimson Pro (serif) for headlines and body text, Work Sans (sans-serif) for UI elements
- **Responsive design** - Works beautifully on desktop, tablet, and mobile
- **Publication-quality layout** - Inspired by The Economist and Financial Times
- **Smooth animations** - Elegant page load and hover effects
- **Easy to customize** - Well-organized code with CSS variables

## How to Add New Articles

### Quick Method (Direct HTML)

1. **Duplicate** `article1.html` and rename it (e.g., `article2.html`)
2. **Edit the content:**
   - Replace the title in `<title>` and `<h1>`
   - Update the category, excerpt, byline, and date
   - Replace the article body text
   - Update the hero image placeholder color if desired
3. **Add to homepage and articles page:**
   - Copy one of the article cards in `index.html` or `articles.html`
   - Update the title, excerpt, author, date, and link to your new article file

### Customizing Colors

All colors are defined at the top of `styles.css` using CSS variables. To change the color scheme:

```css
:root {
    --forest-green: #1a4d2e;        /* Main brand color */
    --forest-green-dark: #0f2e1b;   /* Darker variant */
    --forest-green-light: #2d5f3f;  /* Lighter variant */
    --cream: #faf8f3;               /* Background color */
    /* etc. */
}
```

Change these values to instantly update the entire site's color scheme.

### Replacing Placeholder Images

The current design uses CSS gradient placeholders. To add real images:

1. **For article hero images**, replace this:
```html
<div class="image-placeholder" style="background: linear-gradient(135deg, #1a4d2e 0%, #2d5f3f 100%);">
    <span class="placeholder-text">Article Image</span>
</div>
```

With this:
```html
<img src="your-image.jpg" alt="Article description" style="width: 100%; height: auto; display: block;">
```

2. Save your images in the same folder as your HTML files
3. Use descriptive filenames (e.g., `housing-crisis-hero.jpg`)

## How to Deploy (Get Your Site Online)

### Option 1: GitHub Pages (Free, Recommended)

1. **Create a GitHub account** if you don't have one (github.com)
2. **Create a new repository** named `the-pulse-ubc` (or any name you want)
3. **Upload all files** to the repository:
   - index.html
   - articles.html
   - podcast.html
   - about.html
   - article1.html
   - styles.css
4. **Enable GitHub Pages:**
   - Go to repository Settings
   - Scroll to "Pages" section
   - Under "Source", select "main" branch
   - Click Save
5. **Your site will be live at:** `https://yourusername.github.io/the-pulse-ubc/`

### Option 2: Netlify (Free, Super Easy)

1. **Go to netlify.com** and sign up
2. **Drag and drop** your entire website folder into Netlify
3. **Your site is live!** Netlify gives you a URL like `yoursite.netlify.app`
4. You can customize the subdomain name in settings

### Adding a Custom Domain

Once your site is deployed, you can add a custom domain:

1. **Buy a domain** ($10-15/year) from:
   - Namecheap
   - Google Domains
   - GoDaddy
2. **Connect it to GitHub Pages or Netlify:**
   - Both platforms have simple guides in their docs
   - Usually involves updating DNS settings (they'll walk you through it)

## Customizing Writer Bios

Edit `about.html` to add or modify writer information:

```html
<div class="writer-card">
    <h3 class="writer-name">Your Name</h3>
    <p class="writer-bio">
        Your bio here...
    </p>
</div>
```

## Site Structure

```
the-pulse-ubc/
├── index.html          # Homepage
├── articles.html       # Articles archive
├── podcast.html        # Podcast page
├── about.html          # About/Writers page
├── article1.html       # Sample article (template for new articles)
├── styles.css          # All styling
└── README.md          # This file
```

## Tips for Long-Form Articles

The `article1.html` template is optimized for ~1000 word articles:

- First paragraph has a **drop cap** (large first letter)
- Use `<h2>` for section headers
- Use `<blockquote>` for pull quotes
- Typography is designed for comfortable long-form reading
- Serif font (Crimson Pro) is highly readable at 1.2rem size

## Browser Compatibility

Works in all modern browsers:
- Chrome, Firefox, Safari, Edge
- Mobile browsers (iOS Safari, Chrome Mobile)

## Need Help?

Common questions:

**Q: How do I change fonts?**
A: Edit the Google Fonts link in the `<head>` of each HTML file, then update the font variables in `styles.css`

**Q: Can I add comments to articles?**
A: You'd need to integrate a third-party service like Disqus. For now, the site is static HTML.

**Q: How do I make the site searchable?**
A: Once you have more articles, you could add a simple JavaScript search or use a service like Algolia.

**Q: Can I track visitors?**
A: Yes, add Google Analytics by inserting their tracking code in the `<head>` of each page.

## License

Feel free to modify and use this design for your publication!

---

Built with care for The Pulse UBC
Weekly student journalism on economics, inequality, and policy
