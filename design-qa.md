# VanillaSky Design / Functional QA

## Reference observed

- Source: `https://app.vanillasky.ai/start` and the authorized test draft editor at `/create?id=…`.
- Captured desktop and 390×844 mobile source viewports.
- Observed flow: vehicle photos/details → video format and shape → style, background, music, voice, brand → storyboard review → payment and AI video generation.
- Only the editor before payment was inspected. The source paid generation action was not activated.

## Implementation

- Independent Korean responsive upload, settings, storyboard and preview UI informed by the inspected flow.
- Local photo upload (3–20), car details, format/ratio/style/overlay color/music options, local logo, scene editing/reordering and canvas preview.
- Client-side WebM export from the canvas and browser Korean voice preview.
- No source account backend, paid AI generation, external listing import, payment, cloud storage or server-based AI voice. Background presets tint the original photo; they do not replace its background. Audio is synthesized ambience, not licensed or AI music. These distinctions are shown in the UI and README.
- Test photos remain outside the public source repository.

## Verification

- Deployed GitHub Pages flow: uploaded the provided 3 BMW photos, filled vehicle details, advanced to the editor, selected social format/9:16 and confirmed a real-photo vertical preview.
- First WebM export test reached 100% but did not complete in the embedded browser. Updated the renderer with a bounded stop-event wait; final download behavior still requires confirmation.
- Browser console showed no errors during the observed session.
- Source AI generation/payment parity not tested or claimed.

## Current outcome

Photo upload and preview are verified on the deployed site. WebM download and generated-AI parity are not yet confirmed; do not describe the app as identical to the source AI service.
