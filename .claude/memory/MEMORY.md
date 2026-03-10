# DetectAIves Website — Project Memory

## Site Overview
Static HTML/CSS/vanilla-JS website for the DetectAIves AI literacy initiative at University of Maryland.
Rebranded from "A Eye / Eye AI" to "DetectAIves" in March 2026.

## File Structure (active pages)
- `index.html` — Home page
- `about.html` — About the initiative
- `projects.html` — Projects index (5 Spring 2025 cards + Summer 2026 placeholder)
- `report.html` — AI vs. Human research report (project detail, nav active: Projects)
- `extension.html` — Validate AI Chrome extension (project detail, nav active: Projects)
- `presentations.html` — TWO sections: Sprintern Project Presentations (5) + Workshop Lectures (6)
- `workshops.html` — Workshop history and upcoming
- `resources.html` — Educational resources hub (in footer, not primary nav)
- `scams.html` — AI scam awareness (resource detail, breadcrumb: Resources / AI Scam Awareness)
- `people.html` — Combined Team + Sprinterns (Faculty/Grad on Team section; UNDERGRADS ONLY in Sprinterns section)
- `contact.html` — Contact / Get Involved
- `style.css` — Expanded main stylesheet (~1300 lines)
- `nav.js` — Hamburger toggle + feather.replace() call
- `team.html` — Superseded by people.html (orphaned, nav updated to 7-item nav)
- `sprinterns.html` — Superseded by people.html (orphaned, nav updated)

## Nav Structure (7 items — FINAL)
Home | About | Projects | Presentations | Workshops | People | Contact
- Resources is in footer/linked but NOT a primary nav tab
- people.html replaces old team.html + sprinterns.html

## Key Design Decisions
- Color: --blue #4285f4, --blue-pale #f0f6ff
- Font: Inter (Google Fonts) + Georgia for logo
- Logo: `Detect<span class="logo-ai">AI</span>ves` — "AI" in blue
- Icons: Feather Icons CDN (https://unpkg.com/feather-icons) — `<i data-feather="name"></i>`, replaced via nav.js
- Nav: 7 items, hamburger on mobile (<1024px), horizontal on desktop
- Active nav: filled blue pill; non-active: text with hover
- Sticky header, shared footer on every page
- NO emojis, NO dash/pipe text separators

## CSS Architecture
style.css sections: Reset → Variables → Skip Link → Container → Header/Nav → Footer →
Sections → Page Hero → Buttons → Card Grid → Project/Person/Presentation/Workshop/Resource cards →
Info cards → Embeds → Two-column → Home Hero → Feature Strip → Upcoming Banner → Badge →
About → Contact → Instructions → Breadcrumb → Highlight Box → CTA Section → Feather Icon Sizing →
Section Divider → Responsive

## Content Notes
- Spring 2025 cohort produced FIVE projects (not two) — 2 with real content, 3 with placeholders
- Sprinterns section on people.html: FIVE undergrads only (no grad students there)
- Grad students appear in the Research Team section of people.html only
- Presentations page has two distinct sections:
  A. Sprintern Project Presentations (5 cards, one per project)
  B. Workshop Lectures and Instructional Sessions (6 placeholders across 3 weeks)
- June 2026 workshop cohort upcoming — placeholders throughout
- All placeholder person cards need real names/bios added
- All placeholder projects 3-5 need real titles/descriptions added

## Assets (at root)
- `firstExtension.png`, `validateAI.png`, `toggleFeatures.png` — extension screenshots
- `Images/UMD Logo.png` — UMD logo
- `Validate AI-Lexie.pptx.pdf` — presentation PDF

## User Preferences
- Projects and Presentations are SEPARATE tabs (critical)
- No rebuilding from scratch — refactor and expand
- Static HTML only, no frameworks
- Accessible: 17px base font, clear contrast, semantic HTML, skip links, ARIA labels
- Cohort-organized structure for scalability
- Clean academic aesthetic — no emojis, no decorative separators
