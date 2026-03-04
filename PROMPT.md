# LFG Navbar — Integration Prompt

Copy and paste the prompt below into any Claude instance to add the LFG navbar to a website.

---

## Prompt

```
Add the Looking for Growth (LFG) navigation bar to the top of this page. Here are the exact specifications:

**Structure:**
- A sticky `<nav>` bar at the very top of the page (position: sticky, top: 0, z-index: 9999)
- Left side: "LFG" logo text (bold, 24px, links to https://lookingforgrowth.uk)
- Right side: horizontal list of navigation links, ending with a "Donate" button
- On mobile (≤768px): links collapse behind a hamburger menu

**Navigation links (in this exact order):**
1. About us → https://lookingforgrowth.uk/about-us
2. Our campaigns → https://lookingforgrowth.uk/campaigns
3. Get involved → https://lookingforgrowth.uk/get-involved
4. Dashboards → https://dashboards.lookingforgrowth.uk/
5. Events → https://lookingforgrowth.uk/events
6. Merch → https://merch.lookingforgrowth.uk/
7. Donate → https://lookingforgrowth.uk/donate (styled as a pill button)

**Visual design:**
- Background colour: #8FBCAB (sage/seafoam green)
- Bottom corners rounded: border-radius 0 0 16px 16px (top is flush with page edge)
- Height: 56px on desktop
- Font: Inter (import from Google Fonts), fallback to system sans-serif
- Text colour: #1a1a1a (near-black)
- Link font size: 15px, font-weight: 450
- Links have 28px gap between them
- Padding: 0 32px
- Hover state: links fade to 70% opacity

**Donate button:**
- Background: #D4652C (burnt orange)
- Text: #1a1a1a, font-weight: 600
- Padding: 8px 20px
- Border-radius: 24px (full pill shape)
- Hover: darkens to #c05a26

**Mobile (≤768px):**
- Hamburger button (3 lines) replaces the link list
- Tapping hamburger toggles a vertical dropdown of all links
- Hamburger animates to an X when open
- Links separated by subtle 1px borders (rgba(0,0,0,0.08))
- Donate button remains styled as a pill

**Important notes:**
- All CSS classes are prefixed with `lfg-navbar-` to avoid conflicts with existing styles
- The navbar should be the very first element inside <body>
- Do NOT modify any existing page styles — the navbar is self-contained
- If the page already has a navbar/header, replace it with this one
```

---

## Quick Copy — Raw HTML + CSS

If you just need the code to paste directly, grab everything between the `===== LFG NAVBAR - START =====` and `===== LFG NAVBAR - END =====` comments in `index.html`, plus the matching CSS block.
