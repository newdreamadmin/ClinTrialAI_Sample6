# ClinTrialAI — homepage review

Homepage-only implementation, preserving the existing site's static HTML/CSS/JavaScript architecture. No framework migration or runtime dependencies are required.

## Run

Requires Node.js 20 or later.

```sh
npm run build
npm run dev
```

Open http://127.0.0.1:4173. After source edits, run the build again and refresh. Deploy the contents of `dist/` to any static host.

## Structure

- `src/components/`: reusable, build-time section modules. The output is semantic HTML, available before JavaScript loads.
- `src/styles.css`: design tokens, responsive layouts, shared animation rules, and reduced-motion overrides.
- `src/main.js`: mobile navigation, scroll lifecycle state, viewport reveals, conceptual score animation, and information dialogs.
- `public/images/`: supplied logo and favicon, preserved without alteration.
- `build.mjs`: dependency-free static build.

## Content and launch notes

- Only the homepage is built; navigation links target homepage sections.
- Demo and team CTAs open email to `info@clintrialai.com`, taken from the existing site's contact page. No emails are sent automatically and no submission backend is implied.
- Retention score, patient identifier, and indicators are clearly marked as conceptual/demo data.
- Privacy and Terms currently open contact-information dialogs. Replace these with approved legal documents before a public launch; no legal terms have been invented.
- DM Sans loads from Google Fonts with a system-font fallback. For a fully self-contained deployment, self-host the approved font files.
- Existing files at the original website location are unchanged. This folder is the review deliverable.

## Validation

Reviewed at 1920, 1440, 1366, 1024, 768, 430, 390, and 375 pixel viewport widths. No horizontal document overflow was detected. Mobile menu focus, Escape dismissal, anchor navigation, single-H1 structure, and demo destinations were checked. Reduced-motion styling provides a static experience.
