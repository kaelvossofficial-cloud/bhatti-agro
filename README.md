# BHATTI AGRO SOLUTIONS PAKISTAN - Website

A production-ready agricultural solutions website with modern design and full functionality.

## Pages

- **index.html** - Homepage with hero section, trust indicators, product showcase, and CTAs
- **about.html** - Company information, leadership team, timeline, and certifications
- **products.html** - Product catalog with filtering, comparison, and detail modals
- **contact.html** - Contact forms, support channels, and dealer application
- **admin.html** - Admin dashboard for lead management and analytics

## Features Implemented

### 1. Functional Navigation
- Desktop navigation with active states
- Mobile responsive menu with hamburger toggle
- Smooth scroll behavior
- Cross-page linking

### 2. Responsive Behavior
- Mobile-first design approach
- Breakpoints at sm (640px), md (768px), lg (1024px)
- Mobile menu slide-in animation
- Responsive grids and layouts

### 3. Product Catalog
- Grid layout with product cards
- Category filtering sidebar
- Sort functionality
- Pagination controls
- Product comparison drawer

### 4. Product Detail Pages
- Modal-based product details
- Image gallery
- Specifications display
- Bulk quote request form

### 5. Contact Forms
- Inquiry form with validation
- Business type selection
- Region/city input
- Message textarea

### 6. WhatsApp Integration
- Floating WhatsApp button
- Click-to-chat functionality
- Pre-filled messages
- Support channel links

### 7. Admin Dashboard
- Lead management interface
- Analytics charts (Chart.js)
- Stats overview cards
- Export functionality

### 8. Supabase Backend
- Client library included
- Lead capture functions
- Ready for configuration
- Error handling

### 9. Lead Capture System
- Form submission handlers
- Database integration ready
- Local fallback logging
- Status tracking

### 10. SEO Optimization
- Meta descriptions
- Open Graph tags
- Twitter Card metadata
- Canonical URLs
- Semantic HTML structure
- Alt text for images

## Configuration Required

### Supabase Setup
1. Create a Supabase project at https://supabase.com
2. Create a `leads` table:
```sql
CREATE TABLE leads (
  id UUID DEFAULT gen_random_uuid() PRIMARY KEY,
  name TEXT,
  email TEXT,
  phone TEXT,
  business_type TEXT,
  message TEXT,
  created_at TIMESTAMP WITH TIME ZONE DEFAULT NOW()
);
```
3. Update credentials in each HTML file:
```javascript
const SUPABASE_URL = 'https://your-project.supabase.co';
const SUPABASE_ANON_KEY = 'your-anon-key';
```

### WhatsApp Number
Update the phone number in `openWhatsApp()` function:
```javascript
const phoneNumber = '923001234567'; // Replace with actual number
```

## Tech Stack
- Tailwind CSS (CDN)
- Google Fonts (Inter, Plus Jakarta Sans)
- Material Symbols Icons
- Chart.js (Admin dashboard)
- Supabase (Backend)

## File Structure
```
/workspace/
├── index.html      # Homepage
├── about.html      # About/Company page
├── products.html   # Product catalog
├── contact.html    # Contact & Support
├── admin.html      # Admin dashboard
└── README.md       # Documentation
```

## Browser Support
- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers

## License
© 2024 Bhatti Agro Solutions Pakistan. All rights reserved.
