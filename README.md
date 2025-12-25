# WFBTrakker Website

Marketing website for WFBTrakker products: LinkTray and MonitorTray.

## Pages

- **index.html** - Homepage showcasing both products
- **linktray.html** - Dedicated LinkTray product page
- **monitortray.html** - Dedicated MonitorTray product page

## Technology Stack

- Plain HTML5
- Tailwind CSS (via CDN)
- Vanilla JavaScript
- No build process required

## Running Locally

Simply open any HTML file in a web browser:

```bash
# On Windows
start index.html

# Or just double-click index.html in File Explorer
```

For a local development server (optional):

```bash
# Using Python
python -m http.server 8000

# Using Node.js (if http-server is installed)
npx http-server

# Then visit http://localhost:8000
```

## Features

- Responsive design (mobile, tablet, desktop)
- Mobile navigation menu
- Smooth scrolling
- Tailwind CSS for styling
- SEO-friendly meta tags
- Accessibility considerations

## Deployment

This is a static website and can be deployed to:

- GitHub Pages
- Netlify
- Vercel
- AWS S3
- Azure Static Web Apps
- Any static hosting service

Simply upload the HTML files to your hosting provider.

### GitHub Pages Deployment

1. Create a repository and push these files
2. Go to Settings > Pages
3. Select the main branch as source
4. Your site will be available at `https://username.github.io/repository-name/`

### Netlify Deployment

1. Drag and drop the folder to Netlify
2. Or connect your Git repository
3. Site will be live immediately

## Customization

### Update Download Links

Currently, download links point to `#`. Update these in all three HTML files:

```html
<!-- Search for href="#" in download buttons and update to actual download URLs -->
<a href="path/to/linktray-installer.exe">Download LinkTray</a>
<a href="path/to/monitortray-installer.exe">Download MonitorTray</a>
```

### Change Colors

Colors are configured in the Tailwind config within each HTML file:

```javascript
tailwind.config = {
    theme: {
        extend: {
            colors: {
                primary: '#2563eb',    // Blue - used for LinkTray
                secondary: '#7c3aed',  // Purple - used for MonitorTray
            }
        }
    }
}
```

### Update Content

All content is based on the marketing documents in the `documents/` folder. Update the HTML files to reflect any product changes.

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers

## Performance

- Tailwind CSS loaded via CDN (can be optimized by building locally)
- No external dependencies beyond Tailwind
- Minimal JavaScript
- Fast page loads

## Future Enhancements

Potential improvements to consider:

- Add actual download links when installers are ready
- Implement contact form
- Add FAQ section
- Include screenshots/demo videos of the applications
- Add blog/documentation section
- Implement analytics (Google Analytics, Plausible, etc.)
- Optimize Tailwind CSS by building locally (reduce file size)
- Add social media links and sharing buttons
- Create separate About/Contact pages if needed
