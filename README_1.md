# Shiva Sons Technologies — Website

> Simple B2B tools that save time and grow your business.

The official marketing website for **Shiva Sons Technologies** — a Regina, Saskatchewan SaaS company selling [ReviewFlow](#reviewflow) and [FixTrack](#fixtrack) to Canadian small businesses and landlords.

🌐 **Live site:** [shivasonstech.ca](https://shivasonstech.ca) *(coming soon)*

---

## Products

### ReviewFlow
Automatically collect 5-star Google reviews after appointments and manage all your reviews in one inbox. Built for local clinics, salons, gyms, contractors, and auto shops.

### FixTrack
Simple maintenance request tracker for small landlords and property managers. Tenants submit requests with photos, landlords manage everything from one dashboard.

---

## Tech Stack

| Layer | Tool |
|---|---|
| Framework | Next.js 14 (App Router) |
| Styling | Tailwind CSS |
| Components | shadcn/ui |
| Language | TypeScript |
| Hosting | Cloudflare Pages |
| Version Control | GitHub |
| Forms | Formspree |
| Analytics | Google Analytics 4 + Microsoft Clarity |

---

## Getting Started

### Prerequisites

- Node.js 18+ ([download](https://nodejs.org))
- Git ([download](https://git-scm.com))
- A code editor — we use VS Code

### Installation

```bash
# 1. Clone the repo
git clone https://github.com/YOUR_USERNAME/shiva-sons-website.git

# 2. Move into the project folder
cd shiva-sons-website

# 3. Install dependencies
npm install

# 4. Start the development server
npm run dev
```

Then open [http://localhost:3000](http://localhost:3000) in your browser.

---

## Project Structure

```
shiva-sons-website/
├── app/                        # Next.js App Router pages
│   ├── page.tsx                # Home
│   ├── pricing/page.tsx        # Pricing Plans
│   ├── services/page.tsx       # Our Services
│   ├── about/page.tsx          # About Us
│   ├── contact/page.tsx        # Contact Us
│   ├── careers/page.tsx        # Careers
│   ├── login/page.tsx          # Log In
│   ├── signup/page.tsx         # Sign Up
│   └── dashboard/page.tsx      # Dashboard (Coming Soon)
├── components/                 # Shared components
│   ├── Navbar.tsx
│   ├── Footer.tsx
│   ├── ProductCard.tsx
│   ├── PricingTable.tsx
│   └── ContactForm.tsx
├── public/                     # Static assets
│   ├── images/
│   └── logo.svg
├── tailwind.config.ts          # Brand color configuration
└── README.md
```

---

## Brand Colors

| Name | Hex | Usage |
|---|---|---|
| Orange (Primary) | `#F97316` | Buttons, highlights, ReviewFlow |
| Navy | `#1E3A5F` | Navbar, headings, FixTrack |
| Blue | `#2563EB` | Links, accents |
| White | `#FFFFFF` | Page backgrounds |
| Text | `#1F2937` | Body copy |

**Fonts:** Space Grotesk (headings) · Inter (body)

---

## Pages Checklist

- [ ] Home page
- [ ] Pricing Plans (ReviewFlow + FixTrack)
- [ ] Our Services
- [ ] About Us
- [ ] Contact Us
- [ ] Careers
- [ ] Log In
- [ ] Sign Up
- [ ] Dashboard (Coming Soon placeholder)
- [ ] Privacy Policy
- [ ] Terms of Service

---

## Deployment

This site deploys automatically via **Cloudflare Pages**.

Every push to the `main` branch triggers a new deployment. Pull requests get a preview URL automatically.

**Build settings:**
```
Framework:        Next.js
Build command:    npm run build
Output directory: .next
Node version:     18
```

---

## Environment Variables

Create a `.env.local` file in the root for local development:

```bash
# Formspree (contact form)
NEXT_PUBLIC_FORMSPREE_ID=your_form_id_here

# Google Analytics
NEXT_PUBLIC_GA_ID=G-XXXXXXXXXX
```

> ⚠️ Never commit `.env.local` to GitHub. It's already in `.gitignore`.

---

## Contributing

This is a private company project. If you're working on this repo:

1. Create a branch for your feature: `git checkout -b feature/contact-page`
2. Make your changes and commit: `git commit -m "Add contact page form"`
3. Push your branch: `git push origin feature/contact-page`
4. Open a Pull Request into `main`

**Commit message format:**
```
Add [thing]         → new feature or page
Fix [thing]         → bug fix
Update [thing]      → changes to existing content
Remove [thing]      → deleted something
```

---

## Contact

**Shiva Sons Technologies**
📧 support@shivasonstech.ca
📍 Regina, Saskatchewan, Canada
🌐 shivasonstech.ca

---

© 2026 Shiva Sons Technologies. All rights reserved.
