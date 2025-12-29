# KoyeTech - Static HTML Version

## Project Overview

This is a complete conversion of the KoyeTech React/Next.js website to static HTML with the same design, layout, colors, animations, and content.

## What's Included

### Pages Created:
1. **index.html** - Homepage with hero section, core services, work process, unique benefits, and office information
2. **business-solutions.html** - Business Solutions with Product Management, Product Development, AIML, Healthcare Interoperability, and Data Analytics sections
3. **accelerators.html** - Accelerators program with domain-specific solutions and execution pods
4. **talent-solution.html** - Talent Solutions with Contract Staff Augmentation, Firm Hire, and Contract-to-Hire options
5. **contact.html** - Contact page with contact form, office locations, and contact information
6. **company.html** - Company page with mission, vision, values, and statistics
7. **career.html** - Careers page with job listings and company culture information

### Files:
- **css/styles.css** - Comprehensive CSS stylesheet with all styles, animations, and responsive design
- All pages are fully responsive and work on mobile, tablet, and desktop

## Design & Styling

### Color Scheme:
- **Primary Blue**: #0ea5e9
- **Dark Blue**: #0284c7
- **Light Blue**: #38bdf8
- **Text Dark**: #0f172a
- **Text Muted**: #475569
- **Background**: #f8fafc

### Features:
- ✅ Same layout and alignment as React version
- ✅ Same animations (fade-in-up, scale-in, float)
- ✅ Same header with navigation and dropdown menus
- ✅ Same footer with company information and links
- ✅ Responsive design (mobile, tablet, desktop)
- ✅ Consistent color scheme and typography
- ✅ Interactive elements (dropdowns, accordions, hover effects)
- ✅ Contact form with client-side validation
- ✅ Smooth scrolling and transitions

## Navigation Structure

### Main Navigation Menu:
- Home (/)
- Company (company.html)
- Business Solutions (business-solutions.html)
  - Product Management
  - Product Development
  - AIML Solutions
  - Healthcare Interoperability
  - Data Analytics
- Accelerators (accelerators.html)
- Talent Solution (talent-solution.html)
  - Contract Staff Augmentation
  - Firm Hire Services
  - Contract to Hire
- Career (career.html)
- Contact (contact.html)

## How to Use

### Local Testing:
1. Open any HTML file in a web browser
2. All internal links are relative paths (no build required)
3. Navigation works seamlessly between pages

### Deploy to Production:
1. Upload all files to your web server
2. Ensure the folder structure is maintained:
   ```
   /
   ├── index.html
   ├── business-solutions.html
   ├── accelerators.html
   ├── talent-solution.html
   ├── contact.html
   ├── company.html
   ├── career.html
   └── css/
       └── styles.css
   ```

### Add Contact Form Backend:
The contact form on contact.html is set up to POST to `/api/contact`. To make it functional:

1. Set up a backend endpoint that accepts POST requests
2. Update the form submission URL if needed
3. Process the form data (name, email, phone, company, subject, message)
4. Send a confirmation email or save to database

Example form data structure:
```json
{
  "name": "John Doe",
  "email": "john@example.com",
  "phone": "+1234567890",
  "company": "Company Name",
  "subject": "General Inquiry",
  "message": "Message content..."
}
```

## Browser Compatibility

- ✅ Chrome/Edge (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## Responsive Breakpoints

- **Desktop**: 1024px and above
- **Tablet**: 768px to 1023px
- **Mobile**: Below 768px

All styles are optimized for mobile-first responsive design.

## Key Sections & Components

### Header/Navigation
- Sticky header with logo and navigation menu
- Dropdown menus for Business Solutions and Talent Solution
- Mobile hamburger menu with toggle functionality
- Active link highlighting

### Hero Sections
- Large banner with gradient background
- Animated text (fade-in-up animation)
- Call-to-action buttons
- Decorative blur effects

### Cards
- Service/feature cards with hover effects
- Icon displays with emoji
- Titles, descriptions, and action links
- Smooth scale and shadow transitions on hover

### Sections
- Grid-based layouts (2-column, 3-column, 5-column)
- Consistent spacing and padding
- Border separators between sections

### Forms
- Contact form with multiple input types
- Validation on required fields
- Status messages for success/error
- Responsive form layout

### Footer
- Multi-column layout with links
- Social media icons
- Copyright information
- Quick links to all pages

## Customization

### Modify Colors:
Edit the CSS variables in `css/styles.css`:
```css
:root {
  --color-brand-primary: #0ea5e9;
  --color-brand-dark: #0284c7;
  /* ... more colors ... */
}
```

### Change Content:
Simply edit the HTML content in any file. All text, headings, and descriptions are easy to locate and update.

### Update Links:
All relative links use standard HTML paths. Update href attributes to match your URL structure.

### Add Images:
Replace `/images/` paths with your actual image locations. The site currently references:
- /images/business-solutions.png
- /images/accelerators.png
- /images/talent-solutions.png

## Performance Notes

- Lightweight with minimal CSS (no frameworks required)
- No JavaScript dependencies (vanilla JavaScript only)
- Fast loading times
- Mobile-optimized

## Support & Maintenance

All pages follow the same HTML structure and CSS patterns, making it easy to:
- Add new pages
- Update existing content
- Modify styles consistently
- Scale the design

## File Sizes

- CSS: ~35KB (minified would be ~20KB)
- HTML files: Each page is 15-25KB (easily optimizable)
- Total size: Very lightweight with no external dependencies

## Next Steps

1. **Images**: Add actual product/team images to `/images/` folder
2. **Backend**: Implement the contact form endpoint
3. **Analytics**: Add Google Analytics or similar tracking
4. **Meta Tags**: Update Open Graph and social media tags in each page's `<head>`
5. **Domain**: Point your domain to the web server hosting these files
6. **SEO**: Update meta descriptions and keywords

## Contact Form Setup Example

If using a simple backend, the form will POST to `/api/contact` with the following payload:
```javascript
{
  "name": "string",
  "email": "string",
  "phone": "string",
  "company": "string",
  "subject": "string",
  "message": "string"
}
```

Implement appropriate validation, spam protection, and email notifications on your backend.

---

**Created**: 2025  
**Technology**: Pure HTML5 + CSS3 + Vanilla JavaScript  
**Status**: Ready for deployment
