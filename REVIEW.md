# Portfolio redesign - local review

Branch: `design/charcoal-field-notes`
Implementation commit: `c1853223d629805d19751649c38be666ac72a71f`
Review updated: November 11, 2026 (Central time).

## Final revision

Neutral charcoal, warm off-white type, visible editorial rules, oversized Parker / Van Dyk masthead, split black-and-white film photograph, unboxed Koris presentation and numbered photography index. The resume shares the charcoal typography. This replaces the earlier sage design described by the previous review.

Existing content and destinations are retained, including the resume, Koris, photography galleries, social profiles and email. The homepage uses system fonts; the resume retains its existing Google font dependency. The local film image comes from Parker's linked B&W Pixieset gallery; the Chicago location was inferred from its skyline. Editorial copy is based on existing site content and project notes, without new career results or claims.

## Screenshot evidence

These are the original implementation-pass captures, recovered, visually inspected and copied into the shared task folder during this documentation correction. They are not new captures from this pass.

- Desktop homepage, full-page PNG: `C:\Users\Parker\.openmausbot\task-workspaces\9834cc51-f239-4eac-a83a-a28f8558ca21\bd343c47-2fe9-42b8-8e1f-0947f1dc54f8\desktop.png` (1265 x 3360 image pixels).
- Mobile homepage, viewport PNG: `C:\Users\Parker\.openmausbot\task-workspaces\9834cc51-f239-4eac-a83a-a28f8558ca21\bd343c47-2fe9-42b8-8e1f-0947f1dc54f8\mobile.png` (390 x 844 image pixels).
- Original copies: `C:\Users\Parker\.openmausbot\task-workspaces\36b2532e-3543-40dc-a994-06df253c8fc9\d9a419eb-946a-4346-b300-e4ea43466e63\desktop.png` and `mobile.png` in that same folder.

Desktop SHA256: `23A18305628796BE614C0171A8AAADDEFA25E7B334EC8BEE12E0210377DE0245`
Mobile SHA256: `B63173ADD3D64F4826497B040369087A4F82AE11E8EEF08161F33B564114B123`

The desktop capture shows the complete homepage, including work, photography, biography and contact. The 390px capture shows navigation, masthead, introduction and the top of the photograph. Both visibly match the final charcoal design. The desktop PNG width is the captured content width; the original desktop viewport height was not retained and should not be inferred from this full-page image.

## Verification and limits

Implementation-pass observations recorded in the original report: actual desktop homepage, desktop resume and 390px mobile homepage/work section inspected in the mounted Browser tab; photograph loaded; no horizontal overflow detected. There is no retained screenshot of the resume or mobile work section.

Rechecked during this correction:
- Branch and implementation commit confirmed; working tree initially clean.
- `git diff --check` passed.
- All 21 homepage href/src references checked: local files exist and fragment targets resolve (zero missing).
- Skip-link, visible keyboard-focus and reduced-motion CSS confirmed present; this is source inspection, not a complete accessibility audit.
- Both screenshot files opened for visual inspection; their dimensions and hashes read after copying to the shared folder.

Actual implementation preview address: `http://localhost:4173/` (resume: `http://localhost:4173/resume.html`). Reopening the homepage in this pass failed with `net::ERR_SOCKS_CONNECTION_FAILED`; no host listener on port 4173 was found. The preview is not verified running now. This failure does not invalidate the earlier saved captures, and no fresh rendering or viewport check is claimed here.

Still unverified: physical mobile devices, other browser engines, external destination availability, full keyboard and screen-reader behavior. No implementation changes were made during this documentation correction. No push, publication or deployment was performed.
