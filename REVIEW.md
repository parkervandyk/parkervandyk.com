# Photographic contact sheet redesign

Replaces the oversized editorial homepage with compact fixed identity/navigation, asymmetric photographic contact sheet and hash-addressable About/Work panels. Mobile uses a compact header and staggered two-column sheet. Actual bio, Envoy, Koris, resume, social, email and four gallery destinations retained. Resume document retains its existing styling.

Assets: film.jpg retained locally; color.jpg, medium.jpg and digital.jpg downloaded from the corresponding public Pixieset collection cover images on 2026-11-12. No invented geographic labels. No generated images.

Fresh verification on 2026-11-12 in the mounted Browser tab:
- 1280 x 720 desktop viewport: all four images loaded; document horizontal overflow false. Full-page screenshot visually inspected.
- 390 x 844 same-origin iframe viewport in the mounted browser (not physical device emulation): all four images loaded; horizontal overflow false. Screenshot visually inspected.
- Work panel rendered and Koris URL verified in browser. About/Work are native hash targets, close links return to sheet, Escape returns focus to navigation. Script makes background inert while panels open; visible focus and reduced-motion support included.
- 26 homepage href/src references checked: zero missing local files or fragment targets. git diff --check passes.

Screenshots in repository parent folder: contact-sheet-desktop.png and contact-sheet-mobile.png. Source screenshots: C:\Users\Parker\.agent-browser\tmp\screenshots\screenshot-1794486265960.png and screenshot-1794486291146.png.

Limits: full keyboard/screen-reader audit, physical devices, external link availability and fresh resume rendering unverified. The mobile capture is the initial viewport, not the full page. No push, publication, deployment, accounts or costs. Initial localhost navigation failed with ERR_SOCKS_CONNECTION_FAILED; 127.0.0.1:4173 subsequently worked with local preview server.
