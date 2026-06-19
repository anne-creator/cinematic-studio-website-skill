---
name: cinematic-studio-website
description: Build or redesign a polished, responsive, dark cinematic landing page for a creative studio, artist collective, filmmaker, photographer, designer, or visual creator using React, Vite, TypeScript, Tailwind CSS, Framer Motion, and Lucide icons. Use when the user asks to turn their own brand information, biography, services, feature list, images, or videos into a shareable creative portfolio or studio website inspired by the bundled Prisma landing-page specification.
---

# Cinematic Studio Website

Build the website end to end. Treat the bundled Prisma specification as a visual starting point, not as content to copy blindly.

## Workflow

1. Inspect the current workspace before choosing whether to scaffold a new app or extend an existing one.
2. Read [references/intake.md](references/intake.md) and map the user's information into its fields.
3. Ask only for missing details that materially block a useful result. When the request is actionable, choose sensible defaults and build immediately.
4. Read [references/original-prompt.md](references/original-prompt.md) for the complete reference design and animation behavior.
5. Implement the page using the repository's existing patterns when present. For a new app, use React, Vite, TypeScript, Tailwind CSS, Framer Motion, and Lucide React.
6. Replace every Prisma-specific name, biography, service, CTA, and asset with the user's information. Never present placeholder claims as facts.
7. Run the app, inspect it at mobile and desktop widths, fix visible issues, and run the available build, typecheck, lint, or test commands.

## Personalization Rules

- Preserve the reference's mood: black surfaces, warm cream typography, restrained gray copy, rounded inset panels, cinematic media, and deliberate motion.
- Let the user's brand override the reference. Adapt colors, fonts, section names, card count, and copy when their identity calls for it.
- Use supplied media first. If media is missing, use a tasteful gradient or generated/local placeholder and clearly avoid pretending it belongs to the user.
- Keep external media URLs configurable in one data object or constants module. Add poster images or graceful fallbacks for videos where practical.
- Convert raw user notes into concise web copy while preserving meaning and voice. Do not invent awards, clients, years of experience, locations, or capabilities.
- Keep content data separate from presentation when practical so another person can personalize the result quickly.
- Use semantic landmarks, keyboard-visible focus states, descriptive alt text, sufficient contrast, and reduced-motion behavior.
- Avoid horizontal overflow, illegibly small navigation, giant text collisions, and autoplay video that ignores reduced-data or accessibility considerations.

## Default Page Shape

Use three sections unless the user's content suggests a better structure:

1. **Hero**: inset full-height media panel, compact navigation, oversized brand wordmark, positioning statement, and primary CTA.
2. **About**: dark card with a small discipline label, mixed serif/sans headline, biography, and restrained scroll-linked reveal.
3. **Capabilities**: responsive one-to-four-column cards for services, methods, programs, or product features.

Retain the shared word-pull animation components from the reference when they improve the result. Keep animation timing consistent and disable or simplify motion under `prefers-reduced-motion`.

## Intake Handling

Accept information in any form: prose, bullets, an existing site, a brand brief, or the template in [references/intake.md](references/intake.md). Normalize it into:

- identity and discipline
- audience and desired action
- hero statement and CTA
- biography and credibility details
- three to six capabilities
- navigation labels and destinations
- brand colors, typography, and tone
- image, video, logo, and social/contact assets

When a user provides only a name and short description, create a coherent first draft with editable placeholder capability labels and clearly generic copy.

## Completion Standard

Deliver a working site rather than a mockup or instructions. Confirm:

- production build succeeds
- primary navigation and CTA work
- layout is usable at approximately 390 px, 768 px, and 1440 px widths
- videos and images have fallbacks
- no Prisma-specific content remains unless the user explicitly chose it
- motion is tasteful and respects reduced-motion preferences
- the final response names the important files changed and the verification performed
