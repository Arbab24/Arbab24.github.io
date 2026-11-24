# QA report: Smart water bottle Germany prototype

Reviewed: `04-prototype/index.html` against `02-strategy.md` and `03-copywriting.md`.

## Must fix

- 🔴 None. The page is explicitly labeled as a concept, and uncertain product behavior (sensor tracking, app compatibility, cleaning, privacy, subscription) is qualified instead of presented as verified fact. No checkout or unsupported purchase promise is present.

## Improvements

- 🟡 **Expose the app mockup meaningfully to assistive technology.** `.phone` has an `aria-label` but no accessible role, so the label may not be announced. Either mark the mockup `role="img"` with a concise label and keep its contents decorative, or structure its text and progress as real content. The progress bar's `aria-label` also lacks a role/value, so it currently conveys no progress semantics; use a labeled `role="progressbar"` with `aria-valuenow/min/max` only if the illustrative 62% is intentionally exposed, otherwise hide the decorative bar from assistive tech.
- 🟡 **Clarify the privacy benefit before public use.** The copywriter's approved phrase says user data stays under their control, while the prototype softens this to “see what data the app uses and what settings can be changed.” The page avoids making a guarantee, but the proposed privacy promise still needs confirmation against actual data flows and controls as copy notes specify.
- 🟡 **Add launch information before converting visitors.** There is no price, shipping/returns, materials/capacity, compatibility, or contact/legal links. This is acceptable for a concept page, but these details are needed before publication or paid traffic.
- 🟡 **Consider explicit keyboard focus styling.** Links/buttons retain browser defaults, but a consistent visible `:focus-visible` treatment would improve keyboard navigation and match the visual system.

## Passed

- 🟢 Responsive single-column layout at narrow widths; feature cards collapse cleanly, navigation CTA remains available, and the content order is coherent.
- 🟢 Semantic landmarks and section headings are present (`header`, labeled `nav`, `main`, sections, `footer`, one `h1`); FAQ uses native `details`/`summary` controls.
- 🟢 Hero, benefits, process, CTA, and FAQ align with the supplied German copy and the desk worker/student target segment.
- 🟢 Sensor accuracy, phone compatibility, cleaning, privacy, and subscription details are framed as conditional or pending validation. No medical, sustainability, water-quality, or superiority claims were introduced.
- 🟢 No external assets, scripts, or network dependencies; reduced-motion preference is respected.

## Overall

No 🔴 blockers. Suitable as a reviewable concept prototype; verify the product and privacy statements and add the final purchase/legal information before public launch.
