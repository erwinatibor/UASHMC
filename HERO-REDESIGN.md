# UASHMC Hero Section Redesign Master Prompt

## ROLE

You are a senior UI/UX designer, frontend developer, motion designer, and conversion-focused web designer.

You are working on the UASHMC website:

https://uashmc.vercel.app/

Your task is to redesign and enhance **ONLY the HERO SECTION** of the existing website.

Do not redesign the entire website.

The goal is to make the hero feel like a modern, premium, trustworthy hospital website while maintaining the existing UASHMC identity.

---

# PRIMARY DESIGN DIRECTION

Create a visual experience inspired by:

* Premium modern healthcare websites
* Clean hospital interfaces
* Apple-level spacing and smoothness
* Professional medical branding
* Trustworthy and compassionate visual language
* Modern SaaS-style UI polish, but adapted for healthcare

The design should communicate:

**Trust + Care + Professionalism + Modern Technology**

Avoid making it look like:

* A gaming website
* A futuristic AI website
* A cryptocurrency website
* An overly animated portfolio
* A generic template

The result should look like a professionally designed hospital website.

---

# IMPORTANT FIRST STEP

Before modifying anything:

1. Inspect the existing project structure.
2. Identify the framework being used.
3. Identify the current hero component.
4. Identify existing global styles.
5. Identify the existing color palette.
6. Identify existing fonts.
7. Identify available image assets.
8. Identify whether animations are already implemented.
9. Identify the current responsive behavior.
10. Do not immediately rewrite the project.

Understand the existing code first.

Preserve the existing architecture whenever practical.

---

# HERO STRUCTURE

Redesign the hero into the following visual hierarchy.

## 1. HEADER / NAVIGATION

Keep the existing navigation items if they are already present.

The navigation should feel clean and premium.

Recommended structure:

Logo | Home | About Us | Our Services | Doctors | Facilities | News & Updates | Contact | Book an Appointment

### Navigation behavior

At the top:

* Transparent or semi-transparent background
* Clean spacing
* Strong readability

When scrolling:

* Slight background blur
* White or very light background
* Subtle shadow
* Smooth transition

Use:

```text
backdrop-filter: blur(...)
transition: 300ms ease
```

Do not create an oversized navbar.

---

# 2. HERO BACKGROUND

Use a high-quality UASHMC/hospital exterior image if an existing suitable asset is available.

If an appropriate image already exists in the project, reuse it.

Do NOT invent a fake hospital image if a real UASHMC image is already available.

The image should occupy approximately:

Desktop:
50–60% of the hero visual area

The image can extend toward the right edge of the screen.

Add a subtle gradient overlay where necessary to maintain text readability.

---

# 3. HERO LEFT CONTENT

Create a strong text hierarchy.

Small eyebrow text:

"Compassionate Care. Advanced Medicine."

Main heading:

"Your Health,
Our Priority."

The heading should be large, confident, and highly readable.

Recommended desktop size:

```text
64px–88px
```

Adjust responsively depending on the existing design.

Do not use excessively thin typography.

Use strong weight and excellent spacing.

Highlight the final punctuation or selected word with the UASHMC green accent if it fits the visual design.

---

# 4. SUPPORTING DESCRIPTION

Use a short, professional healthcare statement:

"Delivering quality, patient-centered healthcare with expertise, innovation, and compassion."

Keep the paragraph width controlled.

Do not make the text too wide.

Recommended:

```text
max-width: 520px
```

---

# 5. PRIMARY CTA

Create a prominent green button:

"Book an Appointment"

Include a small calendar icon.

Button characteristics:

* Rounded pill or moderately rounded corners
* UASHMC green
* White text
* Strong contrast
* Smooth hover animation

Hover:

```text
translateY(-2px)
slightly stronger shadow
icon moves slightly right
```

Animation duration:

```text
200ms–300ms
```

---

# 6. SECONDARY CTA

Add:

"Watch Our Video"

Use a play-circle icon.

Style it as a secondary outlined button.

It should visually support the primary CTA without competing with it.

---

# 7. TRUST / SERVICE CARDS

At the bottom portion of the hero, add a clean floating information card.

Create 3 small feature items:

### Expert Doctors

"Highly skilled and compassionate team"

### Advanced Facilities

"Modern technology for better care"

### Patient-Centered

"Your health and comfort come first"

Use simple line icons.

Avoid overly complicated illustrations.

The card should have:

* White/semi-transparent background
* Subtle blur
* Soft shadow
* Rounded corners
* Clean dividers
* Good spacing

On mobile, stack the cards vertically or convert them into a horizontal scroll/card layout.

---

# 8. TRUST BADGE

Add a small floating trust badge toward the lower-right portion of the hero:

"Trusted Healthcare"

Supporting text:

"Committed to excellence in every patient journey."

Use a shield/check icon.

This should feel like a subtle floating UI element.

Do not make it too large.

---

# 9. HERO VISUAL DETAILS

Add very subtle decorative medical elements.

Possible elements:

* Thin medical cross outlines
* Very subtle healthcare line patterns
* Soft gradient blobs
* Small floating circles
* Light abstract curves

These elements should have very low visual weight.

Opacity should generally remain around:

```text
0.05–0.15
```

They should support the design, not distract from the hospital image.

---

# COLOR DIRECTION

Use the existing UASHMC branding where possible.

Preferred palette:

Primary Green:

```text
#147A43
```

Dark Navy:

```text
#102A56
```

White:

```text
#FFFFFF
```

Soft Background:

```text
#F4F8F6
```

Light Blue:

```text
#EAF3FA
```

Do not blindly replace the existing brand colors.

First inspect the existing website and use the current UASHMC palette if it is already defined.

Maintain strong WCAG-friendly contrast.

---

# ANIMATION SYSTEM

The animation should feel premium and subtle.

Do NOT animate everything.

## Initial page load

Animate the hero in this order:

1. Navbar
2. Eyebrow text
3. Main heading
4. Description
5. CTA buttons
6. Feature card
7. Hero image
8. Floating trust badge

Recommended stagger:

```text
0ms
100ms
180ms
260ms
340ms
450ms
550ms
650ms
```

Use opacity + small translateY.

Example:

```text
opacity: 0 → 1
transform: translateY(20px) → translateY(0)
```

---

# HERO IMAGE ANIMATION

Use a very subtle slow zoom.

Example:

```text
scale(1) → scale(1.04)
```

Duration:

```text
10–15 seconds
```

Use an ease-in-out animation.

It should be barely noticeable.

Do NOT use aggressive zooming.

---

# SCROLL ANIMATIONS

When the hero enters the viewport:

* Text fades upward
* Feature cards stagger
* Image gently reveals

Keep movement between:

```text
10px–30px
```

Avoid large movements.

---

# HOVER EFFECTS

Buttons:

* Slight upward movement
* Shadow increase
* Arrow/icon movement

Feature cards:

* Slight elevation
* Slight shadow increase
* Icon scale around 1.05

Navigation links:

* Smooth underline or opacity transition

Avoid:

* Excessive scaling
* Rotation
* Bouncing
* Flashing
* Glitch effects

---

# SCROLL INDICATOR

If appropriate, add a subtle scroll indicator near the bottom of the hero.

Example:

```text
Scroll to explore
↓
```

Animate it very slowly.

Only include this if it does not clutter the hero.

---

# RESPONSIVE DESIGN

The hero MUST be fully responsive.

## Desktop

Use a two-column composition:

```text
LEFT
Text + CTA + supporting content

RIGHT
Hospital image
```

## Tablet

Reduce:

* Heading size
* Navigation spacing
* Image height
* Feature card size

## Mobile

Reorganize into:

```text
Navbar

Hospital Image

Eyebrow

Heading

Description

CTA

Secondary CTA

Trust / service cards
```

Do not allow:

* Horizontal overflow
* Text clipping
* Buttons extending outside the viewport
* Broken images
* Overlapping cards
* Tiny unreadable text

The mobile hero should feel intentionally designed, not simply a desktop layout squeezed into a phone.

---

# ACCESSIBILITY

Implement:

* Semantic HTML
* Proper heading hierarchy
* Accessible buttons
* Alt text for images
* Keyboard navigation
* Visible focus states
* Sufficient contrast
* Reduced-motion support

Respect:

```css
@media (prefers-reduced-motion: reduce)
```

When reduced motion is enabled, minimize or disable non-essential animations.

---

# PERFORMANCE

The hero must remain fast.

Avoid:

* Heavy JavaScript animation libraries unless already installed
* Huge video backgrounds
* Excessive blur effects
* Large unoptimized images
* Continuous expensive animations
* Dozens of DOM elements solely for decoration

Prefer CSS transitions and lightweight animation.

If Framer Motion is already installed, it may be used appropriately.

If it is not installed, do not install a large dependency unless there is a strong reason.

---

# CODE QUALITY

Follow the existing project's coding conventions.

Before editing:

* Inspect components
* Inspect styles
* Inspect assets
* Inspect package.json
* Inspect routing
* Inspect responsive breakpoints

Then make the smallest clean set of changes necessary.

Do not duplicate existing components unnecessarily.

Do not create unused components.

Do not leave debugging code.

Do not leave console errors.

---

# CONTENT RULES

Do not invent:

* Doctors
* Medical services
* Hospital statistics
* Certifications
* Awards
* Medical claims
* Patient numbers
* Accreditations

If existing UASHMC content contains these details, preserve them.

If information is unavailable, use neutral UI copy rather than fabricating facts.

---

# IMPORTANT VISUAL REQUIREMENT

The final hero should have this approximate visual balance:

```text
┌─────────────────────────────────────────────────────────────┐
│ LOGO     NAVIGATION                     BOOK APPOINTMENT    │
│                                                             │
│                                                             │
│  Compassionate Care.              ┌──────────────────────┐  │
│  Advanced Medicine.               │                      │  │
│                                   │   UASHMC HOSPITAL    │  │
│  Your Health,                     │      IMAGE           │  │
│  Our Priority.                    │                      │  │
│                                   │                      │  │
│  Description                      └──────────────────────┘  │
│                                                             │
│  [Book Appointment] [Watch Video]                           │
│                                                             │
│  ┌─────────────────────────────────┐     ┌──────────────┐   │
│  │ Expert │ Facilities │ Patient   │     │ Trusted      │   │
│  │ Doctors│           │ Centered   │     │ Healthcare   │   │
│  └─────────────────────────────────┘     └──────────────┘   │
└─────────────────────────────────────────────────────────────┘
```

This is a visual direction, not a requirement to reproduce the exact layout.

---

# DESIGN PRINCIPLE

The hero should answer three questions immediately:

### WHO ARE YOU?

UASHMC

### WHAT DO YOU PROVIDE?

Quality, patient-centered healthcare.

### WHAT SHOULD I DO?

Book an Appointment.

The user should understand this within 3–5 seconds.

---

# DO NOT CHANGE

Unless absolutely necessary, do not modify:

* Other homepage sections
* Footer
* Services section
* Doctors section
* About section
* News section
* Existing routes
* Existing functionality

This task is specifically focused on the HERO SECTION.

---

# FINAL QA CHECKLIST

After implementation, verify:

[ ] Hero looks premium

[ ] Existing UASHMC branding is preserved

[ ] Hospital image looks professional

[ ] Main heading is immediately readable

[ ] CTA is visually obvious

[ ] Navigation is clean

[ ] Animations are smooth

[ ] Animations are subtle

[ ] No animation feels distracting

[ ] Desktop layout works

[ ] Tablet layout works

[ ] Mobile layout works

[ ] No horizontal scrolling

[ ] No text overflow

[ ] No broken assets

[ ] No console errors

[ ] No fabricated hospital information

[ ] Page remains performant

[ ] Reduced-motion accessibility works

---

# EXECUTION INSTRUCTION

Start by inspecting the existing UASHMC project.

Do not modify files yet.

First determine:

1. Framework
2. Hero component
3. Styling system
4. Existing assets
5. Existing animation system
6. Current responsive structure

Then implement the redesign.

After implementation, review the hero visually and technically.

Fix spacing, alignment, typography, responsiveness, animation timing, and visual hierarchy until the result looks production-ready.

Do not stop at "the code works."

The goal is:

**A polished, modern, premium UASHMC hospital hero section that looks professionally designed and feels smooth without being over-animated.**
