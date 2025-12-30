# StudioX - Creative Portfolio Landing Page

A high-converting, marketing-first landing page for freelance graphic designers and video editors targeting startups and local businesses.

## 🚀 Quick Start

```bash
npm install
npm run dev
```

## 📝 How to Edit Content

### Headlines (Hero Section)
Edit `src/components/HeroSection.tsx`:

**Headline Options (choose one):**
1. "Captivating brand videos that help startups grow."
2. "Video & design that turns local audiences into customers."
3. "Standout visuals for startups ready to scale."

**Subheadline Example:**
"Short reels, crisp brand design, measurable results — built for startups and local businesses."

### CTA Button Text Options
- "Request Quote"
- "See Portfolio"
- "Book a Call"

### Portfolio Projects
Edit `src/components/PortfolioSection.tsx` - the `projects` array contains all portfolio items.

**Project Caption Templates:**
1. "Brand Reel for [Client]: Problem — low local awareness. Solution — 30s social reel. Result — 40% uplift in engagement."
2. "Logo & Packaging for [Client]: Problem — inconsistent brand. Solution — full identity kit. Result — faster product recognition."
3. "Promo Video for [Client]: Problem — low event turnout. Solution — teaser video + IG story edits. Result — tickets sold out."

### Testimonials
Edit `src/components/TestimonialsSection.tsx` - update the `testimonials` array with real client quotes.

### Contact Information
Edit `src/components/ContactSection.tsx`:
- Email address
- Phone number
- Booking link for calendar integration

### Social Links
Edit `src/components/Footer.tsx` - update YouTube, Instagram, and LinkedIn URLs.

## 🖼️ Replacing Images

Images are stored in `src/assets/`:
- `hero-bg.jpg` - Hero background (1920x1080 recommended)
- `portfolio-1.jpg` through `portfolio-6.jpg` - Portfolio thumbnails (800x800 recommended)

Import images in components like:
```tsx
import heroImage from "@/assets/hero-bg.jpg";
```

## 🎨 Customizing Colors

Edit `src/index.css` for the design system:

```css
:root {
  --primary: 12 90% 60%;        /* Coral accent color */
  --background: 220 20% 8%;     /* Dark background */
  --foreground: 0 0% 95%;       /* Light text */
}
```

The 60/30/10 rule:
- 60% Dark charcoal background
- 30% Lighter grays (cards, sections)
- 10% Coral accent (CTAs, highlights)

## 📊 Analytics Setup

### Google Analytics (GA4)
Add to `index.html` before `</head>`:

```html
<!-- Google tag (gtag.js) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

Replace `G-XXXXXXXXXX` with your GA4 Measurement ID.

## 🧪 A/B Testing Recommendations

### Test 1: Hero Headline
- Variant A: "Captivating brand videos that help startups grow."
- Variant B: "Video & design that turns local audiences into customers."
- Variant C: "Standout visuals for startups ready to scale."

### Test 2: CTA Button Color
- Variant A: Coral (#F97316)
- Variant B: Green (#22C55E)
- Variant C: Blue (#3B82F6)

### Test 3: Hero Media
- Variant A: Static image background
- Variant B: Looping video background

### Test 4: CTA Text
- Variant A: "Request Quote"
- Variant B: "Book a Call"
- Variant C: "Get Started"

## ✅ Launch Checklist

### Before Launch
- [ ] Replace placeholder images with real portfolio work
- [ ] Update all contact information
- [ ] Add real testimonials with client permission
- [ ] Update meta tags in `index.html`
- [ ] Add favicon and OG image
- [ ] Set up contact form backend (email/database)
- [ ] Connect analytics
- [ ] Test on mobile devices
- [ ] Check all links work
- [ ] Compress images for performance

### SEO Checklist
- [ ] Title tag under 60 characters
- [ ] Meta description under 160 characters
- [ ] Single H1 tag per page
- [ ] Alt text on all images
- [ ] Schema.org structured data present
- [ ] Canonical URL set
- [ ] Mobile-friendly design

### Accessibility
- [ ] Keyboard navigation works
- [ ] Color contrast passes WCAG AA
- [ ] ARIA labels on interactive elements
- [ ] Focus states visible

## 📧 Form Microcopy

**Success Message:**
"Thanks for reaching out! I'll review your project details and get back to you within 24 hours."

**Error Messages:**
- Empty name: "Name is required"
- Invalid email: "Please enter a valid email"
- Message too long: "Message must be less than 1000 characters"

**Privacy Note:**
"Your info is safe. I'll only use it to respond to your inquiry — no spam, ever."

## 🚀 Deployment

### Lovable (Recommended)
Click the "Publish" button in the Lovable editor.

### Vercel
```bash
npm run build
# Deploy the `dist` folder to Vercel
```

### Netlify
```bash
npm run build
# Drag and drop `dist` folder to Netlify
```

## 📁 Project Structure

```
src/
├── assets/          # Images and media
├── components/
│   ├── ui/          # Reusable UI components
│   ├── HeroSection.tsx
│   ├── PortfolioSection.tsx
│   ├── TestimonialsSection.tsx
│   ├── ProcessSection.tsx
│   ├── ContactSection.tsx
│   ├── Footer.tsx
│   └── Navbar.tsx
├── hooks/           # Custom React hooks
├── lib/             # Utilities
├── pages/
│   └── Index.tsx    # Main landing page
├── index.css        # Design system (colors, fonts)
└── main.tsx         # App entry point
```

## 📞 Support

Built with Lovable using React, TypeScript, Tailwind CSS, and shadcn/ui.
