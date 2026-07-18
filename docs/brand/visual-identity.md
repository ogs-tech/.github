# Visual Identity — brand reference

<!-- nav -->
[Docs](../) › [Brand](README.md) › Visual Identity

> *Information-oriented.* The exact specifications of the OGS tech mark: construction,
> color, typography, and usage rules. Source: **Guia de Marca, Ed. 03** —
> [live brand book](https://dx05qx18l5va6.cloudfront.net/ogs-tech/brand/).
> The logo SVGs live in [`assets/logo/`](assets/logo/).

For the *why* behind the mark, see [Company](company.md).

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/logo/logo-dark.svg">
  <img alt="OGS tech mark" src="assets/logo/logo-primary.svg" width="140" align="right">
</picture>

---

## Anatomy — "O Avião"

The symbol is a **paper plane** in solid silhouette, climbing forward and up:

- **Body** — lower wing + tail, in the structural color (indigo on light, paper on dark).
- **Wing** — the upper wing, always **amber** in the color variants: the brand's signature.
- **Crease (vinco)** — the fold from nose to notch that divides wing from body; the
  slogan's `›››` turned into form.

| Part | Role |
|---|---|
| **Wordmark** | `OGS` — solid, sans ("human voice") |
| **Descriptor** | `tech` — small, mono, letter-spaced, **amber** ("machine voice") |

---

## Construction & grid

The plane is geometry, not freehand — **4 points + 1 crease** on a `0 0 120 120` viewBox:

| Element | Spec |
|---|---|
| Body path | `M102 26 L58 66 L66 102 Z` |
| Wing path | `M102 26 L26 50 L58 66 Z` |
| Attitude | climbing at **~28°** — never level, never diving |
| Corners | slightly rounded — stroke 4, round joins, same color as fill |

---

## Variations & lockups

Four variants cover everything. Color variants use **one brand color + the amber wing**;
mono variants are **a single ink, no amber** — for engraving, low relief, and cheap
reproduction.

| Variant | Body | Wing | Use |
|---|---|---|---|
| **Primário** | indigo `#302F76` | amber `#E39C19` | light backgrounds — [`logo-primary.svg`](assets/logo/logo-primary.svg) |
| **Invertido** | paper `#F6F2ED` | amber `#E39C19` | dark backgrounds — [`logo-dark.svg`](assets/logo/logo-dark.svg) |
| **Mono tinta** | ink `#14133A` | same ink | engraving, single-ink print |
| **Mono claro** | paper `#F6F2ED` | same paper | single ink on dark, stamp-style |

- **Horizontal** lockup — symbol + `OGS tech`, for wide signatures
- **Empilhado** (stacked) — symbol → `OGS` → `tech`, for square spaces

The GitHub org avatar is the Invertido mark on ink — [`avatar-512.png`](assets/logo/avatar-512.png),
reproducible from [`avatar-512.svg`](assets/logo/avatar-512.svg).

---

## Scale & clear space

Tested from 72px (avatar) down to **16px (favicon)** — the decisive test: the wings must
not clog at minimum size. Reference steps: 72 / 48 / 32 / 24 / 16 px.

---

## Color

One shared **11-rung value ladder** (computed in OKLCH) carries three hue families —
indigo (structure), amber (signature), warm neutral (surfaces & text). A color's contrast
is a property of its rung: to retune, move the rung, never patch a one-off hex.

| Token | Rung | HEX | Role |
|---|---|---|---|
| **Ink** | indigo-900 | `#14133A` | primary ground |
| **Violet** | indigo-700 | `#302F76` | support · logo body on light |
| **Violet bright** | indigo-500 | `#5D58E1` | signal · large text/UI only · **Studio** |
| **Gold** | amber-300 | `#E39C19` | signature accent · logo wing · **Partners** |
| **Gold light** | amber-200 | `#F1BF79` | glint on dark |
| **Gold ink** | amber-600 | `#704A02` | amber as text on light |
| **Slate** | neutral-700 | `#3E3A34` | **Engine** |
| **Mist** | neutral-300 | `#B1ABA5` | secondary text on dark |
| **Paper** | neutral-050 | `#F6F2ED` | light ground · logo body on dark |

Hard rules:

- **No green in the identity.** Green exists only as the semantic *success* UI state — a
  separate system (success · warning · error · info), never brand identity.
- **No blue in the identity.** Blue was demoted in favor of indigo-violet — it exists only
  as the semantic *info* UI state. Indigo leads; amber signs.
- **Amber ≤ ¼** of any composition's area.
- Amber as *text on light* must use `#704A02` (amber-600), never `#E39C19` (amber-300).

---

## Typography

Two voices compose the system — both dependency-free system stacks (no webfonts):

| Voice | Stack | Use |
|---|---|---|
| **Sans — human voice** | `system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif` | wordmark & body text |
| **Mono — machine voice** | `"SF Mono", "JetBrains Mono", "Menlo", "Consolas", "Liberation Mono", monospace` | labels, data, the `tech` descriptor, PT·EN markers |

Modular scale ×1.25 (major third), base 16px: 13 / 16 / 20 / 25 / 31 / 39 / 49 / 61 / 76 / 96.
Body leading 1.5 · measure ~66ch (42ch narrow). All-caps strings always letter-spaced.

---

## Seal & stamp — retired in Ed. 03

The official seal and the physical stamp of the previous identity no longer exist in the
brand system.

---

## Misuse — do not

To protect recognition, never:

- ✕ Deform the mark or change the ~28° climb angle
- ✕ Recolor it outside the four variants
- ✕ Rotate it — level or diving reads as failure
- ✕ Add detail to the wing, or effects to the silhouette
- ✕ Place it on low-contrast backgrounds
- ✕ Swap the wordmark

---

See also: [Company](company.md) · [Brand Architecture](../explanation/brand-architecture.md)

---

↑ [Brand](README.md) · [Docs Hub](../)
