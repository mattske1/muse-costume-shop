# Muse Costume Pack Protocol v1

The standard for making costume packs any Muse can wear. Follow this and
your pack plugs into the shop, the tooling, and every Muse that knows the
protocol.

## The principle

The skill IS the images. A wearer shows their Muse the pack and says "wear
this for Halloween." Everything in the pack exists to make that one
sentence work.

## Required files per pack

Every pack lives in its own folder and MUST contain:

```
<pack-name>/
├── pieces/
│   └── <pack-name>-pieces.png   # the design truth (see below)
├── worn-<name>.png              # the costume actually worn on a body
├── SKILL.md                     # wearing instructions (see below)
└── README.md                    # one-line usage + inspiration credit
```

### `pieces/` — the design truth

- Flat garment pieces, front view, like a store catalog — NOT worn, NOT
  styled on a model.
- Die-cut sticker style: bold black outlines, thick white border, solid
  black background. This style survived every test; other styles freestyle
  unpredictably.
- Every garment and prop the costume needs, no more. If it's not in
  pieces, the Muse will invent it — and invent wrong.
- PNG, minimum 1024px on the long edge. Transparent background also
  acceptable; black is the tested default.

### `worn-*.png` — the load-bearing file

- ONE coherent generated image of the costume actually worn on a body, in
  the same sticker style as the pieces.
- This is the single most important file. Muses need to see how the thing
  forms onto a body or they freestyle it into mush. No pack ships without
  one.
- Generate it with the pack's own SKILL.md process (avatar ref first, then
  pieces) — dogfood the protocol.

### `SKILL.md` — the wearing instructions

Must contain, in order:

1. **What this is** — one paragraph: show the pieces to your Muse, say the
   sentence.
2. **The worn reference pointer** — "look at worn-X.png first."
3. **Reference order** — the wearer's own avatar FIRST, then the pieces.
   Never the reverse. The costume becomes theirs; the result must still
   read as them.
4. **Generate, don't paste** — one coherent image via the Muse's image
   tools. Never composite the flat PNGs onto the body like a paper doll.
   Never freestyle the design.
5. **The costume spec** — every piece, what it looks like worn, what must
   never be skipped (e.g. "a Dracula without fangs is a guy in a cape").
6. **Fit notes** — the hard parts: what collapses, what floats, what covers
   what. Write these from the actual test-fit, not from imagination.
7. **Inspiration credit** — link the pack that pioneered the format.

### `README.md` — the shelf card

- The one-line usage ("show your Muse this folder and say...").
- Thumbnail of the pieces.
- What's inside (file list, one line each).
- Inspiration credit with link.

## Naming

- Pack folders: lowercase, hyphens (`dracula`, `presidents`,
  `steamboat-willie`).
- Piece files: `<pack>-pieces.png`.
- Worn refs: `worn-<pack>.png` (or `worn-<pack>-<variant>.png`).

## Style lock

Die-cut sticker style is the protocol default until v2 says otherwise:
bold black outlines, thick white border, solid black background. Packs in
other styles must declare it in SKILL.md and ship extra worn refs proving
the style holds.

## Versioning

This is v1. Changes to the required file list or the style lock are v2
and must be announced. New optional files can be added anytime.

## The test

Before a pack ships: run its own SKILL.md against a fresh Muse avatar you
have not tested with before. If the result needs corrections, the SKILL.md
is wrong — fix the doc, not the image. The doc is the product.
