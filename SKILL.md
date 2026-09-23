---
name: product-website-workflow
description: Build, review, and iteratively refine product websites and campaign landing pages. Use when shaping site structure, storytelling, motion, responsive behavior, signup flows, assets, previews, or publishing for a product.
---

# Product Website Workflow

Use this workflow for websites and campaign pages across product categories. Adapt the story, visual language, proof, and interaction to the specific product, audience, and business goal; never assume a fixed product type or chapter map.

## Understand the project

- Inspect the current source, project instructions, recent approved versions, and the relevant styles, scripts, and assets before editing. Treat synced or explicitly read-only sources as reference material.
- Identify the exact page, breakpoint, state, or interaction the user wants changed. Treat corrections during work as scope-setting; for example, “desktop only” means leave mobile behavior unchanged.
- Preserve the latest approved direction and user decisions. Ask only for missing facts or choices that materially affect the result; otherwise make a reversible, clearly scoped assumption and say what it is.
- Keep product claims grounded in user-provided or verified facts. Never invent capabilities, performance figures, certifications, privacy properties, materials, or compatibility.
- Before a meaningful edit, briefly state the intended change in the user's language. Keep progress updates concise.

## Shape the story and visual system

- Choose a page structure that serves the product and campaign. A useful pattern may include a hero, problem or context, solution, demonstration, lifestyle or use cases, differentiators, and a conversion close—but use only the parts that fit.
- Use the product's established brand system when available. Otherwise define a coherent visual direction from the brief and existing assets; do not impose a preset palette or style.
- Favor clear hierarchy, deliberate typography, legible copy, and product-relevant imagery. Avoid generic card grids, dashboard/PPT treatments, abrupt section boundaries, and decorative motion that competes with the message unless the user explicitly wants them.
- Make transitions feel intentional. If scroll or touch controls a pinned cinematic stage, keep the stage visually fixed while its timeline advances, then release into normal page flow at the agreed point. Do not impose this interaction on every site.
- Keep motion responsive to keyboard and touch as well as pointer input. Respect reduced-motion preferences, maintain readable timing, and avoid scroll trapping.

## Responsive behavior and media

- Check the target desktop and mobile layouts for overlap, clipped controls, unreadable text, and viewport-specific behavior. Preserve any explicitly approved breakpoint decisions.
- For autoplay video, use muted inline playback where appropriate and account for browser restrictions. A failed `play()` must not silently advance a story or leave an empty stage; pause timeline-dependent copy while media buffers and provide a clear fallback when needed.
- Keep captions and visual claims synchronized with the corresponding media moment. Test chapter entry, playback start, buffering, exit, and repeat behavior at relevant viewport sizes.
- Distinguish concept/demo assets from approved production assets. Preserve supplied originals; prepare web-optimized derivatives when needed and retain source media according to the user's delivery preference.
- Do not imply a demo form stores an email, takes payment, or registers for a third-party service unless the integration is actually connected.

## Conversion and interaction

- Make forms, floating prompts, and CTA transitions part of the page's composition. When a floating signup merges into a final CTA, reserve layout space for it, animate the layout change deliberately, and verify both the transition and settled state so text or footer content is not covered.
- Make form states clear: idle, focused, invalid, submitting, success, and any next-step choice. Explain where data goes and do not collect or transmit real data in a preview unless the user authorized and the implementation supports it.
- Keep the interaction accessible: semantic labels, visible focus, keyboard operation, sufficient contrast, and reduced-motion handling.

## Review, preview, and handoff

- Verify the changed behavior in the actual page at relevant breakpoints. Inspect animation mid-state and end-state as well as text legibility, spacing, and overlap.
- Respect the requested preview scope. If the user asks for local-only review, do not publish. When publishing is requested or is an established part of the project workflow, use the existing host and preserve its audience and access settings.
- When updating a versioned repository as part of the request, add a concise user-facing change note and keep the version record aligned with the saved preview where that convention exists. Do not apply repository-specific conventions to unrelated projects.
- Finish with the preview or artifact link, a compact change summary, and any meaningful limitation.
