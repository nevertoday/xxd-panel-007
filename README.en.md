<p align="center">
  <img src="./assets/banner.svg" alt="XXD Panel 007 project banner" width="1200">
</p>

<div align="center">

# 🦁 XXD Panel 007

### Turn a photograph into an intimate handwritten atlas for looking and reading

[![Codex Skill](https://img.shields.io/badge/Codex-Skill-000000?style=flat-square)](./SKILL.md)
[![Four Modes](https://img.shields.io/badge/Modes-4-d75d32?style=flat-square)](#four-outputs-one-observation-atlas-logic)
[![Raster Output](https://img.shields.io/badge/Output-PNG-3c6f67?style=flat-square)](#boundaries-and-trust)

<a href="README.md">简体中文</a> · <strong>English</strong> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a> · <a href="README.ar.md">العربية</a>

</div>

> OBJECT-LIKE MINIATURES · CLOSE-UP / SECTION / REPEAT · STAGGERED PAPER · THIN BLACK NOTES

XXD Panel 007 is an image-generation Skill for Codex and compatible agents. It decomposes one photograph into small physical-looking whole views, close-ups, sections, repeated pieces, and detail fragments, loosely distributed through the upper and middle of clean white paper.

Each fragment retains source material, colour, rounded contour, slight perspective, and hand-painted evidence. Thin black handwritten words, sound cues, and notes weave around the drawings to alternate looking and reading. It sits between a picture-book information page and an object notebook without becoming an icon table or sticker collection.

## Why it exists

“Journal style” easily collapses into neat icons, standard stickers, repeated labels, and unrelated trinkets where the source photo is only a replaceable theme name.

007 reverses that logic:

```text
lock source facts → choose useful whole / close-up / section / repeat / detail views → preserve physical material → stagger them through white paper → connect with thin black handwriting → finish with scan softness and pigment absorption
```

If an unrelated photograph could replace the source without materially changing fragment selection, material cues, handwritten observations, or reading order, the result is not 007.

## The 007 visual contract

- **One-source observations:** whole views, close-ups, sections, repeats, and details all belong to the same subject; there is no fixed cell count.
- **Physical note quality:** small scale, rounded contour, slight perspective, and hand painting preserve material and identity.
- **Grounded detail:** grain, browned edge, crumb, fibre, seam, reflection, texture, or section appears only when supported.
- **Loose reading:** fragments sit mostly in upper and middle zones, using staggered whitespace for a near-horizontal or script-appropriate flow.
- **No rigid grid:** reject tables, card walls, columns, centred specimen matrices, and equal icon systems.
- **Writing is structure:** thin black words, phrases, sound cues, and notes interweave with relaxed spacing and gently jumping baselines.
- **White paper and warm colour:** paper dominates, black writing carries information, and sparse dark or saturated accents carry focus.
- **Scanned touch:** slight softness, natural compression, uneven edges, and pigment absorption replace heavy shadow, borders, or forceful modern type.

## Samples · From X

> [Xiaoxiaodong (@xiaoxiaodong01)](https://x.com/xiaoxiaodong01/status/2090005645353468277) · 2026-08-19<br>
> GPT2 x 手账 x 手绘 x 插画 x 拆解 x 美学提示词 x VOL.007

<table>
  <tr>
    <td width="50%"><a href="https://x.com/xiaoxiaodong01/status/2090005645353468277"><img src="./assets/examples/sample-01.jpg" alt="XXD Panel 007 sample 1"></a></td>
    <td width="50%"><a href="https://x.com/xiaoxiaodong01/status/2090005645353468277"><img src="./assets/examples/sample-02.jpg" alt="XXD Panel 007 sample 2"></a></td>
  </tr>
  <tr>
    <td width="50%"><a href="https://x.com/xiaoxiaodong01/status/2090005645353468277"><img src="./assets/examples/sample-03.jpg" alt="XXD Panel 007 sample 3"></a></td>
    <td width="50%"><a href="https://x.com/xiaoxiaodong01/status/2090005645353468277"><img src="./assets/examples/sample-04.jpg" alt="XXD Panel 007 sample 4"></a></td>
  </tr>
</table>

<p align="center"><a href="https://x.com/xiaoxiaodong01/status/2090005645353468277">View the original post and full prompt →</a></p>

These samples demonstrate the 007 aesthetic motive. Their subjects, composition, palette, copy, and earlier canvas ratio never become generation references or current defaults.

## Four combinable output modes

Choose one or several modes with `1`, `1+3`, `1,2,4`, or `all`; `all` produces seven separate PNGs per source. After mode selection and before generation, the Skill explicitly asks for the whole finished canvas: the original-prompt `3:4`, an explicit source-aspect choice, a common ratio, or custom ratio/exact pixels. Source dimensions are never applied silently.

| Mode | Canvas rule | Result |
| --- | --- | --- |
| `top-bottom` | user-confirmed whole canvas | one complete generation: high-fidelity source above, 007 design below, approximately 50/50 |
| `left-right` | user-confirmed whole canvas | one complete generation: high-fidelity source left, 007 design right, approximately 50/50 |
| `design-only` | user-confirmed whole canvas | 007 design fills the canvas; source remains invisible |
| `wallpaper-pack` | confirmed per device | separate phone, iPad, desktop, and children's-watch PNGs |

Paired modes use the source as a high-fidelity edit/reference input and one complete style prompt to generate the finished composition directly, so photography, design, colour, light, typography, and meaning can cohere. Deterministic composition is fallback-only: after one targeted complete-canvas retry fails, when pixel-identical source preservation is explicitly required, when the active route cannot realise the canvas, or for lossless final pixel calibration.

Wallpapers may be linked or independent. A linked pack approves one iPad anchor, then recomposes every other device from the original plus that same anchor. An independent pack gives each device only the original. Neither crops another device output nor chains derivatives.

## Copy must let the viewer look and read in alternation

Before generation, choose automatic copy, custom copy, or text-free output. Name the target language or locale whenever copy is present.

Automatic copy derives a restrained set of words, phrases, onomatopoeia, and notes from visible material, action, function, relation, credible sensory suggestion, or known context. Sensory and memory claims require image evidence or user context.

The default is one title. Add zero to two short annotations only when they carry real information; never invent catalogue numbers, years, coordinates, or archival labels merely to look sophisticated. Copy must still pass the unrelated-image swap test.

Finished user wording stays verbatim. A direction or editable draft is refined only while preserving audience, purpose, mandatory words, tone, and implication.

Language follows the intended audience rather than the command language:

```text
target market or audience > requested output language > direction language; if none is explicit, ask before generation
```

A Japanese edition uses natural Japanese, a Korean-audience edition uses natural Korean and correct spacing, a UK edition uses British English, and Arabic defaults to natural Modern Standard Arabic with genuine right-to-left composition. The Skill never guesses nationality from appearance, clothing, scenery, or signs and never uses pseudo-foreign text.

## Complete-canvas first, raster-only delivery

The image model owns the aesthetics of the entire finished composition; paired layouts also default to one complete-canvas generation. `scripts/compose_panel.py` remains only for condition-based recovery, lossless pixel calibration, and read-only audit. It is not run pre-emptively and does not judge aesthetic success.

Every deliverable is a raster PNG and every invocation creates a fresh task under `~/Desktop/xxd/`. The configured image route exposes sanitised status only—never providers, endpoints, credentials, headers, prompts, responses, or account details. SVG, HTML, Canvas, diagrams, and programmatic drawing are not substitutes for the final artwork.

## Image-model priority

GPT Image 2 is the default first choice. It keeps this project's established workflow: high-fidelity source reference, explicit whole-canvas selection before generation, one complete-canvas generation for paired modes, and scripted composition only as a conditional fallback.

Seedance 5.0 Pro, Nano Banana Pro (Gemini Image Pro), Nano Banana 2 (Gemini Image Flash), or another compatible bitmap model may also be used when it is actually available through the current tools or configured routes and can satisfy source fidelity, whole-canvas ratio, target-language text, and linked-wallpaper multi-reference requirements. An alternative changes only the generation route; it must not change modes, canvas, copy, locale, wallpaper relationship, or the complete-canvas-first strategy.

If no suitable route is available, the Skill asks the user to enable an image-generation tool or provide an API key. User-provided credentials may be used for the current task without being echoed, displayed, logged, or exposed. They are not persisted, and provider, account, billing, or global route configuration is not modified, unless the user explicitly requests that configuration change.

## Get started

```bash
git clone https://github.com/nevertoday/xxd-panel-007.git
mkdir -p ~/.codex/skills
ln -s "$(pwd)/xxd-panel-007" ~/.codex/skills/xxd-panel-007
```

Claude Code users may link the same directory to `~/.claude/skills/xxd-panel-007`. Restart the agent session after installation.

```text
$xxd-panel-007
Turn this photograph into a left-right composition. Derive the copy from the image and write it in natural Korean.
```

You may invoke the Skill with only a photograph. It first asks for one or more modes in a numbered multiline menu, then for copy settings; wallpaper mode also asks for linked/independent continuity and device sizes.

Full specifications:

- [Skill workflow](SKILL.md)
- [Chinese full prompt](references/xxd-panel-007-prompt.zh-CN.md)
- [English full prompt](references/xxd-panel-007-prompt.en.md)
- [Original style brief](references/007-source.md)

## Boundaries and trust

- Each photograph stays within its own task and never borrows subjects, colours, copy, or composition from other inputs, old results, or samples.
- Every invocation creates a fresh task directory; even identical sources and parameters must generate anew.
- Deliverables are PNG bitmaps, never SVG, HTML, Canvas, or programmatic-drawing substitutes.
- The configured bitmap bridge emits sanitised status only and does not expose providers, endpoints, headers, credentials, prompts, or response bodies.
- Each selected ordinary mode returns one file; selected `wallpaper-pack` adds four separate wallpapers. `all` returns seven PNGs per source across four sibling mode directories, never a contact sheet or overview.

Local composition needs Python 3 and Pillow. The safe bitmap bridge uses Python 3.11+ `tomllib`. Image generation still requires a host agent with built-in raster generation or an already configured compatible raster route.

## Repository

```text
xxd-panel-007/
├── SKILL.md
├── README.md / README.en.md / README.ja.md / README.ko.md / README.ar.md
├── agents/openai.yaml
├── assets/
│   ├── banner.svg
│   └── examples/ (reserved for future local samples)
├── scripts/
│   ├── compose_panel.py
│   └── configured_imagegen.py
└── references/
    ├── xxd-panel-007-prompt.zh-CN.md
    ├── xxd-panel-007-prompt.en.md
    └── 007-source.md
```

## About XXD

XXD is the abbreviated brand name of Xiaoxiaodong. This project is created and maintained by [@xiaoxiaodong01](https://x.com/xiaoxiaodong01).

## Support and Membership

### In-depth Consultation · CNY 299/hour

One-to-one consultation for using the Skills is billed at CNY 299 per hour. Contact Xiaoxiaodong through the WeChat QR code below to book.

### Xiaoxiaodong Skills User Community · CNY 99 to join

A one-time CNY 99 fee joins the community for workflow sharing, work discussion, and peer support. It does not include hourly one-to-one consultation. Include “Skills User Community” in your WeChat message.

### Knowledge Planet + Member Prompt Library · CNY 699/year

[Knowledge Planet](https://wx.zsxq.com/group/15554814142882) and the [XXD Member Prompt Library](https://vip.xiaoxiaodong.ai/) are one membership: **one annual payment unlocks both, with no second purchase required.**

1. Subscribe through [Knowledge Planet](https://wx.zsxq.com/group/15554814142882), then contact Xiaoxiaodong on WeChat for a Prompt Library redemption code.
2. Subscribe through the [Member Prompt Library](https://vip.xiaoxiaodong.ai/), then contact Xiaoxiaodong on WeChat for a Knowledge Planet invitation.

<p align="center">
  <a href="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png"><img src="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png" alt="XXD paid community WeChat QR code" width="320"></a>
</p>

<div align="center">

**Do not line objects up; leave the act of observing them on the paper.**

</div>

---

<div align="center">
  <h2>☕ Support this open-source project</h2>
  <p>If this project saved you time, a Star, a share, or a coffee helps keep it moving.</p>
  <table>
    <tr>
      <td align="center" width="240">
        <a href="https://github.com/nevertoday/zhongguo-traditional-colors/blob/main/docs/images/buy-me-a-coffee-qr.png?raw=true"><img src="https://github.com/nevertoday/zhongguo-traditional-colors/blob/main/docs/images/buy-me-a-coffee-qr.png?raw=true" alt="Support Xiaoxiaodong through Buy Me a Coffee" width="180"></a><br>
        <strong>Buy me a coffee</strong><br>
        <sub>Scan or open the QR code to support Xiaoxiaodong</sub>
      </td>
    </tr>
  </table>
  <p><sub>Support is entirely optional and never changes access to this open-source project.</sub></p>
</div>
