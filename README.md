# Bikram & Itishree — Wedding Website

**Wedding date:** 13 December 2026  
**Location:** Bhubaneswar, Odisha, India  
**Website:** https://bikram-90.github.io/bikram-weds-itishree/  
**Repository:** https://github.com/bikram-90/bikram-weds-itishree

A bilingual wedding invitation website for Bikram and Itishree, hosted with GitHub Pages.

## Latest release — 3 November 2026

- A language-selection screen is shown on every fresh open and page refresh. Guests choose English or Odia; the choice is not persisted between page loads.
- English transliteration updated from **“Shubha Bibaha”** to **“Subha Vivaha”**.
- Background soundtrack uses a single speaker control; it starts muted where browser autoplay policies allow and guests can tap to unmute.
- Scratch-card foil resets on page reload.
- Travel & Connectivity appears immediately after Venues.
- GoatCounter visitor-count integration includes a fallback status if the service is blocked or unavailable.
- Existing couple hero artwork and event assets are retained.

## Repository contents

- `index.html` — website entry point. Keep this file in the repository root.
- `.nojekyll` — prevents GitHub Pages/Jekyll from filtering site assets.
- `assets/` — local artwork, logos, event illustrations, and decorative motifs.
- `README.md` — this project and deployment guide.
- `README.txt`, `SETUP.txt`, `TRAVEL_INFO.txt`, `DEPLOYMENT_QA.txt` — supplementary project notes.

## Deploy to GitHub Pages

1. Download and extract the latest deployment ZIP.
2. Open the GitHub repository: https://github.com/bikram-90/bikram-weds-itishree
3. Select the `main` branch.
4. Choose **Add file → Upload files**.
5. Upload the *contents* of the extracted ZIP to the repository root. Do not upload the ZIP file itself and do not create an extra enclosing folder.
6. Confirm that `index.html`, `.nojekyll`, and `assets/` appear at the root, then commit the changes to `main`.
7. In **Settings → Pages**, confirm GitHub Pages is configured to deploy from `main` and the `/(root)` folder.
8. Open the **Actions** tab and wait for the Pages deployment to complete.
9. Visit https://bikram-90.github.io/bikram-weds-itishree/ and hard-refresh the page if an older cached version appears.

## RSVP email configuration — action required before launch

The RSVP form opens a WhatsApp message and also submits the message through FormSubmit's AJAX service. The current recipient configured in `index.html` is `bikramwedsitishree@yopmail.com`.

**Privacy warning:** YOPmail inboxes are public and password-free. Anyone who knows the inbox name may be able to read messages. Do not use this address for private guest information. Before sharing the site widely, replace the configured RSVP email address in `index.html` with a private mailbox you control.

After changing the address:

1. Deploy the updated `index.html`.
2. Submit one test RSVP.
3. Open the destination mailbox and complete FormSubmit's one-time activation/confirmation if requested.
4. Verify that the test submission arrives and that the WhatsApp draft opens correctly.

## Visitor counter — GoatCounter

The website uses:

- Counter endpoint: `https://bikramwedsitishree.goatcounter.com/count`
- Script: `https://gc.zgo.at/count.js`
- Site-wide public counter path: `TOTAL` (a supported GoatCounter special path).

Recommended settings and checks:

1. In GoatCounter, set **Your site** to `https://bikram-90.github.io/bikram-weds-itishree/`.
2. Keep **Allow adding visitor counts on your website** enabled.
3. **Dashboard viewable by** controls dashboard privacy; it does not determine whether the public counter can be embedded.
4. **Individual pageviews** may remain disabled if only aggregate totals are needed.
5. If the website reports that the counter is blocked or unavailable, test in a private/incognito window with browser extensions disabled. Privacy tools and ad blockers may block `gc.zgo.at` or the GoatCounter domain.
6. Public counter responses may be cached, so a new visit may not appear immediately.

The visitor counter depends on the external GoatCounter service and the visitor's browser/network settings. A missing count does not necessarily mean the website itself failed to load.

## Music and browser behaviour

The soundtrack is controlled by one speaker icon near the bottom-right of the page. The site starts playback muted where the browser allows muted autoplay. A guest must interact with the speaker control to enable audible playback; browsers do not allow websites to force sound on automatically before user interaction.

## Event schedule

| Event | Date and time | Venue |
|---|---|---|
| Mehendi — The Green Gala | 12 December 2026, 6:00 PM onwards | K-4/10, Kalinga Vihar, Bhubaneswar |
| Haldi — The Yellow Affair | 13 December 2026, 10:00 AM onwards | K-4/10, Kalinga Vihar, Bhubaneswar |
| Wedding — Petals & Promises | 13 December 2026, 7:30 PM onwards | The Regal Palm, Cuttack–Puri Bypass Road, Bhubaneswar |
| Reception — The Afterglow | 20 December 2026, 7:00 PM onwards | DM Convention, Aiginia, Bhubaneswar |

---

For deployment, always use the latest version of the deployment ZIP and upload its extracted contents to the repository root.
