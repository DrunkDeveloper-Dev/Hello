# BrandName Robotics Website - Design Guidelines

## Design Approach
**Reference-Based Approach**: Drawing inspiration from premium tech brands (Linear, Apple, Stripe) combined with Afrofuturist aesthetics for a warm, credible robotics experience.

---

## Core Design Elements

### A. Color Palette

**Dark Mode (Primary)**
- Background Deep: `26 73% 13%` (deep chocolate #2B1A10)
- Background Elevated: `26 62% 17%` (card surface #3E2416)
- Accent Copper: `25 75% 47%` (#D2691E)
- Accent Bronze: `28 54% 46%` (#B87333)
- Text Primary: `37 57% 92%` (off-white #F5EDE0)
- Border Soft: `37 57% 92%` at 12% opacity
- Glow Effect: `25 75% 47%` at 35% opacity

### B. Typography

**Font Families**
- Display/Headers: Oxanium (futuristic, rounded) via Google Fonts
- Body/UI: Inter via Google Fonts
- Code: JetBrains Mono via Google Fonts

**Type Scale**
- H1: 56-64px (3.5-4rem)
- H2: 36-44px (2.25-2.75rem)
- H3: 24-28px (1.5-1.75rem)
- Body: 16-18px (1-1.125rem)
- Caption: 13-14px (0.8125-0.875rem)

### C. Layout System

**Spacing Primitives**: Use Tailwind units of 2, 4, 8, 12, 16, 20, 24, 32
- Micro spacing: p-2, gap-4
- Component spacing: p-8, py-12
- Section spacing: py-20, py-24, py-32

**Container Strategy**
- Full-width sections with inner max-w-7xl
- Content sections: max-w-6xl
- Cards: rounded-2xl with subtle border

### D. Component Library

**Navigation**
- Translucent brown glass effect (backdrop-blur)
- Sticky positioning
- Copper underline on hover (2px, transition 150ms)

**Cards**
- Rounded-2xl corners
- Soft shadow with glow
- 1px inner border using --line-soft
- Hover: 2-4px lift + copper glow shadow

**Buttons**
- Pill shape (fully rounded)
- Copper/bronze fill for primary
- Medium height (h-11 to h-12)
- Visible focus ring for accessibility
- Glass effect with blur for outline variants on images

**Code Blocks**
- Monospace font
- Faint copper border
- Syntax highlighting with warm tones
- Read-only display

**Badges**
- Small pill shape
- Bronze border for "New", "Research", "Beta"
- Subtle background tint

### E. Animations

**Micro-interactions** (150-250ms ease-in-out)
- Parallax hero glow effect
- Scroll-reveal fade-up with 60ms stagger
- Card hover: 2-4px lift + glow shadow
- Video thumbnail hover: autoplay preview

**Accessibility**
- Respect prefers-reduced-motion
- All transitions optional for reduced motion users

---

## Section-Specific Guidelines

### Hero Section
- **Layout**: Full viewport height with cinematic visual
- **Visual**: Large 3D-styled brown-metallic humanoid robot with warm rim lighting and subtle particle glow
- **Typography**: Bold H1 "Soul Meets Circuit" with large display font
- **CTAs**: Two buttons - Primary "See Our Robots" (copper fill) + Secondary "Follow on X" (glass outline)
- **Effect**: Subtle parallax glow on scroll

### About/Mission
- **Layout**: 2-column split (copy left, visual/stats right)
- **Content**: Three pillars displayed as cards or list items with icons
- **Style**: Clean, minimal with generous spacing

### Platforms
- **Layout**: 3-column grid (lg), 1-column mobile
- **Cards**: Each platform (Humanoid, Manipulator, Mobile Base) as elevated card
- **Content**: Brief specs list + "View Details" link
- **Hover**: Card lift with glow

### Core Technology
- **Layout**: Section header + 6 subsections in 2-3 column grid
- **Diagram**: Simple flow diagram (Sensors → Perception → World Model → Planner → Controller → Actuators) using SVG or styled divs
- **Cards**: Each tech area (Perception, Control, Brains, Sensors, Edge Compute, Safety) as small card

### Demos & Showcases
- **Layout**: Masonry or uniform grid of video thumbnails
- **Interaction**: Hover autoplay preview
- **Content**: Title, caption, "Watch Full Demo" overlay
- **Style**: Rounded thumbnails with copper border on hover

### Applications
- **Layout**: 4-tile grid (2x2 desktop, 1 column mobile)
- **Content**: Pain-point headline, solution, outcome metrics (with accent color)
- **Style**: Large tiles with icon or visual, hover glow

### R&D/Publications
- **Layout**: List view with paper titles, venue badges, year
- **Elements**: Benchmark badges (small pills), dataset links
- **CTA**: Prominent "Read our whitepaper" button

### Developers (SDK & API)
- **Layout**: Tabbed interface (Quickstart, ROS, Python, Simulation, Web Console)
- **Content**: Code snippet blocks with syntax highlighting
- **Style**: Dark code blocks with copper accent, "Open Docs" links

### Community
- **Layout**: Single prominent line/card
- **Content**: "Follow updates and drops on X → x.com/YourHandle"
- **Style**: Copper link with icon, hover glow

### News/Blog
- **Layout**: 3-card grid of latest posts
- **Content**: Title, date, excerpt
- **CTA**: "All posts" link

### Careers
- **Layout**: Role cards in grid
- **Content**: Role titles (Robotics Software, Controls, etc.)
- **CTA**: "Work with us" / "Partner inquiry" buttons

### Footer
- **Layout**: Multi-column (Contact, Quick Links, Legal)
- **Elements**: Email form, HQ city, social links
- **Tagline**: "Born from code. Built with soul."

---

## Images

**Hero Image**: Large, cinematic 3D render of brown-metallic humanoid robot or robotic arm with warm rim lighting (orange/copper), subtle particle effects, dark gradient background. Position: centered, fills 60-80% of hero viewport.

**Platform Cards**: Smaller product shots of each robot platform (Humanoid, Manipulator Arm, Mobile Base) from dynamic angles showing brown-metallic finish.

**Application Tiles**: Contextual imagery showing robots in logistics, healthcare, hospitality, creative settings - warm color grading.

**Team/Lab Photos** (if needed): Authentic workspace shots with warm color correction to match brown aesthetic.

---

## Accessibility & Performance

- Contrast ratios ≥ 4.5:1 for all text
- Focus states visible on all interactive elements
- Lazy-load images with srcset for responsive delivery
- WebM/H.264 fallbacks for video
- Reduced motion support
- SEO: meta tags, Open Graph with brown gradient + copper logo
- Privacy-friendly analytics with toggle