# Asset Map

Which provided image is used where, and why.

| Source image (as provided) | Repo file | Used in |
|---|---|---|
| Coding-room desk scene — dual monitors, white tiger, neon city skyline through the window — cropped to a wide 2.5:1 banner (trimmed ceiling/plants above and desk clutter below) with a subtle top/bottom vignette added | `assets/hero/hero.jpg` / `.webp` | Top of `README.md` — the cinematic hero banner |
| Mountain overlook at night — figure with a white tiger, city and river below, "Keep Building Krish…", "Ideas · Build · Learn · Create · Repeat" | `assets/backgrounds/mountain-night.jpg` / `.webp` | Closing/footer section of `README.md` — the cinematic sign-off |
| Dashboard-style mockup (profile card, About Me, Currently Building, Featured Projects, Tech Stack, GitHub Analytics, Achievements) | *not copied into the repo* | Used only as the **layout reference** for how `README.md` is structured — GitHub Markdown can't render a live dashboard like that, so its structure (not its pixels) was translated into Markdown/HTML sections |

## Why some assets are placeholders

- **Project banners** (`assets/projects/vyom.svg`, `kairos.svg`, `bitvault.svg`)
  are original, generated SVG cards (dark background, blue/violet glow) rather
  than real product screenshots, since no screenshots of VYOM, KAIROS, or
  BitVault were provided. Swap in real screenshots or GIFs when you have them —
  same filenames, any aspect ratio close to 700×220 will drop in cleanly.
- **Profile avatar**: instead of a static image, the README uses your live
  GitHub avatar (`https://github.com/<username>.png`), so it always matches
  whatever you have set on your account. No file needed.
- **Typing animation** in the hero badge row is generated on the fly by
  `readme-typing-svg` (an external, GitHub-compatible service) — no local GIF
  required, and it's easy to edit the text via the URL's `lines=` parameter.

## Image optimization

Both photographic images were resized to a 1400px-wide max and saved as both
`.jpg` (universal compatibility) and `.webp` (smaller, GitHub renders it fine)
so the repo stays lightweight — the two images together are under 1 MB rather
than the multi-megabyte originals.
