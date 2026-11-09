# Marketing Data & AI Portfolio Lab — Preview

Educational demonstration: one fictional candidate, three connected learning deliverables.

## Pages

| Path | Objective |
|---|---|
| `/` | Personal marketing-data portfolio with transparent evidence |
| `/company-a/` | Tailored portfolio for fictional lifestyle-commerce employer **Atelier A** |
| `/campaign/` | Fictional new-customer landing page with A/B headline switch and event-preview UX |

## Run locally

No dependency or build step. Open `index.html` or serve the root directory:

```bash
python3 -m http.server 8000
```

Then browse `http://localhost:8000/`.

## Deployment

GitHub branch `feature/marketing-ax-portfolio-lab` is intended for **Vercel Preview**. Production `main` is not to be changed until preview review and approval. After merge, production updates through the existing Git integration.

## Editing workshop

1. Replace fictional candidate material with real verifiable achievements and links.
2. Research an employer, extract candidate-facing brand evidence, and replace `company-a/` concept.
3. Make or refine `DESIGN.md`, generate design exploration in Google Stitch, and explain final design choices.
4. Use Codex to implement and verify the landing page.
5. Document a campaign hypothesis, CTA events, and one A/B copy comparison.
6. Verify keyboard/mobile experiences and Vercel deployment.

## Important disclaimers

Kim Harin and Atelier A are fictional educational examples. The JD, sample projects and marketing campaign are mockups. No real promotion, discount, sign-up, scoring service, user tracking or verified performance metrics are provided. The campaign shows *local demo-only* event previews and does not send analytics events.

## File map

- `index.html`: personal portfolio
- `company-a/index.html`: employer-specific variation
- `campaign/index.html`: conversion-focused landing page
- `assets/site.css`: shared responsive design system
- `DESIGN.md`: brand/design tokens, experience and measurement assumptions
