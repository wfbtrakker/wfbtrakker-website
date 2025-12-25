# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is the **WfbtrakkerWebsite** repository, containing the marketing website for WFBTrakker applications. The site markets two Windows productivity applications:

- **LinkTray**: A Windows system tray application for organizing and managing links/bookmarks
- **MonitorTray**: A Windows system tray application for managing multi-monitor setups

## Current Structure

```
WfbtrakkerWebsite/
├── index.html                      # Homepage showcasing both products
├── linktray.html                   # LinkTray product page
├── monitortray.html                # MonitorTray product page
├── README.md                       # Website documentation
├── CLAUDE.md                       # This file
└── documents/
    ├── LinkTray-Marketing.md       # Source content for LinkTray
    └── MonitorTray-Marketing.md    # Source content for MonitorTray
```

## Technology Stack

- **HTML5**: Plain HTML, no framework
- **CSS**: Tailwind CSS (loaded via CDN)
- **JavaScript**: Vanilla JavaScript for mobile menu and smooth scrolling
- **No Build Process**: Static site, can be opened directly in browser or deployed to any static host

## Related Projects

This repository is part of a larger solution that includes:
- **LinkTrayInterface**: The actual LinkTray application (.NET/Windows Forms)
- **RemoteMonitorManager**: The actual MonitorTray application (.NET/Windows Forms)
- **KLDTimeSheet**: A time tracking application

All projects are located in the parent directory: `C:\Users\scott\source\repos\wfbtrakker\`

## Product Information

### LinkTray
- **Purpose**: System tray link/bookmark manager for Windows
- **Key Features**: Browser URL capture (CTRL+L hotkey), hierarchical folder organization, favorites system, link groups, click tracking
- **Tech Stack**: .NET 8, Windows Forms
- **Target Platform**: Windows 8/10/11

### MonitorTray
- **Purpose**: Multi-monitor control and management from system tray
- **Key Features**: Power control, brightness adjustment, scheduled automation, custom monitor naming, DDC/CI protocol support
- **Tech Stack**: .NET 8.0, Windows Forms
- **Target Platform**: Windows 10 or later

## Running the Website Locally

To view the website:

```bash
# Open directly in browser
start index.html

# Or use a local server (optional)
python -m http.server 8000
# Then visit http://localhost:8000
```

## Development Notes

### Content Source
- Marketing documentation in `documents/` is the source of truth for product features and messaging
- All website content is based on these marketing documents
- Target audience: home office professionals, developers, gamers, designers, traders, students, IT administrators

### Current Implementation
- Three-page responsive website (home, LinkTray page, MonitorTray page)
- Mobile-friendly with responsive navigation
- Smooth scrolling and accessibility features
- Download links currently point to `#` placeholders - update these when installers are ready

### Color Scheme
- **Primary (Blue)**: `#2563eb` - Used for LinkTray branding
- **Secondary (Purple)**: `#7c3aed` - Used for MonitorTray branding
- Configured in Tailwind config within each HTML file

### Key Features to Highlight
- Both applications are 100% free with no ads or subscriptions
- Privacy-focused (all data stored locally)
- Lightweight and fast
- Built on .NET 8.0

## Common Tasks

### Update Download Links
Search for `href="#"` in all HTML files and replace with actual download URLs when installers are ready.

### Modify Content
Edit the HTML files directly. Content is organized into semantic sections with clear headings.

### Change Styling
Modify the Tailwind config at the top of each HTML file, or add custom CSS classes.

## Deployment

This static site can be deployed to:
- GitHub Pages
- Netlify (drag-and-drop deployment)
- Vercel
- AWS S3
- Azure Static Web Apps
- Any static hosting service

See README.md for detailed deployment instructions.
