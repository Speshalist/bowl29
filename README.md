# Bowl 29 Website

## Overview
This repository contains the static website for Bowl 29 in Leonardtown, MD.
The site highlights storefront dining, full menu content, food truck and catering information, and customer contact options.

## Project Structure
- **index.html** - Main landing page with featured content, storefront location, and contact details
- **menu.html** - Full menu page with core bowls, specials, and catering menu sections
- **storefront.html** - Dedicated storefront page with address details and map embed
- **food-truck.html** - Food truck and catering details for Southern Maryland events
- **styles.css** - Global styles for all pages
- **images/** - Logos, artwork, and food photography assets
- **pdfs/** - Downloadable PDF files for menu and catering materials
- **server.js** - Node.js static server for local development on port 5000

## Technology Stack
- Pure HTML5, CSS3, JavaScript
- jQuery and DataTables for schedule display
- Web3Forms API for contact form submissions
- Google Apps Script integration for dynamic schedule data
- Node.js server for local development

## Key Features
1. **Storefront Information** - Location, map, and customer-ready visit details
2. **Menu Experience** - Full menu plus specials and catering offerings
3. **Food Truck and Catering** - Service area and booking-oriented content
4. **Responsive Design** - Mobile-friendly layout across all pages
5. **Social Media Integration** - Links to Facebook, Instagram, and Snapchat
6. **Online Ordering** - Integration with Clover online ordering

## External Dependencies
- Google Fonts (Poppins)
- jQuery 3.7.1
- DataTables 2.3.2
- Google Apps Script for schedule data
- Web3Forms API (configure via project settings)

## Local Development
1. Install Node.js 18+.
2. From the project root, start the static server:
  ```bash
  node server.js
  ```
3. Open the site at `http://127.0.0.1:5000/`.
4. Stop the server with `Ctrl+C`.

Quick checks:
- Home page: `http://127.0.0.1:5000/`
- Menu page: `http://127.0.0.1:5000/menu.html`
- Storefront page: `http://127.0.0.1:5000/storefront.html`
- Food Truck page: `http://127.0.0.1:5000/food-truck.html`

## Maintenance Notes
- Static assets and pages are served by server.js on port 5000 for local development.
- Keep sitemap.xml and robots.txt in sync with any URL or page structure changes.
- Update metadata and structured data when major content sections are revised.

## Architecture
This is a static website with client-side JavaScript for interactivity and third-party integrations.
All content is served by a lightweight Node.js HTTP server that handles MIME types and cache-control headers.

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
