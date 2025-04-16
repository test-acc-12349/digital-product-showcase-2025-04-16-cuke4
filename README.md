# Digital Product Showcase
### A curated directory of cutting-edge digital products and services

![Digital Product Showcase](assets/images/hero-banner.png)

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Getting Started](#getting-started)
- [Directory Structure](#directory-structure)
- [Customization Guide](#customization-guide)
- [Deployment](#deployment)
- [Custom Domain Setup](#custom-domain-setup)
- [Troubleshooting](#troubleshooting)
- [Support & Resources](#support--resources)

## Overview
Digital Product Showcase is a modern directory website featuring a responsive 3-column grid layout designed to highlight digital products and services. The platform offers intuitive navigation, category filtering, and a clean, professional design optimized for showcasing digital offerings.

## Features
- Responsive 3-column grid layout
- Category-based filtering system
- Search functionality
- Dynamic hero section
- Lazy loading images
- Mobile-friendly design
- SEO optimized structure
- Custom category labels
- Sort and filter options

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn
- Basic knowledge of HTML/CSS

### Installation
```bash
# Clone the repository
git clone https://github.com/yourusername/digital-product-showcase.git

# Navigate to project directory
cd digital-product-showcase

# Install dependencies
npm install

# Start development server
npm run dev
```

## Directory Structure
```
digital-product-showcase/
├── assets/
│   ├── images/
│   ├── css/
│   └── js/
├── components/
│   ├── Directory.js
│   ├── Hero.js
│   └── Navigation.js
├── data/
│   ├── products.json
│   └── categories.json
├── pages/
│   ├── index.js
│   └── about.js
└── public/
```

## Customization Guide

### Adding Directory Items
1. Navigate to `data/products.json`
2. Add new items following this structure:
```json
{
  "id": "unique-id",
  "title": "Product Name",
  "description": "Product description",
  "category": "category-slug",
  "image": "/assets/images/product-image.jpg",
  "url": "https://product-url.com"
}
```

### Modifying Category Labels
Edit `data/categories.json`:
```json
{
  "categories": [
    {
      "slug": "saas",
      "name": "SaaS Products",
      "description": "Software as a Service solutions"
    }
  ]
}
```

### Updating Hero Section
1. Open `components/Hero.js`
2. Modify the content:
```jsx
<div className="hero">
  <h1>Your New Title</h1>
  <p>Your new description</p>
</div>
```

### Customizing Colors
1. Navigate to `assets/css/variables.css`
2. Update color variables:
```css
:root {
  --primary-color: #your-color;
  --secondary-color: #your-color;
  --text-color: #your-color;
}
```

## Deployment

### Build for Production
```bash
# Generate production build
npm run build

# Test production build locally
npm run start
```

### Deploy to Hosting
```bash
# Deploy to Vercel
vercel

# Deploy to Netlify
netlify deploy
```

## Custom Domain Setup

1. Purchase domain from preferred registrar
2. Add DNS records:
```
A     @     76.76.21.21
CNAME www   your-site.vercel.app
```
3. Configure in hosting platform:
   - Navigate to domain settings
   - Add custom domain
   - Verify DNS configuration

## Troubleshooting

### Common Issues

#### Images Not Loading
- Verify image path in products.json
- Check image dimensions (max: 1200x800px)
- Ensure proper image format (jpg/png/webp)

#### Category Filters Not Working
- Check category slugs match in both files
- Clear browser cache
- Verify JSON syntax

## Support & Resources

### Documentation
- [Component API Reference](docs/api-reference.md)
- [Styling Guide](docs/styling-guide.md)
- [Deployment Guide](docs/deployment-guide.md)

### Support Channels
- [GitHub Issues](https://github.com/yourusername/digital-product-showcase/issues)
- [Discord Community](https://discord.gg/digitalshowcase)
- Email: support@digitalshowcase.com

### Additional Resources
- [Contributing Guidelines](CONTRIBUTING.md)
- [Code of Conduct](CODE_OF_CONDUCT.md)
- [License](LICENSE.md)

---

## License
MIT License - see [LICENSE.md](LICENSE.md) for details

## Contributing
Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on contributing to this project.

---

Made with ❤️ by [Your Name/Organization]