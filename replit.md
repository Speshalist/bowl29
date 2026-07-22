# Bowl 29 Food Truck Website

## Overview
This is a static website for Bowl 29, a fusion food truck in Lusby, MD. The site features a menu showcase, location schedule, catering information, and contact forms.

## Project Structure
- **index.html** - Main landing page with hero section, featured menu items, location/schedule, about section, and contact form
- **menu.html** - Full menu page with core bowls, daily specials, and catering menus
- **styles.css** - All styling for the website
- **images/** - Directory containing food images, logos, and menu images
- **pdfs/** - Directory containing downloadable PDF menus
- **server.js** - Node.js server to serve static files on port 5000

## Technology Stack
- Pure HTML5, CSS3, JavaScript
- jQuery and DataTables for schedule display
- Web3Forms API for contact form submissions
- Google Apps Script integration for dynamic schedule data
- Node.js server for local development

## Key Features
1. **Dynamic Schedule** - Fetches weekly schedule from Google Sheets via Google Apps Script
2. **Contact Form** - Integrated with Web3Forms API for email submissions
3. **Responsive Design** - Mobile-friendly layout
4. **Catering Menus** - Downloadable PDF menus and image previews
5. **Social Media Integration** - Links to Facebook, Instagram, and Snapchat
6. **Online Ordering** - Integration with foodtruck.pub ordering system

## External Dependencies
- Google Fonts (Poppins)
- jQuery 3.7.1
- DataTables 2.3.2
- Google Apps Script for schedule data
- Web3Forms API (access key: 93da09eb-8351-42fc-a132-4f16f4596fc6)

## Recent Changes
- **2025-11-10**: Imported from GitHub and configured for Replit environment
  - Created Node.js server to serve static files on port 5000
  - Configured workflow for automatic server startup
  - Set up deployment configuration for Replit
  - Added .gitignore for Node.js environment

## Architecture
This is a static website with client-side JavaScript for interactivity. The schedule data is cached in localStorage to reduce API calls to Google Sheets. All content is served via a simple Node.js HTTP server that properly handles MIME types and cache control headers.

## SEO TODO Backlog
- [ ] Expand structured data beyond baseline
  - Add consistent Organization or LocalBusiness schema block across all core pages
  - Add BreadcrumbList schema where breadcrumbs are present
  - Consider richer Menu schema coverage on menu page sections
- [ ] Image SEO pass
  - Add descriptive alt text audit for all high-value images
  - Add explicit width and height attributes to key page images to improve CLS
  - Prefer modern formats and compress oversized assets where possible
- [ ] Internal linking pass
  - Add contextual in-body links between Home, Menu, Storefront, Food Truck, Contact, and Catering sections
  - Use anchor text aligned to target intent (ramen, poke, catering, storefront)
- [ ] Local SEO consistency pass
  - Verify NAP consistency (name, address, phone) across page copy, schema, and contact references
  - Normalize formatting and punctuation of address details across all pages
- [ ] Sitemap maintenance improvements
  - Keep sitemap lastmod values current with page changes
  - Evaluate optional image sitemap entries for top visuals
- [ ] Technical hardening
  - Add custom 404 page
  - Confirm redirect policy for www/non-www and trailing slash consistency
  - Run and fix mobile performance issues (especially media-heavy sections)
- [ ] Long-tail content expansion
  - Add concise FAQ and page copy for local-intent terms (ramen in Leonardtown, poke bowls Leonardtown, food truck catering Southern Maryland)
  - Refresh copy quarterly based on seasonal offerings and events
