# Manifesto for a Free Internet

A clean, modern website for the Iranian Women's Coalition for Internet Freedom manifesto.

## Quick Start

### Local Development

1. Clone this repository
2. Add your logo image as `assets/images/logo.png`
3. Replace the manifesto placeholder content in `index.html`
4. Open `index.html` in your browser or use a local server:

```bash
# Using Python 3
python -m http.server 8000

# Using Node.js (if you have live-server installed)
npx live-server

# Using PHP
php -S localhost:8000
```

Visit `http://localhost:8000` to view your site locally.

### GitHub Pages Deployment

1. Create a new GitHub repository (make it public)
2. Upload your files:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git
   git push -u origin main
   ```
3. Go to repository Settings > Pages
4. Under "Source", select "Deploy from a branch"
5. Choose "main" branch and "/ (root)" folder
6. Click Save

Your site will be available at: `https://[your-username].github.io/[repository-name]/`

### Custom Domain Setup

1. **Buy a domain** from Namecheap, Google Domains, or Cloudflare
2. **Configure DNS** in your registrar:
   - CNAME record: `www` → `your-username.github.io`
   - A records: `@` → GitHub Pages IPs (185.199.108-111.153)
3. **Add domain in GitHub**: Settings > Pages > Custom domain
4. **Enable HTTPS** (recommended)

**Suggested domains**: `iranianwomencoalition.org`, `manifestoforfreeinternet.org`

## Customization

### Adding Your Logo
1. Save your logo as `assets/images/logo.png`
2. The logo should be a high-resolution PNG file (300x300px or larger)

### Adding Your Manifesto Content
1. Open `index.html`
2. Find the section with `<div class="manifesto-content">`
3. Replace the placeholder content with your actual manifesto text
4. You can use HTML formatting for headings, paragraphs, lists, etc.

### Customizing Colors and Styling
- Edit `styles.css` to change colors, fonts, and layout
- The CSS uses CSS custom properties (variables) for easy color customization
- Main colors are defined in the `:root` section at the top of the CSS file

## File Structure

```
manifesto-website/
├── index.html              # Main website file
├── styles.css              # Styling and layout
├── assets/
│   └── images/
│       ├── logo.png         # Your logo (you need to add this)
│       └── README.md        # Instructions for logo
├── .github/
│   └── workflows/
│       └── deploy.yml       # GitHub Pages deployment
└── README.md               # This file
```

## Features

- ✅ Clean, modern design
- ✅ Fully responsive (mobile-friendly)
- ✅ Instagram social media integration
- ✅ Smooth scrolling navigation
- ✅ GitHub Pages ready
- ✅ Accessibility features
- ✅ Fast loading
- ✅ SEO optimized

## Social Media

The website includes integration with Instagram (@zannetazadi). The link is configured in both the navigation and footer.

## Browser Support

This website supports all modern browsers including:
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers

## License

This project is created for the Iranian Women's Coalition for Internet Freedom.