# DESIGN.md — Marketing Portfolio Lab

> Version: 1.0 · 2026-11-09 · Educational demonstration only

## 1. Project intent
Create three connected static HTML pages from one candidate profile: general portfolio (`/`), fictional employer-specific portfolio (`/company-a/`), and acquisition campaign (`/campaign/`). Demonstrate that brand analysis is more than swapping a color palette: reframe the message, audience, hierarchy, CTA, and supporting evidence.

## 2. Brand system
- **Candidate / base:** rational, editorial, approachable, data-informed. Dark forest `#17241e`, emerald `#1d5547`, warm white `#f8f8f4`, muted `#627068`.
- **Atelier A / fictional employer:** understated lifestyle commerce, slower cadence, warm neutrals, considered curation. Deep sage `#2c372c`, moss `#5a684c`, cream `#f5f0e6`.
- **Atelier A / fictional campaign:** more emotional, sensory, aspirational, still clear about visitor action. Pine `#28382e`, soft ivory `#f8f4ec`, sage `#536b53`.
- These are **original fictional brand tokens**; not extracted from a real company's design system. Avoid official logos/trademarks or real claims.

## 3. Typography
- Korean body: Pretendard / Noto Sans KR / system sans fallback.
- English + UI: Manrope (Google Fonts) / system sans.
- Editorial hero on employer and campaign pages: Georgia.
- Strong hierarchy: H1 52–93px responsive; H2 28–65px; eyebrow 11px uppercase; body 15–18px.
- Korean copy should be short, natural, readable, and not sound like a design template.

## 4. Layout
- Shared max content width 1160px, 28px gutters desktop, 18px mobile.
- Base home: asymmetric split hero and 2-column project cards, evidence matrix.
- Employer: editorial hero with arch image, skills-to-JD traceability, proof cards.
- Campaign: split full-bleed editorial hero, campaign benefits, CTA, copy experiment.
- Mobile viewport: all dense grids become one column; nav remains visible and wraps.

## 5. Components
- Sticky header, small wordmark, text navigation, high-contrast primary button.
- Eyebrow, pill, metric/evidence card, editorial visual block, call-to-action section.
- Button min-height 48px; visible focus outlines. Avoid decorative controls that look functional.
- Contrast and responsive navigation must remain legible.
- Respect `prefers-reduced-motion`.

## 6. Marketing hypothesis and measurement
Scenario: a fictional lifestyle-commerce newcomer welcome campaign.
- Audience: first-time visitors, aged roughly 20–30 (assumption).
- Purpose: understand whether visitors want to explore new-member benefits.
- Primary CTA: `#welcome` and educational signup-preview button.
- Hypothesis A: emotional brand-discovery copy might encourage exploration.
- Hypothesis B: clearer new-visitor copy might lead to more benefit checks.
- Demo-only event examples: `landing_view`, `copy_variant_selected`, `campaign_cta_click`.
- **Do not claim real conversion rates, actual member benefits or tracked users.** Event names appear only in local interface. No analytics network calls.

## 7. Content integrity
Kim Harin is fictional. Atelier A and its JD are fictional. Data projects are educational mockups and not shipped operational analytics tools. Employment claims, job-fit scores, testimonials, revenue increases and simulated dashboard metrics are forbidden unless clearly marked fictional.

## 8. Suggested Google Stitch workflow
1. Supply a screenshot or URL of the current page together with the brand description and sections above.
2. Ask Stitch for a responsive editorial design under these exact colors and typography rules.
3. Compare two hero variants and choose one with clear CTA hierarchy.
4. Export/record resulting design rationale and update this `DESIGN.md`.
5. Implement chosen designs in Codex; verify actual HTML/CSS in Chrome and Safari at 375px, 768px and 1440px.
6. Preserve campaign events and disclosed demo-only behavior.

## 9. Acceptance checklist
- Routes `/`, `/company-a/`, `/campaign/` load and cross-link.
- No false claims or fake contact details presented as real.
- A/B copy controls update hero, selection state and event preview.
- CTA demo never claims account registration or sends data.
- Mobile menu accessible with keyboard; images have relevant alternative text.
- GitHub PR and Vercel preview built before a production merge.
