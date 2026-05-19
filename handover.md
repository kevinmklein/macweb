# Monroe Arts Council — Website Redesign Project
## Handover Document

**Organization:** Monroe Arts Council (MAC), Monroe, WA — Snohomish County
**Project:** Comprehensive redesign and relaunch of monroeartscouncil.org
**Platform:** SquareSpace (existing account, continuing)
**Prepared:** April 2026
**Status:** Phase 1 complete — board presentation ready, awaiting signoff

---

## 1. Project overview

The MAC website at monroeartscouncil.org is functional but overdue for a comprehensive redesign. The current site suffers from navigation clutter (Donate appears three times, Subscribe twice), pages with content 6–7 years out of date, no clear primary call to action, and a structure that doesn't reflect the organization's current programs or ambitions — including no mention of the Sky Valley Philharmonic.

The goal of this project is a clean, modern, brand-consistent website that serves the MAC's four distinct user audiences, drives community engagement and donor conversion, showcases the Wagner Performing Arts Center, and is maintainable by volunteers without developer support. The site will remain on SquareSpace.

---

## 2. Deliverables produced to date

All files are located in `/MAC/Website Redesign/` on the Desktop.

| File | Description |
|---|---|
| `mac_board_presentation.html` | Five-tab interactive board presentation covering site audit, personas, sitemap, design brief, and process roadmap |
| `mac_content_inventory.html` | Full page-by-page content inventory of the current site — 21 pages/nav items audited with keep / update / merge / deprecate / new status for each |
| `Monroe-Arts-Council-Logo-transparent.png` | Source logo file (black background stripped) — used as embedded asset in both HTML files |
| `handover.md` | This document |
| `project.md` | Additional background on the project and user |

The two HTML files are self-contained — the logo is embedded as base64 and they cross-link to each other. Both files must remain in the same folder to resolve the cross-link correctly.

---

## 3. Decisions made and rationale

### Navigation structure
The current site has 13+ navigation items at the top level with significant redundancy. The new structure consolidates to four top-level sections plus Home:

| New section | Replaces / consolidates |
|---|---|
| **Events & Programs** | Events, Projects (programs only) |
| **The Wagner** | Wagner History, Rent the WPAC, Wagner Accessibility Map, restoration content from Projects |
| **Get Involved** | Donate, Volunteer, Join Us — unified under one hub |
| **About MAC** | Mission, Board, Supporters, Contact, News & Updates |

**Donate** becomes a single persistent header button sitewide — not a nav item.
**Subscribe** moves to a persistent footer component and a post-event prompt — not a nav item.

### Content disposition
- **Keep (5 pages):** Events, Home, Contact, Board, Supporters
- **Update (5 pages):** Mission/What We Do, Projects & Programs, Rent the Wagner, Volunteer, Donate
- **Merge (4 pages/items):** Join Us → Get Involved; Wagner Accessibility Map → Rent the Wagner; Wagner History → The Wagner section; Subscribe → footer component
- **Deprecate (3 things):** MAC News blog (all posts 2018–19), `/sounds-of-the-world-2026` used as generic Donate link, all duplicate nav/footer CTA instances
- **New (4 pages):** Get Involved hub, The Wagner section hub, Restoration Progress page, News & Updates feed

### Platform
SquareSpace is confirmed as the continuing platform. Rationale: built-in permissioning, low maintenance overhead, no developer required, existing account. Custom CSS and code injection are available under the Pro plan for design customization. No bespoke code or third-party hosting is needed for Phase 1.

### Brand colors
Derived directly from the existing MAC logo:

| Swatch | Name | Hex |
|---|---|---|
| MAC Sage | Primary | `#84a14d` |
| Forest | Dark primary | `#5a7234` |
| Deep Green | Headers / footers | `#3d5023` |
| Terracotta | Accent / CTAs | `#b35a1a` |
| Dark Brown | Dark accent | `#7a3c0e` |
| Warm Cream | Page base | `#faf7f2` |

### Typography
Playfair Display (serif, for headings — conveys historic gravitas) paired with DM Sans (clean sans-serif, for body and UI). Both available free via Google Fonts and can be injected via SquareSpace's custom font upload on Pro.

---

## 4. User personas and golden paths

Four audiences were identified. The primary conversion goal is Community Member → Volunteer/Donor.

**Community Member** (largest group, top of funnel)
Motivation: "What's on this weekend?"
Golden path: Home → Events → Ticket/Info → Subscribe to newsletter

**Volunteer / Donor** (highest conversion value)
Motivation: "I love the Wagner — how do I help?"
Golden path: Home → Get Involved → Donate or Volunteer → Confirmation

**Theater Renter** (revenue-generating)
Motivation: "I need a 632-seat venue with full tech support."
Golden path: Home or search → Rent the Wagner → Specs + Gallery → Inquiry form

**Known Volunteer / Member** (Phase 2)
Motivation: "What's my next shift? Can I see my giving history?"
Golden path: Login → Dashboard → My assignments / giving history
*(This audience requires SquareSpace Member Areas or a tool like Givebutter — scoped for Phase 2.)*

---

## 5. Current site audit — key findings

The full page-by-page inventory is in `mac_content_inventory.html`. Summary of headline issues:

- "Donate" appears 3 times in navigation, pointing to 2 different URLs
- "Subscribe" appears twice as a standalone nav item
- "Join Us" and "Volunteer" are separate pages with heavily overlapping purposes
- "Contact" and "Contact Us" are redundant
- MAC News contains only posts from 2018–2019 — 6–7 years stale, actively damaging credibility with new visitors
- The Accessibility Map is buried as a top-level nav item
- No clear primary CTA exists anywhere on the site
- No mention of Sky Valley Philharmonic anywhere on the current site

The most urgent quick win, even before the redesign launches: unpublish the MAC News blog and consolidate the three Donate nav links to one. These two changes cost nothing and immediately reduce confusion.

---

## 6. Design assets needed

The following assets should be gathered or commissioned before the build phase begins. This list is also in Tab 4 of the board presentation.

**Photography (highest priority)**
- Professional interior shots of the Wagner stage, auditorium, and lobby — ideally post-renovation completion
- Exterior / façade shots of the Wagner building on Main Street
- Candid shots of audience members, performers, and volunteers in action
- Archival 1939 dedication photos (some already on the Wagner History page — confirm rights)
- Before/after renovation progress photos

**Identity**
- SVG version of the MAC logo (current PNG is usable but not print/injection-ready)
- Program logos from Monroe Community Band, Sky Performing Arts, and Sky Valley Philharmonic
- Consider a Wagner-specific wordmark or icon as a secondary identity element

**Video (optional but high-impact)**
- Short "about the restoration" clip — 60–90 seconds — for the Wagner section hero

**Board headshots**
- Updated photos for the Board of Directors page

---

## 7. Proposed 5-phase roadmap

| Phase | Description | Timeline | Owner |
|---|---|---|---|
| 1 | Audit & alignment — board signoff on sitemap, personas, deprecation list | Now | VP / Board |
| 2 | Design sprint — style tile, type system, color palette, homepage wireframe | Weeks 1–3 | Design partner |
| 3 | Content migration — rewrite keep/update pages, draft new sections in SquareSpace staging | Weeks 3–5 | MAC volunteer lead |
| 4 | Build & QA — apply design system, integrate newsletter CTA, accessibility and mobile testing | Weeks 5–7 | Design partner + volunteer |
| 5 | Launch + Phase 2 planning — go live, analytics setup, scope member portal | Week 8+ | VP |

Total estimated elapsed time to launch: ~8 weeks from board signoff.

---

## 8. Board asks — pending signoff

The following four items require board approval before the project can advance to Phase 2:

1. **Approve** the 4-section navigation structure and the deprecated content list
2. **Authorize** a design partner engagement for the design sprint (Phase 2)
3. **Confirm** SquareSpace as the continuing platform — no full rebuild required
4. **Identify** a content migration lead from current volunteers (Phase 3 owner)

---

## 9. Phase 2 scoping notes (for future reference)

The Known Volunteer / Member audience (Persona 4) requires functionality not available out of the box in SquareSpace's standard tier. Options to evaluate:

- **SquareSpace Member Areas** — native gating of content by membership tier; limited but low-friction
- **Givebutter** — donor management, volunteer coordination, and giving history; integrates via embed
- **Bloomerang or Little Green Light** — nonprofit CRM options if a more robust donor database is needed

This is explicitly scoped as Phase 2 and should not delay the Phase 1 launch.

---

## 10. Open questions and items to resolve

- [ ] Confirm whether the **Sounds of the World 2026** campaign (`/sounds-of-the-world-2026`) is still active or has ended — affects how the Donate page consolidation is handled
- [ ] Verify the **Paul G. Allen Foundation** logo on the Supporters page — the foundation wound down in 2024; confirm whether acknowledgment is still appropriate
- [ ] Confirm current status of **Community Keys** (2017 piano project) and **#ArtUpMonroe** (2017 scavenger hunt) — both listed on Projects as if ongoing; decide whether to archive or update
- [ ] Obtain **SVG version of the MAC logo** from original designer or recreate
- [ ] Schedule **post-renovation photography** session at the Wagner — timing dependent on renovation completion
- [ ] Identify and brief the **content migration volunteer lead** before Phase 3 begins
- [ ] Confirm **SquareSpace plan tier** — custom font injection requires Pro; verify current subscription level
- [ ] Update **restroom renovation notice** on Rent the Wagner page once construction is complete

---

*Document prepared in support of the MAC Website Redesign Project, April 2026.*
*For questions, contact the MAC VP or refer to the board presentation at `mac_board_presentation.html`.*
