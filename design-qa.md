# VanillaSky Design / Functional QA

## Reference observed

- Source: `https://app.vanillasky.ai/start` and the authorized test draft editor at `/create?id=…`.
- Captured both a desktop viewport and a 390×844 mobile viewport.
- Source flow: vehicle photos/details → video format and shape → video style, background, music, voice, brand → storyboard review → payment and AI video generation.
- Source uses a warm ivory surface, understated dark text, muted green accents, compact selection cards, a left vehicle summary, and a sticky mobile review action.
- Only the publicly available editor before payment was inspected. The paid source generation step was not activated.

## Implementation

- Independently implemented Korean upload and editing UI, matching the observed flow and visual language.
- Local photo upload (3–20), basic car information, selection cards, storyboard reorder/text/photo selection, canvas preview, browser WebM rendering/download.
- Added browser-based Korean voice preview and local synthesized ambience. No source account backend, AI generation, external listing import, payment, or cloud storage is claimed.
- User-provided test images and their metadata were not copied into this public source repository.

## Verification

- Pending local browser verification of upload → editor settings → preview → WebM export and deployed Pages.
- Source service paid video comparison not performed: user approved inspection of test upload and vehicle information, but not payment or generation.

## Current outcome

**Blocked pending local and deployed verification.** Do not report source AI video parity; this version creates a client-side slideshow video from the user's photographs.
