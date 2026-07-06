
## Deliverable

A single PowerPoint file `Armana_Group_Kaizen_Rollout_BuyerReview_July2026.pptx` saved to `/mnt/documents/` and shared as a `<presentation-artifact>`. Font: **Inter Tight** throughout. Visual pattern (color, structure, chart style) mirrors the approved `Kaizen_update_Armana_Group - Compressed.pdf`, with rollout details taken from `Kaizen_Rollout_plan_Armana.xlsx` and phase content from `Book1.xlsx` / `Rollout.docx`.

## Narrative Arc (Customer-Centric)

Frame: "We committed → we delivered in Armana Apparels (Apr–Jun) → same disciplined playbook now rolling out across the full group on committed dates."

## Slide Outline (approx. 18 slides)

1. **Title** — Armana Group Kaizen Rollout | Buyer Review | July 2026
2. **Agenda** — Journey so far, results, playbook, group rollout plan, governance
3. **Armana Group at a Glance** — 5 factories, total lines (10+8+12+12+41+27+32), impacted lines summary
4. **Kaizen Vision & Buyer Commitment** — Efficiency, quality, on-time delivery, sustainability
5. **Phase 1 Recap — Armana Apparels & Fashions Ltd (Apr–Jun 2026)** — Pilot L4 & L12; approach summary
6. **Phase 1 Results — Before vs After** — Efficiency 63%→70%, DHU 5%→2%, 5S 50%→85%, changeover 60→30 min, multiskill 20%→30% (from Book1.xlsx targets, framed as achieved/on-track)
7. **The Kaizen Playbook — 3 Cycles** — Cycle 1 Bottleneck/Motion/Machine speed · Cycle 2 Defect + Layout · Cycle 3 5S + Automation
8. **Cycle 1 Detail** — Kaizens, KPIs, responsibilities (from Book1.xlsx)
9. **Cycle 2 Detail** — Defect reduction, workstation layout, material flow
10. **Cycle 3 Detail** — 5S foundation, visual management, automation
11. **Group Rollout Master Plan (Gantt)** — Visual timeline Apr'26–Jun'27 for all 5 factories × Pilot/Phase I/II/III (from rollout Excel)
12. **Factory Rollout — Armana Apparels** — 12 lines, Pilot (L4,L12) → I (L3,L5,L12) → II (L2,L8,L11) → III (L1,L6,L7,L10)
13. **Factory Rollout — Zyta Apparels** — 12 lines, Pilot L4 & L12, July start
14. **Factory Rollout — Denimach** — 41 lines, Pilot L1 (Padam Line-1), 11–23 July
15. **Factory Rollout — Denitex** — 27 lines, Pilot L1, L12 & L25; scope: workstation/motion, line balancing, changeover, multiskill, OT reduction, NVA elimination
16. **Factory Rollout — Sterling Styles** — 32 lines, Pilot L8
17. **Governance & Cadence** — Weekly Gemba, monthly steering, buyer review cadence, escalation
18. **Commitment to Buyer / Next Steps** — Milestones, next review date, ask

## Design System

- Palette: **Midnight Executive** — navy `#1E2761` primary, ice blue `#CADCFC` secondary, white accent, coral `#F96167` for KPI callouts (matches serious industrial tone).
- Typography: Inter Tight for all text (title 40–54pt bold, section 28–32pt, body 20–24pt, caption 14–16pt).
- Motif: thin left-side navy bar + rounded ice-blue KPI cards; consistent footer with "Armana Group | Kaizen Rollout | Buyer Review — July 2026".
- Every slide has a visual (Gantt bars, KPI cards, icon rows, before/after columns, factory cards) — no text-only slides.

## Technical Approach

- Build with `python-pptx` (16:9, 13.333×7.5 in).
- Register Inter Tight via `run.font.name = "Inter Tight"`.
- Gantt: draw colored rectangles per factory-phase row aligned to a month grid derived from the Excel.
- Data pulled programmatically from `Kaizen_Rollout_plan_Armana.xlsx` and `Book1.xlsx` so numbers are traceable.

## QA Checklist

1. Render to PDF via LibreOffice, convert every slide to JPG at 150 DPI.
2. Inspect each slide image for: overflow, overlap, low contrast, wrapping titles breaking layout, Gantt alignment, leftover placeholder text.
3. Grep for "Lorem", "XXXX", placeholder strings.
4. Fix and re-render until clean, then emit the artifact tag.
