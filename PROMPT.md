# LFG Navbar — Integration Prompt

Copy and paste the prompt below into any Claude instance to add the LFG navbar to a website.

---

## Prompt

```
Add the Looking for Growth (LFG) navigation bar to the top of this page. Here are the exact specifications:

**Structure:**
- A sticky `<nav>` bar at the very top of the page (position: sticky, top: 0, z-index: 9999)
- No rounded corners — the bar is a solid rectangle, flush edge-to-edge
- Left side: "LFG" logo text (bold, 24px, links to https://lookingforgrowth.uk)
- Right side: horizontal list of navigation links, ending with a "Donate" pill button
- On mobile (≤768px): desktop links are hidden; a hamburger icon opens a slide-out panel

**Desktop navigation links (in this exact order):**
1. About us → https://lookingforgrowth.uk/about-us
2. Our campaigns → https://lookingforgrowth.uk/campaigns
3. Get involved → https://lookingforgrowth.uk/get-involved
4. Dashboards → https://dashboards.lookingforgrowth.uk/
5. Events → https://lookingforgrowth.uk/events
6. Merch → https://merch.lookingforgrowth.uk/
7. Donate → https://lookingforgrowth.uk/donate (styled as a pill button)

**Desktop visual design:**
- Background colour: #79CAC4 (teal green)
- No border-radius — completely rectangular, flush with page edges
- Height: 56px
- Font: Inter (import from Google Fonts), fallback to system sans-serif
- Text colour: #1a1a1a (near-black)
- Link font size: 15px, font-weight: 450
- Links have 28px gap between them
- Padding: 0 32px
- Hover state: links fade to 70% opacity

**Donate button (desktop):**
- Background: #D4652C (burnt orange)
- Text: #1a1a1a, font-weight: 600
- Padding: 8px 20px
- Border-radius: 24px (full pill shape)
- Hover: darkens to #c05a26

**Mobile (≤768px) — Slide-out panel:**
- Hamburger button: 3 horizontal lines (26px wide, 2.5px thick, 6px gap) in the navbar
- Tapping hamburger opens a slide-out panel from the LEFT side
- Panel width: 75% of screen (max 360px), full viewport height
- Panel background: white (#ffffff)
- A semi-transparent dark overlay (#000 at 30% opacity) covers the rest of the page
- X close button (×) in top-right corner of the panel (28px font size)
- Tapping the overlay also closes the panel
- Panel slides in/out with a 0.3s ease transition
- Body scroll is locked when panel is open

**Mobile panel links:**
- Stacked vertically with generous spacing (14px padding top/bottom each)
- Font size: 18px, font-weight: 600, colour: #1a1a1a
- NO borders between links — clean spacing only
- Links in panel: About us, Our campaigns, Get involved, Dashboards, Events

**Mobile panel footer (pinned to bottom of panel):**
- Two special links at the bottom: "donate →" and "buy our merch →"
- These are larger (22px), bold (700), lowercase
- Each has a 3px solid #D4652C (burnt orange) underline (border-bottom)
- The arrow (→) is appended via CSS ::after pseudo-element
- Links: donate → https://lookingforgrowth.uk/donate, buy our merch → https://merch.lookingforgrowth.uk/

**Important notes:**
- All CSS classes are prefixed with `lfg-navbar-` or `lfg-mobile-` to avoid conflicts
- The navbar should be the very first element inside <body>
- The mobile panel and overlay are separate elements after the <nav>
- Do NOT modify any existing page styles — the navbar is self-contained
- If the page already has a navbar/header, replace it with this one
- The mobile panel requires a small JS snippet (vanilla, no dependencies) for open/close
```

---

## Quick Copy — Raw HTML + CSS + JS

If you just need the code to paste directly, grab everything between the `===== LFG NAVBAR - START =====` and `===== LFG NAVBAR - END =====` comments in `index.html`, plus the matching CSS block.
