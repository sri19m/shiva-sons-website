# Shiva Sons Technologies — Website

> Simple B2B tools that save time and grow your business.

The official marketing website for **Shiva Sons Technologies** — a Regina, Saskatchewan micro-SaaS company building focused tools for small landlords and local service businesses across Canada.

🌐 **Live site:** [shivasonstech.ca](https://shivasonstech.ca) *(coming soon)*

---

## Products

### 🏠 FixTrack by Shiva Sons
Simple maintenance request tool for small landlords.

Full property-management software is built for big companies and costs $100+/month. Small landlords with 3–10 units just want something cheap and simple. FixTrack gives tenants a link to submit maintenance requests with photos, and gives landlords a clean dashboard to track everything — no more messy WhatsApp threads and spreadsheets.

**Pricing**
| Plan | Price | Units |
|---|---|---|
| Starter | $15/month | Up to 10 units |
| Pro | $29/month | Up to 30 units |
| Business | $49/month | Up to 100 units |

---

### ⭐ TestiFlow by Shiva Sons
AI-powered testimonial collector for small businesses.

Businesses know testimonials sell, but they rarely ask in a systematic way. TestiFlow automatically messages customers after a purchase or appointment asking for a short text or video testimonial, then gathers all the best ones in one dashboard — ready to embed on your website, landing pages, and ads.

**Pricing**
| Plan | Price | Requests/Month |
|---|---|---|
| Starter | $29/month | Up to 100 requests |
| Pro | $49/month | Up to 500 requests |
| Business | $79/month | Up to 2,000 requests |

---

### 🎁 Client Referral Program
Applies to both products. Refer a friend who signs up for any paid plan → get 1 free month of your current plan. Maximum 5 referrals per year (5 free months max).

---

## Tech Stack

| Layer | Tool |
|---|---|
| Framework | Next.js 14 (App Router) |
| Styling | Tailwind CSS |
| Components | shadcn/ui |
| Language | TypeScript |
| Database & Auth | Supabase (PostgreSQL) |
| Payments | Lemon Squeezy (start) → Stripe at scale |
| Transactional Email | Resend (100/day free) |
| Marketing Email | Brevo (300/day free) |
| CRM | HubSpot Free |
| Hosting | Cloudflare Pages |
| CI/CD | GitHub Actions |
| Version Control | GitHub |
| Analytics | Google Analytics 4 + Microsoft Clarity |
| Domain | Cloudflare Registrar |

---

## Getting Started

### Prerequisites
- Node.js 18+ ([download](https://nodejs.org))
- Git ([download](https://git-scm.com))
- VS Code ([download](https://code.visualstudio.com))

### VS Code Extensions
Install these before writing a line of code:
- **Live Server** — preview HTML/CSS instantly
- **Prettier** — auto-format code on save
- **ESLint** — catch JavaScript errors early
- **Tailwind CSS IntelliSense** — autocomplete for Tailwind classes
- **Codeium** (free) or **GitHub Copilot** — AI code completion

### Installation

```bash
# 1. Clone the repo
git clone https://github.com/YOUR_USERNAME/shiva-sons-website.git

# 2. Move into the project folder
cd shiva-sons-website

# 3. Install dependencies
npm install

# 4. Copy environment variables template
cp .env.example .env.local

# 5. Start the development server
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

---

## Project Structure

```
shiva-sons-website/
├── app/                         # Next.js App Router pages
│   ├── page.tsx                 # Home
│   ├── services/page.tsx        # Our Services (FixTrack + TestiFlow)
│   ├── pricing/page.tsx         # Pricing Plans + Referral Program
│   ├── about/page.tsx           # About Us
│   ├── contact/page.tsx         # Contact Us
│   ├── careers/page.tsx         # Careers
│   ├── login/page.tsx           # Log In
│   ├── signup/page.tsx          # Sign Up
│   ├── dashboard/page.tsx       # Dashboard (Coming Soon)
│   ├── privacy/page.tsx         # Privacy Policy
│   └── terms/page.tsx           # Terms of Service
├── components/                  # Shared components
│   ├── layout/
│   │   ├── Navbar.tsx
│   │   └── Footer.tsx
│   ├── home/
│   │   ├── HeroSection.tsx
│   │   ├── ProductsSection.tsx
│   │   ├── WhyChooseUs.tsx
│   │   └── CtaBanner.tsx
│   ├── pricing/
│   │   ├── PricingTable.tsx
│   │   └── ReferralBanner.tsx
│   └── shared/
│       ├── ProductCard.tsx
│       ├── ContactForm.tsx
│       └── SearchModal.tsx
├── public/                      # Static assets
│   ├── images/
│   │   ├── hero/
│   │   ├── products/
│   │   └── icons/
│   └── logo.svg
├── lib/                         # Utilities and config
│   └── utils.ts
├── .env.example                 # Environment variable template
├── tailwind.config.ts           # Brand color + font config
└── README.md
```

---

## Brand

### Colors
| Name | Hex | Usage |
|---|---|---|
| Orange (Primary) | `#F97316` | Buttons, highlights, CTAs |
| Navy (Secondary) | `#1E3A5F` | Navbar, headings, FixTrack |
| Blue | `#2563EB` | Links, accents |
| White | `#FFFFFF` | Page backgrounds |
| Off-white | `#F9FAFB` | Section backgrounds |
| Text | `#1F2937` | Body copy |

### Typography
- **Headlines:** Space Grotesk (700) — modern, geometric, tech feel
- **Body:** Inter (400/500) — clean, readable
- **Code:** JetBrains Mono

### Tone
Professional but friendly. Simple English. No corporate jargon. Canadian.

---

## Environment Variables

Create a `.env.local` file from the template:

```bash
cp .env.example .env.local
```

```bash
# Supabase
NEXT_PUBLIC_SUPABASE_URL=your_supabase_project_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key

# Lemon Squeezy (payments)
LEMONSQUEEZY_API_KEY=your_api_key
LEMONSQUEEZY_STORE_ID=your_store_id
NEXT_PUBLIC_FIXTRACK_STARTER_LINK=your_checkout_link
NEXT_PUBLIC_FIXTRACK_PRO_LINK=your_checkout_link
NEXT_PUBLIC_FIXTRACK_BUSINESS_LINK=your_checkout_link
NEXT_PUBLIC_TESTIFLOW_STARTER_LINK=your_checkout_link
NEXT_PUBLIC_TESTIFLOW_PRO_LINK=your_checkout_link
NEXT_PUBLIC_TESTIFLOW_BUSINESS_LINK=your_checkout_link

# Resend (transactional email)
RESEND_API_KEY=your_resend_api_key

# Google Analytics
NEXT_PUBLIC_GA_ID=G-XXXXXXXXXX
```

> ⚠️ Never commit `.env.local` to GitHub. It is already in `.gitignore`.

---

## Pages Checklist

- [ ] Home
- [ ] Our Services (FixTrack + TestiFlow detail)
- [ ] Pricing Plans (both products + referral program + FAQ)
- [ ] About Us
- [ ] Contact Us
- [ ] Careers (+ resume upload form)
- [ ] Log In
- [ ] Sign Up
- [ ] Dashboard (Coming Soon placeholder)
- [ ] Privacy Policy
- [ ] Terms of Service

---

## Deployment

This site deploys automatically via **Cloudflare Pages**.

Every push to `main` triggers a production deployment.
Every pull request gets an isolated preview URL.

**Build settings in Cloudflare Pages:**
```
Framework preset:  Next.js
Build command:     npm run build
Output directory:  .next
Node version:      18
```

---

## Git Workflow

```bash
# Start a new piece of work
git checkout -b feature/pricing-page

# Save progress
git add .
git commit -m "Add pricing page — FixTrack + TestiFlow tiers"

# Push and open a PR
git push origin feature/pricing-page
```

**Commit message format:**
```
Add [thing]      → new page, feature, or component
Fix [thing]      → bug or visual issue
Update [thing]   → content or copy change
Remove [thing]   → deleted code or file
```

---

## Contact

**Shiva Sons Technologies**
📧 support@shivasonstech.ca
📍 Regina, Saskatchewan, Canada
🌐 shivasonstech.ca

---

© 2026 Shiva Sons Technologies. All rights reserved.
