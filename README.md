# Photography Studio Website

A modern, premium photography studio website built with Next.js, TypeScript, and Tailwind CSS.

## Features

- **Homepage**: Hero slideshow, service previews, and quick links
- **About Us**: Studio introduction, photographer profile, vision, values, and specialties
- **Services**: Detailed service listings with pricing
- **Portfolio/Gallery**: Filterable image gallery with categories
- **Booking System**: Appointment booking form with date/time selection
- **Contact**: Contact form and studio information
- **Testimonials**: Client reviews and ratings
- **Pricing**: Package options and add-ons
- **Content Manager**: Admin interface for managing gallery and testimonials

## Tech Stack

- **Next.js 14** - React framework with App Router
- **TypeScript** - Type-safe development
- **Tailwind CSS** - Utility-first CSS framework
- **React Icons** - Icon library

## Getting Started

### Prerequisites

- Node.js 18+ and npm/yarn

### Installation

1. Install dependencies:
```bash
npm install
```

2. Run the development server:
```bash
npm run dev
```

3. Open [http://localhost:3000](http://localhost:3000) in your browser

## Project Structure

```
├── app/                    # Next.js app directory
│   ├── about/             # About Us page
│   ├── services/          # Services page
│   ├── portfolio/         # Portfolio/Gallery page
│   ├── booking/           # Booking page
│   ├── contact/           # Contact page
│   ├── testimonials/      # Testimonials page
│   ├── pricing/           # Pricing page
│   └── content-manager/   # Content Manager section
│       ├── gallery/       # Gallery management
│       └── testimonials/  # Testimonials management
├── components/            # Reusable components
│   ├── Navbar.tsx
│   ├── Footer.tsx
│   └── HeroSlideshow.tsx
├── data/                  # TypeScript data files
│   ├── heroSlides.ts
│   ├── services.ts
│   ├── gallery.ts
│   ├── testimonials.ts
│   ├── packages.ts
│   ├── about.ts
│   ├── contact.ts
│   └── blog.ts
└── types/                 # TypeScript type definitions
    └── index.ts
```

## Content Management

All content is stored in TypeScript files in the `/data` directory. This makes it easy to update content without touching the code:

- `data/heroSlides.ts` - Homepage hero slideshow images
- `data/services.ts` - Service listings and pricing
- `data/gallery.ts` - Portfolio gallery images
- `data/testimonials.ts` - Client testimonials
- `data/packages.ts` - Pricing packages and add-ons
- `data/about.ts` - About page content
- `data/contact.ts` - Contact information

### Content Manager

Access the Content Manager at `/content-manager` to:
- Manage gallery images (add, edit, delete)
- Manage testimonials (add, edit, delete)

**Note**: Changes in the Content Manager are currently stored in component state. To make permanent changes, update the data files in the `/data` folder.

## Customization

### Colors

The website uses a black-white-gold color scheme. Customize colors in `tailwind.config.js`:

```javascript
colors: {
  gold: {
    // Gold color variations
  }
}
```

### Fonts

The website uses:
- **Playfair Display** - For headings (serif)
- **Inter** - For body text (sans-serif)

Fonts are configured in `app/layout.tsx` and `app/globals.css`.

## Building for Production

```bash
npm run build
npm start
```

## SEO Optimization

- Semantic HTML structure
- Meta tags in layout.tsx
- Image alt text for accessibility
- Fast-loading optimized images with Next.js Image component

## Mobile Responsive

The website is fully responsive and works on:
- Mobile devices
- Tablets
- Desktop computers

## License

This project is created for demonstration purposes.

