# Altara Energy Website Project Brief
**For Claude Code Implementation**

---

## Project Overview

Build a Jekyll-based website for **Altara Energy** (altaraenergy.com) to be hosted on GitHub Pages. Altara Energy is a city convenience EV charging network designed for high-traffic city locations with fast, reliable charging and flexible site partnerships.

**Brand Architecture:**
- **Altara** is a standalone brand with its own identity and positioning
- Operates as a traditional CPO with flexibility for site host partnerships, retail locations, and various business models
- No visible connection to other brands except through shared loyalty program (Pathfinder Network)
- **Behind the scenes**: Altara is operated by Rangeway Energy, sharing NOC and operational systems, but this is not customer-facing

**Key Brand Positioning:**
- **Standalone brand**: Altara stands on its own credibility, not endorsed by other brands
- **Operational flexibility**: Can partner with various site hosts, retailers, and property owners
- **Traditional CPO model**: Not constrained by premium hospitality promises or experience guarantees
- **Pathfinder Network member**: Participates in Pathfinder Rewards loyalty network alongside other charging brands

---

## Brand Positioning

### Core Identity
- **Category**: City convenience EV charging
- **Tagline**: "Power up, move forward"
- **Promise**: Fast, reliable charging where you need it, when you need it
- **Target Customer**: City drivers, ride-share/delivery drivers, daily commuters, fleet operators
- **Loyalty Program**: Pathfinder Rewards—a charging network loyalty program accepted at Altara and partner locations
- **Social Handles**: @altaraev (consistent across Twitter/X, Instagram, LinkedIn)
- **Language Note**: Avoid "urban areas" in public-facing copy—use specific city names, "cities," or "convenient locations" instead

### Brand Personality
- **Efficient**: Quick in-and-out, optimized for busy lives
- **Accessible**: City locations, straightforward pricing, no frills
- **Reliable**: Real-time monitoring, professional operations
- **Flexible**: Adaptable to various site hosts and partnership models

### Visual Direction (Urban Current Edition v2.0)
- **Color Palette**: 
  - **Current Teal** (Primary): `#0891B2` - Modern, energetic, professional
  - **Ember Orange** (Accent): `#F97316` - Warm, active, high-visibility
  - **Deep Teal** (Supporting): `#0E7490` - Darker contrast, depth
  - **Bright Orange** (Supporting): `#FB923C` - Hover states, lighter accent
  - **Concrete** (Neutral): `#9CA3AF` - Light text, borders
  - **Slate** (Dark): `#334155` - Body text, dark UI elements
  - **White**: `#FFFFFF` - Backgrounds
  - **Gradient**: Ember Orange → Current Teal → Ember Orange (logo orbital ring); Current Teal → Deep Teal (hero backgrounds)
- **Logo**: Circular orbital ring with gradient stroke (orange-teal-orange), "A" symbol in Current Teal at center
  - Available variants: standard (full color with gradient), monochrome white, monochrome teal, small size optimized, horizontal lockup with wordmark
  - Minimum sizes: 32px icon only, 120px horizontal lockup
- **Typography**: Outfit (primary typeface via Google Fonts)
  - Modern geometric sans-serif with slightly rounded forms
  - Weights: Semi-Bold (600) for headings, Regular (400) for body, Medium (500) for labels/UI
  - Fallback stack: `'Outfit', -apple-system, BlinkMacSystemFont, 'Segoe UI', system-ui, sans-serif`
- **Tone**: Modern, clean, efficient, approachable, energetic
- **Imagery**: City streetscapes, EV drivers in cities, convenience store interiors, busy professionals, modern locations
  - **Note**: Show city environments in imagery, but avoid "urban" language in copy—use specific city names instead

### What Altara IS NOT
- Not premium/luxury positioning
- Not scenic/destination-focused
- Not hospitality-first (it's convenience-first)
- Not boutique/artisanal

---

## Technical Requirements

### Platform
- **Static Site Generator**: Jekyll 4.x
- **Hosting**: GitHub Pages compatible
- **Domain**: altaraenergy.com
- **Responsive**: Mobile-first design, fully responsive

### Performance
- Fast load times (<2s)
- Optimized images (WebP with fallbacks)
- Minimal JavaScript (progressive enhancement)
- Accessible (WCAG 2.1 AA compliant)

### Dependencies
- Jekyll 4.x
- jekyll-seo-tag
- jekyll-sitemap
- Minimal additional plugins (GitHub Pages compatible only)

---

## Site Structure

### Primary Pages

#### 1. Homepage (`index.html`)
**Purpose**: Communicate value proposition quickly, drive to station locator

**Key Sections**:
- **Hero**: 
  - Headline: "Fast, Reliable Charging Where You Need It"
  - Subhead: "City EV charging designed for your daily drive"
  - CTA: "Find a Station" + "Join Pathfinder Rewards"
- **Value Props** (3 columns):
  - ⚡ Fast Charging: "10+ high-power DC fast chargers at every location"
  - 📍 Convenient Locations: "Convenient sites near your daily routes"
  - 💰 Flat Member Rates: "No time-of-use surprises—one rate, any time"
- **How It Works** (simple 3-step):
  1. Pull in → 2. Plug in → 3. Power up
- **Amenities**: "Each location features comfortable waiting areas, and site-specific amenities like shaded seating, picnic areas, or dog parks"
- **Pathfinder Network**: "Join Pathfinder Rewards—accepted at Altara and partner charging networks"
- **CTA Section**: "Join Pathfinder Rewards" (free membership, works across network)

#### 2. Locations (`locations.html`)
**Purpose**: Help users find stations (even if none exist yet)

**Content**:
- "Coming Soon" map with planned markets
- City list: "Launching in: San Francisco Bay Area, Los Angeles, San Diego" (or specific cities you're targeting)
- Email signup: "Get notified when we open near you"
- Placeholder for future interactive map

#### 3. Membership (`membership.html`)
**Purpose**: Explain Pathfinder Rewards membership and pricing

**Key Content**:
- **Pathfinder Rewards** (multi-network loyalty program):
  - Works at Altara and partner charging networks
  - Free to join
  - Flat rate pricing (no TOU volatility)
  - App-based payments
  - Real-time station availability
  - Usage history and receipts
- **Pricing** (Pathfinder Rewards tiers):
  - Non-members: Time-of-use pricing (Peak/Mid/Off-Peak)
  - Explorer (free): Base flat rate
  - Voyager: 5% credits back on charging
  - Pioneer: 10% credits back (+$100 annual credit)
  - Trailblazer: 15% credits back (+$500 annual credit, invite-only)
- **Network Benefit**: "Your Pathfinder Rewards work at participating charging networks"
- **Partner Networks**: "Accepted at Altara and select partner locations" (leave room for adding Rangeway/others later)
- **CTA**: "Join Free" (email capture for waitlist)

#### 4. For Fleet Operators (`fleet.html`)
**Purpose**: Appeal to ride-share, delivery, and commercial fleet drivers

**Key Content**:
- Fleet-specific benefits (volume discounts, dedicated support)
- Reliability guarantee
- Convenient city locations for route optimization
- Contact form for fleet partnerships

#### 5. Partner with Us (`partners.html`)
**Purpose**: Site host recruitment

**Key Content**:
- "Bring Altara to Your Location"
- Ideal site profiles (high-traffic locations, 0.5+ acre for 10+ chargers)
- Partnership model: Altara installs and operates charging, partners provide or host amenities
- Revenue share opportunity
- Partner application form

#### 6. About (`about.html`)
**Purpose**: Establish credibility and explain Altara's mission

**Key Content**:
- Mission: "Making EV charging as convenient as filling up at your favorite gas station"
- Vision: "Building a city charging network designed for daily drivers, fleet operators, and commuters"
- Technology: Professional network operations center (NOC), real-time monitoring
- Partnership approach: "We partner with retailers, property owners, and businesses to bring charging where you need it"
- Pathfinder Network: "Proud member of the Pathfinder Rewards network"
- Team: Professional charging network operators with experience in infrastructure and hospitality

#### 7. FAQ (`faq.html`)
**Purpose**: Address common questions

**Key Topics**:
- What is Altara Energy?
- What is Pathfinder Rewards and how does it work?
- Where can I use my Pathfinder Rewards?
- What vehicles can charge here?
- How do I pay?
- What amenities are available?
- Do you partner with businesses or property owners?
- Where are you expanding next?

### Supporting Pages

#### Legal/Compliance
- Privacy Policy (`privacy.html`)
- Terms of Service (`terms.html`)
- Accessibility Statement (`accessibility.html`)

#### Utility
- Contact (`contact.html`)
- Press/Media Kit (`press.html`)
- Careers (`careers.html`) - optional, or link to parent company if not maintaining separate careers page

---

## Content Guidelines

### Voice & Tone
- **Voice**: Direct, efficient, friendly but not overly casual
- **Tone**: Confident, helpful, no-nonsense
- **Style**: Short sentences, scannable content, clear CTAs

### Messaging Dos
✅ "Fast, reliable charging for your daily drive"  
✅ "Convenient locations where you need them"  
✅ "Part of the Pathfinder Rewards network"  
✅ "City charging designed for daily drivers"  
✅ "Simple, transparent pricing"  
✅ "Flexible partnerships with local businesses"  
✅ Use specific city names (San Francisco, Los Angeles, etc.) rather than "urban areas"  

### Messaging Don'ts
❌ No "journey" or "adventure" language (keep focused on daily convenience)  
❌ No premium/luxury positioning  
❌ No specific mentions of other charging brands unless in Pathfinder Network context  
❌ No overpromising on hospitality (it's site-dependent, not standardized)  

---

## Design Specifications

### Layout Principles
- **Clean, spacious layouts**: Generous white space
- **Card-based design**: Modular, scannable content blocks
- **Strong CTAs**: High-contrast buttons, clear hierarchy
- **Mobile-first**: Optimize for phone users first

### Component Patterns

#### Logo Usage
**Logo Files** (reference Altara Brand Guidelines v2.0 - Urban Current Edition):
- `altara-logo-standard-v2.svg` - Full color with gradient orbit (primary use)
- `altara-logo-monochrome-white.svg` - All white for dark backgrounds
- `altara-logo-monochrome-teal.svg` - Current Teal single color
- `altara-logo-small-v2.svg` - Optimized for small sizes/favicons
- `altara-logo-horizontal-v2.svg` - Icon + "Altara Energy" wordmark for headers

**Logo Specifications**:
- Circular orbital ring with gradient stroke (Ember Orange → Current Teal → Ember Orange)
- "A" symbol at center in Current Teal (#0891B2)
- Minimum sizes: 32px for icon, 120px for horizontal lockup
- Clear space: Minimum radius of logo around all sides
- Do NOT: Rotate, stretch, recolor, add effects, use on busy backgrounds

#### Buttons
- **Primary**: Current Teal background (#0891B2), white text
- **Secondary**: White background, Current Teal border and text
- **Accent**: Ember Orange background (#F97316), white text (use sparingly for CTAs)
- **Text Size**: 16px minimum
- **Padding**: Generous (16px vertical, 32px horizontal)
- **Border Radius**: 6-8px for modern feel
- **Text Size**: 16px minimum
- **Padding**: Generous (16px vertical, 32px horizontal)
- **Border Radius**: 6-8px for modern feel

#### Cards
- **Border**: Subtle shadow or light border
- **Padding**: 24px
- **Images**: If used, top-aligned or left-aligned
- **Consistent height**: In multi-column layouts

#### Typography
- **Headings**: Bold, clear hierarchy (H1: 48-56px, H2: 36-40px, H3: 24-28px)
- **Body**: 16-18px, 1.5-1.6 line height
- **Links**: Blue, underline on hover
- **Lists**: Generous spacing between items

### Navigation
- **Desktop**: Horizontal nav bar, sticky on scroll
- **Mobile**: Hamburger menu
- **Items**: Home | Locations | Membership | Fleet | Partners | About

### Footer
- **Columns** (4 on desktop, stacked on mobile):
  1. About Altara (short description + logo)
  2. Quick Links (Locations, Membership, FAQ)
  3. Company (About, Careers, Press, Contact)
  4. Legal (Privacy, Terms, Accessibility)
- **Bottom Bar**: Copyright, "Pathfinder Network Member" badge/link (optional), social icons (@altaraev on all platforms)
- **Social handles**: @altaraev (Twitter/X, Instagram, LinkedIn)

---

## Content Requirements (Placeholders)

Since Altara doesn't exist yet, use appropriate placeholder content:

### Station Details
- "Coming soon to [City Name]"
- Charger specs: "10+ DC fast chargers, 150-350kW"
- Amenities: "Clean restrooms, comfortable waiting areas, and site-specific amenities—shaded seating, picnic areas, dog parks, and more depending on location"

### Pricing
- Use example rates (clearly marked as examples)
- "Pricing varies by market and will be announced before launch"

### Images
- Use royalty-free stock images of:
  - EV charging in cities
  - Modern convenience stores
  - City streetscapes
  - People charging EVs in everyday settings
- Avoid scenic/nature imagery (keep focus on city convenience)
- Keep imagery clean, modern, showing city environments

### Stats/Claims
Only use claims that Altara can back up independently:
- ✅ "Professional network operations center"
- ✅ "Real-time monitoring and support"
- ✅ "Part of the Pathfinder Rewards network"
- ❌ Don't claim specific station counts, markets, or launch dates unless confirmed
- ❌ Don't reference other brands or their operational track records

---

## Operational Flexibility & Business Model

### Why Altara Exists
Altara is designed for maximum operational flexibility. Unlike premium charging brands with strict experience standards, Altara can adapt to various partnership models and site configurations.

### Partnership Models Altara Can Support:

**1. Site Host Agreements**
- Partner owns/leases property
- Altara installs and operates charging equipment
- Revenue share or monthly site host fee (e.g., $200/stall)
- Partner provides or hosts amenities
- Example: Retail plaza, grocery store, hotel parking lot

**2. White-Label Operations**
- Altara operates charging under partner's brand
- Partner gets charging revenue and customer relationship
- Altara gets operations fee
- Example: Property management company wants branded charging

**3. Full Ownership**
- Altara owns/leases property
- Altara owns all equipment
- Altara controls all revenue
- Partner provides hospitality services (food/beverage, retail)
- Example: Standalone Altara location with Coz-E Corner lease

**4. B2B Partnerships**
- Fleet charging agreements
- Corporate partnerships (employee charging benefits)
- Utility demand response programs
- Example: Delivery company exclusive charging access during certain hours

### Why This Flexibility Matters:
- Can say "yes" to deals that don't fit premium brand standards
- Can enter markets faster with lower capital requirements
- Can partner with various property types and business models
- Can offer white-label to partners who want branded charging
- Traditional CPO model without brand promise constraints

### What Altara Can Do (That Premium Brands Can't):
- ✅ Operate without indoor lounges or standardized amenities
- ✅ Partner with existing retail/restaurants for hospitality
- ✅ White-label for site hosts who want their own branding
- ✅ Flexible site configurations based on host needs
- ✅ B2B exclusive access arrangements

---

## Pathfinder Network Integration

### What is Pathfinder Network?
Pathfinder Rewards is a multi-brand EV charging loyalty program. Think of it like airline alliances (Star Alliance, OneWorld) or credit card reward networks—multiple independent brands participate, and members can earn/redeem across all participating locations.

**For customers:**
- One loyalty account works at multiple charging networks
- Earn credits charging at any participating location
- Redeem credits at any participating location
- More locations = more value

**For Altara:**
- Instant loyalty program without building from scratch
- Access to existing member base
- Credibility through network participation
- Room to add more partners over time

### How to Present Pathfinder on Altara Site

**Primary positioning:**
- "Altara accepts Pathfinder Rewards"
- "Part of the Pathfinder Network"
- "Join Pathfinder Rewards for benefits at Altara and partner locations"

**On Membership page:**
- Explain Pathfinder tiers and benefits
- Show that it works at multiple networks (don't need to name specific partners)
- Emphasize convenience of one app/account across networks

**Visual treatment:**
- Pathfinder logo alongside Altara logo where appropriate
- "Pathfinder Accepted Here" badge on homepage
- Co-branded membership materials

### What NOT to do:
- ❌ Don't claim Altara created or owns Pathfinder
- ❌ Don't list all participating networks (leaves flexibility)
- ❌ Don't over-explain the network mechanics (keep it simple for customers)

### Future flexibility:
- Structure allows adding more brands to Pathfinder later
- Can bring in third-party CPOs if desired
- Can white-label Altara's operations under other brands within network

---

## SEO & Metadata

### Primary Keywords
- City EV charging / EV charging [city name]
- DC fast charging [city name]
- Electric vehicle charging stations
- EV charging network
- Fast charging near me
- Convenient EV charging

### Meta Descriptions (Page-Specific)
- **Homepage**: "Altara Energy delivers fast, reliable EV charging at convenient city locations. Part of the Pathfinder Rewards network. Join today."
- **Locations**: "Find Altara Energy charging stations in [cities]. High-power DC fast charging with convenient amenities."
- **Membership**: "Join Pathfinder Rewards for flat-rate pricing with no time-of-use surprises. Free membership works at Altara and partner networks."

### Schema.org Markup
- Organization schema
- LocalBusiness schema (for each station when live)
- FAQPage schema for FAQ page

---

## Technical Implementation Notes

### Jekyll Configuration (`_config.yml`)
```yaml
title: Altara Energy
description: Fast, reliable city EV charging. Part of the Pathfinder Network.
url: https://altaraenergy.com
baseurl: ""
theme: minima # or custom theme

# Build settings
markdown: kramdown
plugins:
  - jekyll-feed
  - jekyll-seo-tag
  - jekyll-sitemap

# SEO
twitter:
  username: altaraev
  card: summary_large_image

social:
  name: Altara Energy
  links:
    - https://twitter.com/altaraev
    - https://instagram.com/altaraev
    - https://linkedin.com/company/altaraev

# Collections (if needed for locations/posts)
collections:
  locations:
    output: true
    permalink: /locations/:path/
```

### Folder Structure
```
/
├── _config.yml
├── _includes/
│   ├── header.html
│   ├── footer.html
│   ├── nav.html
│   └── head.html
├── _layouts/
│   ├── default.html
│   ├── page.html
│   └── location.html
├── _sass/
│   ├── _base.scss
│   ├── _layout.scss
│   ├── _components.scss
│   └── _variables.scss
├── assets/
│   ├── css/
│   │   └── main.scss
│   ├── js/
│   │   └── main.js
│   └── images/
├── index.html
├── locations.html
├── membership.html
├── fleet.html
├── partners.html
├── about.html
├── faq.html
├── contact.html
├── privacy.html
├── terms.html
└── README.md
```

### Forms
- Use Formspree or similar for contact/partnership forms
- Email capture for location waitlist
- Fleet inquiry form

### Analytics
- Google Analytics 4 (when ready to deploy)
- Track: page views, CTA clicks, form submissions, outbound links

---

## Development Phases

### Phase 1: Core Structure (MVP)
- [ ] Set up Jekyll project structure
- [ ] Create base layouts and includes
- [ ] Build homepage
- [ ] Build core pages (About, Locations, Membership)
- [ ] Mobile responsive
- [ ] Basic styling

### Phase 2: Content & Polish
- [ ] Add remaining pages (Fleet, Partners, FAQ)
- [ ] Integrate placeholder images
- [ ] Add forms (contact, waitlist)
- [ ] Legal pages (Privacy, Terms)
- [ ] SEO optimization

### Phase 3: Refinement
- [ ] Performance optimization
- [ ] Accessibility audit
- [ ] Browser testing
- [ ] Content review
- [ ] Launch preparation

---

## Success Criteria

### User Experience
- ✅ Clear value proposition within 5 seconds of landing
- ✅ Easy to understand Pathfinder Network benefit
- ✅ Simple path to join Pathfinder Rewards
- ✅ Mobile-friendly (majority of EV drivers use phones)

### Technical
- ✅ Loads in <2 seconds on 4G
- ✅ Passes Lighthouse audit (90+ scores)
- ✅ Accessible (WCAG AA)
- ✅ Works in all modern browsers

### Brand
- ✅ Clear standalone identity
- ✅ City convenience positioning is obvious
- ✅ Pathfinder Network membership is explained
- ✅ Professional, credible, trustworthy
- ✅ Balances efficiency with approachability
- ✅ Flexible partnership model is evident

---

## Brand Positioning Clarity

**Critical**: Altara is a standalone brand. It does NOT reference other charging networks in customer-facing materials except through Pathfinder Network participation.

### What Altara IS:
- City convenience EV charging network
- Fast, reliable, accessible
- Flexible partnership model with site hosts
- Traditional CPO operations
- Pathfinder Network member

### What Altara is NOT:
- Premium/luxury charging experience
- Hospitality-first (it's efficiency-first)
- Destination charging (it's daily-use charging)
- Adventure/scenic route focused

### Key Differentiators:
- **10+ DC fast chargers** at every location (not 4-6 like some competitors)
- **Flexible partnerships** with retailers, property owners, businesses
- **Pathfinder Rewards** acceptance (multi-network loyalty)
- **Site-specific amenities** (not standardized, adapts to location)
- **City-focused** locations where daily drivers need them

**Language Note**: In customer-facing copy, avoid "urban areas"—use specific city names, "cities," "convenient locations," or "where you need them" instead. "Urban" can be used internally for strategic discussions.

---

## Reference Materials

### Inspiration Sites (for urban convenience positioning)
- Wawa (convenience + fuel)
- Circle K / 7-Eleven (urban convenience)
- Pilot Flying J (modern, clean service stations)
- Sheetz (fresh, efficient, tech-forward convenience)

### What to AVOID
- Don't mimic Tesla Supercharger (too tech/minimal)
- Don't mimic Electrify America (too generic/soulless)
- Don't reference specific other charging brands unless in context of Pathfinder Network
- Avoid premium/luxury aesthetic (keep it accessible and efficient)

---

## Brand Assets Available

### Logo Files (from Altara Brand Guidelines v1.0)
You have the following logo assets available (v2.0 - Urban Current Edition):
- `altara-logo-standard-v2.svg` - Full color with gradient orbit (primary use on light backgrounds)
- `altara-logo-monochrome-white.svg` - All white for dark backgrounds
- `altara-logo-monochrome-teal.svg` - Current Teal single color for single-color reproduction
- `altara-logo-small-v2.svg` - Optimized for small sizes (favicons, under 64px)
- `altara-logo-horizontal-v2.svg` - Icon + "Altara Energy" wordmark (for website header)

**Logo Structure**:
- Circular orbital ring with gradient stroke (Ember Orange → Current Teal → Ember Orange)
- "A" symbol at center in Current Teal (#0891B2)
- "Altara" wordmark in Current Teal, semi-bold weight (Outfit font)
- "Energy" wordmark in Current Teal, regular weight (Outfit font)

### Color Values (Urban Current v2.0)
```css
:root {
    --current-teal: #0891B2;    /* Primary - Modern teal */
    --ember-orange: #F97316;    /* Accent - Energetic orange */
    --deep-teal: #0E7490;       /* Supporting - Darker teal */
    --bright-orange: #FB923C;   /* Supporting - Lighter orange */
    --concrete: #9CA3AF;        /* Neutral - Light gray */
    --slate: #334155;           /* Dark - Body text */
    --white: #FFFFFF;           /* White - Backgrounds */
}
```

### Typography
- **Primary Font**: Outfit (Google Fonts)
  - `@import url('https://fonts.googleapis.com/css2?family=Outfit:wght@400;500;600&display=swap');`
- **Font Stack**: `'Outfit', -apple-system, BlinkMacSystemFont, 'Segoe UI', system-ui, sans-serif`
- **Headings**: Font weight 600 (semi-bold)
- **Body**: Font weight 400 (regular)
- **Labels/UI**: Font weight 500 (medium)

### Gradient Definitions
```css
/* Logo orbital gradient */
linear-gradient(135deg, #F97316 0%, #0891B2 50%, #F97316 100%)

/* Hero background gradient */
linear-gradient(135deg, #0891B2 0%, #0E7490 100%)
```

---

## Contact for Questions

During development, if clarification needed on:
- **Brand positioning**: Altara is standalone city charging network, not connected to other brands except via Pathfinder Network
- **Pricing structure**: Use Pathfinder Rewards tiers (credits back model, not rate discounts)
- **Partnership model**: Flexible site host agreements, B2B partnerships, white-label potential
- **Operational details**: Professional NOC, real-time monitoring
- **Pathfinder Network**: Multi-brand loyalty program, Altara is a participating network

---

## Final Notes

**This is a CONCEPT site for a brand that hasn't launched yet.** The goal is to:
1. Visualize Altara as a standalone city charging brand
2. Test positioning and messaging
3. Demonstrate Pathfinder Network integration
4. Have a placeholder ready when Altara launches

**Existing Site**: There is currently an altaraenergy.com site that was adapted from another template. This project is to create a properly positioned site that reflects Altara's standalone identity, operational flexibility, and Pathfinder Network membership.

**Placeholder approach**: Use "Coming Soon" and "Join Waitlist" language rather than pretending stations exist. Be transparent this is a future network.

**Behind the scenes**: While Altara is operated by Rangeway Energy (sharing NOC, systems, and operational standards), this is NOT customer-facing information. Altara stands as an independent brand. The only visible connection to other brands is through Pathfinder Network participation.

---

**Ready to build? Give this brief to Claude Code and let's see what Altara Energy looks like.**
