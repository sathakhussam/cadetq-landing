# Product screen provenance

Captured on 2026-09-19 from the existing Training Intelligence app at localhost:5050 using its supported local-development sign-in. These are cropped screenshots of rendered pages, not recreated or generated product interfaces. WebP conversion preserves the captures at quality 90.

Cadet names, IDs, contact information, licence numbers and attachment names were anonymised in intercepted browser responses before capture. Other recorded training values and the original UI are preserved. No training, cadet, licence, communication or workflow records were changed. Captures are static examples, not live programme totals.

| Asset | Actual screen / source component |
| --- | --- |
| journeys.webp | `/live/admin`, expanded Acron Batch 08 in Cadet Journeys. `client/src/pages/app/admin-cadet-journeys.tsx`: BatchCard, StudentPhaseDisplay. |
| consolidated-view.webp | `/live/admin/consolidated-view`, Acron Batch 08 selected. `client/src/pages/app/admin-consolidated-view.tsx`. |
| milestones.webp | Flight Training cadet detail, Progression. `client/src/components/v2/progression-v2-tab.tsx`. |
| v2-delays.webp | `/live/admin/v2/delays`, logged and unlogged delay tables in the current recorded state. `client/src/pages/admin/flight-training-v2/delays.tsx`. |
| ground-training.webp | `/live/admin/ground-training`, Acron Batch 08, Tests Summary. `client/src/pages/app/admin-ground-training.tsx` and its existing test-summary component. |
| flight-training.webp | `/live/admin/flight-training`, Acron Batch 08, Batch Overview. `client/src/components/v2/batch-curriculum-overview.tsx`. |
| curriculum.webp | Flight Training cadet detail, Curriculum. `client/src/components/v2/student-course-tree-panel.tsx`. |
| fto-onboarding.webp | `/live/admin/fto-onboarding`, Acron Batch 08, Batch Summary. `client/src/pages/admin/fto-onboarding/batch-summary.tsx`. |
| post-process.webp | `/live/admin/post-process`, Batch Summary with stages, dates and document counts. `client/src/pages/app/admin-post-process.tsx`. |
| licenses.webp | `/live/admin/licenses`, existing RTR record. `client/src/components/LicensesTab.tsx`. |
| reports.webp | `/live/admin/reports?report=dgca-exams`, Acron Batch 08 selected. `client/src/pages/app/admin-reports.tsx`. |

The airline routes reuse several of these components; onboarding and reporting are captioned as programme-operations views. This page makes no claim that every airline role receives every administrative permission.

Capture scripts and intermediate images remain in the ignored `.impeccable/review/` directory. No browser credentials or session stores are included in the landing folder.

## Demo assets (assets/product/demo/)

Added 2026-10-11. The hero dashboard and the four Consolidated View states used in sections 1 and 3 are **demo recreations**, not captures. They are rendered from `prototypes/mocks/dashboard.html` and `prototypes/mocks/consolidated.html?s=pre|dgca|disc|ft` with headless Chrome at 2x, so no real academy, batch, staff or cadet data appears on the page. Every name, batch code, total and flight-training value is invented (generic placeholders: "Flight Academy", "Partner FTO", "Batch 07", "Batch 10", "Batch 11", "FT-07A/B/C"). To change the data, edit the mock and re-render. The original captures are left in place but are no longer referenced by sections 1–3.
