# BrandName - Afrofuturist Robotics Website

## Overview
BrandName is a premium robotics company website featuring an Afrofuturist brown/copper aesthetic. The site showcases emotionally aware AI robots with a warm, credible, and production-ready design.

**Theme**: Dark-first design with warm brown (#2B1A10 deep chocolate backgrounds), copper (#D2691E) accents, and bronze highlights. Professional, cinematic, and accessible.

## Recent Changes
- **2024**: Complete frontend implementation with all sections
- Design system configured with Oxanium display font, Inter body font, JetBrains Mono for code
- All 12 sections implemented: Hero, About, Platforms, Technology, Demos, Applications, Research, Developers, Community, News, Careers, Contact
- Smooth scroll navigation, parallax effects, hover animations (150-250ms transitions)
- Generated robot imagery for hero and platform cards
- SEO optimization with meta tags and Open Graph

## Project Architecture

### Frontend Stack
- **Framework**: React with TypeScript
- **Routing**: Wouter
- **Styling**: Tailwind CSS + Shadcn UI components
- **Fonts**: Oxanium (display), Inter (body), JetBrains Mono (code)
- **Animations**: Framer Motion patterns, CSS transitions
- **Forms**: React Hook Form + Zod validation
- **State**: TanStack Query for data fetching

### Design System
- **Primary Color**: Copper #D2691E (25 75% 47%)
- **Background**: Deep Chocolate #2B1A10 (26 73% 13%)
- **Card Background**: #3E2416 (26 62% 17%)
- **Text**: Off-white #F5EDE0 (37 57% 92%)
- **Border Radius**: 2xl (16px) for cards, pill for buttons
- **Shadows**: Copper glow effects (shadow-glow-sm/md/lg)
- **Motion**: Reduced motion support, 150-250ms transitions

### Page Sections
1. **Hero**: Cinematic robot visual, dual CTAs, parallax glow
2. **About**: Mission statement with 3 pillars (Human-Centered, Autonomy, Responsible AI)
3. **Platforms**: Humanoid, Manipulator Arm, Mobile Base cards
4. **Core Technology**: 6 tech areas + pipeline diagram
5. **Demos**: Video showcase grid (6 demos)
6. **Applications**: 4 industry use cases with metrics
7. **Research**: Publications, benchmarks, whitepaper CTA
8. **Developers**: Tabbed SDK documentation (Quickstart, ROS, Python, Simulation, Console)
9. **Community**: Prominent X (Twitter) follow link
10. **News**: 3 latest blog posts
11. **Careers**: 5 open roles + general application
12. **Contact**: Form + HQ location
13. **Footer**: Links, social, tagline "Born from code. Built with soul."

### Data Models
- **Contact Messages**: Name, email, company (optional), message
- Stored in-memory (MemStorage) for development

### Backend
- Express.js server
- In-memory storage for contact form submissions
- API endpoint: POST /api/contact

## User Preferences
- Dark mode is the default (Afrofuturist brown theme)
- Premium, credible aesthetic matching modern tech companies
- Accessibility: 4.5:1 contrast ratios, focus states, reduced motion support
- Performance: Lazy-loaded images, optimized assets

## Key Files
- `client/src/pages/Home.tsx` - Main landing page
- `client/src/components/` - All section components
- `client/src/index.css` - Color tokens and elevation utilities
- `tailwind.config.ts` - Design system configuration
- `design_guidelines.md` - Complete design specifications
- `shared/schema.ts` - TypeScript types and Zod schemas

## Development
- Run: `npm run dev` (starts both frontend and backend)
- Frontend: Vite dev server on port 5000
- Backend: Express server integrated with Vite
- All routes serve from same origin (no CORS needed)

## Next Steps
- Contact form API integration
- Optional: CMS for blog posts
- Optional: Video hosting integration for demo showcases
- Deployment to Replit
