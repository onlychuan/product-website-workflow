---
name: miaolab-website-workflow
description: Build, review, and iteratively refine the MiaoLab Safety Outlet product website and Kickstarter story. Use when the user asks to change this site's sections, cinematic video flow, mobile behavior, launch signup, assets, preview, or publishing.
---

# MiaoLab Website Workflow

Use this workflow for the existing MiaoLab product website. Preserve the approved visual direction and the user's latest choices while making focused, reviewable changes.

## Start from the current site

- Inspect the current source, existing project instructions, recent version notes, and relevant page styles/scripts before editing. Treat synced `sources/` as read-only. Preserve user changes and leave unrelated routes and assets alone.
- Identify the exact area the user wants changed. A request such as “show me how it looks” means implement the requested preview and hand it to the user, not just describe a proposal.
- When the user gives a correction during work, treat it as steering: incorporate it into the same change. For example, “mobile does not need changes” means scope CSS and behavior to desktop and verify mobile declarations remain untouched.
- Ask only for missing product facts or decisions that would materially change the design. Keep confirmed product claims accurate; never invent performance numbers, certifications, components, or privacy properties.
- Explain the planned change briefly in Chinese before a meaningful edit. Keep progress updates short.

## Preserve MiaoLab's design and story

The current direction is editorial product film with industrial minimalism: deliberate typography, quiet product imagery, and restrained motion. Avoid generic cards, dashboard/PPT layouts, abrupt section transitions, excess decoration, and copy that competes with the product. Use the existing brand colors and components.

The page's current chapter map is:

1. Hero / home scene
2. Question / risk context
3. Technology / exploded product view
4. Proof / functional demonstration
5. Lifestyle / release into ordinary page flow
6. Experience & Privacy
7. Kickstarter call to action

Preserve the architecture and copy of the latest approved version unless the user requests a change. The cinematic opening has used one pinned full-screen stage for chapters 01–04; scroll or touch advances its timeline, then the page releases into normal flow around 05. If changing this behavior, keep the transitions continuous and ensure the interaction still works with keyboard, touch, and reduced-motion settings.

Use the current approved responsive decisions as project-specific preferences, not universal design laws: the desktop finale is a vertical centered composition with product film and heading above the signup; mobile layout has been explicitly kept unchanged. Reconfirm scope from the latest user message before adjusting either.

## Product video behavior

- For mobile playback, use muted inline video where appropriate and account for Safari and Chrome autoplay restrictions. A failed `play()` must not silently advance the story or leave a blank stage.
- Start the exploded view when its chapter becomes active, keep timeline copy tied to the actual video position, and pause progression while buffering. Provide a visible, accessible retry/play affordance if the browser blocks playback.
- Distinguish a tap from a real swipe before handing control to a scroll-driven scrubber. Keep a clear explore cue in an unobstructed position.
- Check video behavior at the relevant viewport and chapter boundary. Do not claim real-device coverage unless the user or an available device actually verified it.

## Floating launch signup and finale

The launch email capsule can expand when focused and merge into the final Kickstarter CTA. Keep the transition as one composition: reserve room for headings, let the final form and VIP states participate in page layout, and animate layout changes without covering text or footer content. Check both the moving state and the settled state, including capture, VIP choice, skipped reminder, and completion. At narrow widths, verify the user's approved mobile behavior rather than inheriting desktop-only adjustments.

The current signup may be a preview only. Keep its status truthful: do not imply an email was saved, a payment was taken, or a Kickstarter notification was registered unless those services are actually connected. Add legal/privacy copy or a new data destination only when needed and authorized for that implementation.

## Assets and product claims

- Distinguish concept/demo images from approved product renders, photography, and footage. Do not present a placeholder as a final or technically accurate product depiction.
- Preserve supplied originals; when preparing production assets, keep both the original media and a web-optimized copy. Do not request engineering project files when the user's established delivery preference is source footage plus web-compressed media.
- Keep the proof sequence legible: approach, detect, unused outlet off, lamp on. Do not imply that normal connected devices lose power if the product only disconnects an unused outlet.
- Privacy statements for this product (no camera, no microphone, no internet connection, with sensing and decisions on-device) were explicitly confirmed by the user. Preserve them accurately, and do not extend them into broader unverified guarantees.

## Review, preview, and handoff

- After the smallest scoped change, check the relevant desktop and mobile view, text legibility, clipping/overlap, and any altered interaction. Inspect the ending state of animations as well as the in-between frame.
- Respect explicit preview scope. If the user requests local-only review, do not publish. Otherwise use the project's existing Sites hosting setup and preserve its current audience; do not widen access. Reuse the established site and avoid creating duplicates.
- When publishing is requested or is the project's established workflow, use the Sites publishing process for the exact edited source, then open the updated preview so the user can inspect it.
- The user has an established MiaoLab GitHub workflow with Chinese version notes. When updating that repository as part of the requested work, add a concise user-visible change entry and keep the version record/tag aligned with the saved Site version. Do not apply this convention to unrelated repositories or push unrelated files.
- Finish with the preview link or artifact, a compact statement of what changed, and any meaningful limitation (for example, a demo form that does not store email). Do not call an attempted or pending deployment complete.
