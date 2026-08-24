# XXD Panel 007 · Handwritten Everyday Observation Atlas Core

## Runtime complete-canvas contract — highest priority

- `TOP_BOTTOM` and `LEFT_RIGHT` default to one complete finished generation using the current source as a high-fidelity edit/reference input. Do not pre-split the job into photographic and design halves.
- Top-bottom keeps the faithful source in approximately the upper 50% and performs this style transformation below; left-right uses the faithful source in approximately the left 50% and the transformation on the right. Unify both regions through colour, light, rhythm, typography, and meaning.
- `DESIGN_ONLY` and `WALLPAPER_PACK` use the complete canvas while the source remains an invisible identity/content reference. Recompose every wallpaper separately for its device.
- `FINAL CANVAS` means the ratio/pixels of the whole finished artwork and must be explicitly resolved before generation; never apply source dimensions silently. `DESIGN FRAME` is used only if a failed complete-canvas retry triggers deterministic composition fallback.
- Retry a failed complete canvas once against the failed constraint only. Scripted composition is allowed only after that retry still fails, when pixel-identical source preservation is explicitly required, when the active route cannot realise the canvas, or for lossless pixel calibration.

### Model priority and credentials

- **Prefer GPT Image 2.** When GPT Image 2 is available through the current built-in image tool or a configured compatible route, use it first for the high-fidelity reference/edit and complete-canvas generation required by this prompt.
- Also support Seedance 5.0 Pro, Nano Banana Pro (Gemini Image Pro), Nano Banana 2 (Gemini Image Flash), or another compatible bitmap model only when the actual route can preserve the source, realise the whole finished canvas, render the target-language text, and accept the multiple references needed by a linked wallpaper pack.
- An alternative model changes only the generation route. It must not change this prompt's modes, canvas, source visibility, copy, locale, wallpaper relationship, or complete-canvas-first / composition-fallback-only logic. Do not silently downgrade a hard requirement.
- If no suitable route is available, ask the user to enable an image-generation tool or provide an API key. User-provided credentials may be used for the current task, but never echo, display, log, or expose their value in chat, prompts, or diagnostics. Do not persist them or modify global route configuration unless explicitly requested.
- Judge availability by actual image capability, not by a provider name or one missing environment variable.

Treat the one currently selected photograph as the sole content source. Never borrow objects, observations, composition, palette, or copy from samples, other inputs, or historical outputs.


## 0. Immutable aesthetic motive

**this exact photographed subject or inseparable relation → at least three identity, material, action, function, or relation cues → decomposition into several small physical-looking whole views, close-ups, section cuts, repeats, small pieces, or detail fragments → rounded contours, slight perspective, source colour, material texture, and hand-painted evidence → loose distribution through the upper and middle of dominant clean-white paper → staggered whitespace creating an approximately horizontal or script-appropriate reading rhythm rather than a table → thin black handwritten words, short phrases, sound cues, and annotations woven around the drawings → scanned-paper softness, pigment absorption, uneven edges, and an optional small footer line**.

Intimacy comes from observing source-specific material, suggested touch, repetition, section, action, sound evidence, or a visible carrier of memory. Never invent biography, place, event, ownership, emotion, memory, taste, or sound; sensory copy requires visible evidence or user context. If an unrelated photo could replace the source without materially changing fragment selection, material cues, handwritten observations, or reading order, the result has failed.

## 1. Lock source facts and observations

Privately determine:

1. The one principal subject or inseparable relation and at least three source-specific identity, material, action, function, or relation cues.
2. One recognisable whole or principal fragment, plus only the close-ups, sections, repeats, small pieces, or details that reveal useful information. Let content determine count; never impose a fixed grid.
3. The source basis for every fragment's contour, colour, material, opening, connection, layer, grain, browned edge, crumb, fibre, reflection, seam, or texture.
4. A loose upper/middle distribution, staggered gaps, and approximately horizontal or script-appropriate reading order.
5. The hierarchy of white paper, thin black writing, warm clean subject colour, and sparse saturated warm, dark, or theme-supporting accents.
6. When copy is present, evidence-led short words, phrases, sound cues, or notes for useful fragments, plus whether one small footer line is warranted.

## 2. Physical-looking observation fragments

- Every miniature belongs to the same source subject and reads as another way of observing it, never as an unrelated collection.
- Preserve small scale, rounded contour, slight perspective, and hand-painted evidence. Whole, close-up, section, repeat, and fragment views should differ meaningfully in scale and function.
- Grain, browned edge, crumb, texture, fibre, seam, reflection, or section detail appears only when supported by the source.
- Never standardise fragments into equal size, identical outline, or identical angle. Reject stock stickers, cartoon faces, and library icons.

## 3. Clean paper and loose reading rhythm

- Clean white or gently warm paper occupies the largest area. Fragments live mainly in the upper and middle zones with generous staggered gaps.
- The composition may read approximately horizontally, but never becomes straight rows, a strict table, card wall, labelled columns, or centred specimen grid.
- Connect observations through proximity, whitespace, repeated material, and handwritten phrases. Use arrows or leader lines only when truly necessary, keeping them sparse and hand-drawn.
- A small signature-like explanation, number, date, title, or theme phrase may sit near the bottom only when supplied or reliably established. It may not become branding.

## 4. Hand-painted material and colour

- Miniatures retain the source's own material, colour, and recognition cues through warm, clean, slightly high-value hand painting.
- White paper carries space; thin black handwriting carries information. Sparse saturated warm, dark, or supporting colour is reserved for focus, shadow, texture, and rhythm.
- Preserve slight scanned softness, natural compression, uneven edges, and pigment absorption without a digital-noise filter.
- Reject heavy cast shadow, decorative border, forceful modern typography, smooth vector icons, plastic stickers, photorealism, complex volume, and 3D.

## 5. Typography specific to 007

Type is the atlas's structural backbone, making the viewer look and read in alternation—not a pasted labelling system.

- Automatic copy derives a restrained set of short words, phrases, onomatopoeia, and notes from visible material, action, function, relation, credible sensory suggestion, or known context. Write only where a fragment genuinely benefits.
- Preserve final user wording verbatim. Use place, date, number, signature, and memory claims only when supplied or reliably established.
- Use thin black, lightly childlike or naturally handwritten forms with relaxed spacing and a gently jumping baseline. Preserve native construction across scripts.
- Weave notes to the left and right of drawings; let some touch an edge and others float in whitespace. Preserve breath and never cover defining material cues.
- Reject heavy commercial titles, rigid sans-serif labels, repeated capsules, data legends, pseudo-foreign text, and decorative pseudo-writing.

The photographic panel contains no typography. Text-free mode contains no letters, characters, numbers, or pseudo-text anywhere in the transformed frame.

## 6. Current mode and wallpaper

The caller appends the one current mode, exact dimensions, source visibility, and locked copy. Execute only those values.

- Recompose fragments, whitespace, and reading order for every wallpaper aspect. Keep system-UI zones low-information and render no UI or device frame.
- A linked wallpaper always receives the original source plus the same approved anchor: the source locks identity and content; the anchor locks only fragment grammar, loose reading rhythm, white-paper balance, hand-painted material, colour warmth, scan texture, and handwritten-note behaviour. Never crop mechanically or chain derivatives.

## 7. Pre-generation check

1. At least three source-specific cues remain across the observation fragments, and every fragment belongs to one subject.
2. Whole, close-up, section, repeat, or detail choices carry information; there is no fixed cell count or unrelated filler.
3. White paper dominates; fragments sit loosely through upper and middle zones in a readable rhythm that is not a table, grid, card wall, or icon set.
4. Miniatures preserve rounded contour, slight perspective, source material, colour, and hand-painted evidence; every detail is grounded.
5. Thin black handwriting genuinely connects looking and reading; words, sound cues, and notes are accurate, natural, and native to the locale.
6. White paper, black writing, warm clean subject colour, and sparse accents form a clear hierarchy with scanned softness, pigment absorption, and uneven edges.
7. There is no heavy shadow, border, forceful modern type, generic sticker, commercial cartoon, smooth vector, photorealism, 3D, logo, watermark, UI, or mockup.
8. Mode, size, source visibility, wallpaper safe areas, and copy obey the appended values.
