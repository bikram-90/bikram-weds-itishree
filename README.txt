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

## Post-deployment QA checklist

- [ ] Open the website in a new tab and confirm the language-selection screen appears.
- [ ] Refresh the page and confirm language selection appears again.
- [ ] Select English and Odia; check headings, event details, navigation, buttons, RSVP labels, and helper text.
- [ ] Confirm “Subha Vivaha” appears in the intended English wording.
- [ ] Confirm event artwork and the couple hero image load on desktop and mobile.
- [ ] Confirm the speaker icon toggles mute/unmute and no floating YouTube player is visible.
- [ ] Scratch the card, refresh, and confirm the foil resets.
- [ ] Confirm the section order is Venues → Travel & Connectivity → RSVP.
- [ ] Test Google Maps and Google Calendar links for each event.
- [ ] Test the RSVP WhatsApp draft and email delivery after configuring a private recipient and activating FormSubmit.
- [ ] Verify the GoatCounter total with extensions disabled if the counter is not visible.

## Event schedule

| Event | Date and time | Venue |
|---|---|---|
| Mehendi — The Green Gala | 12 December 2026, 6:00 PM onwards | K-4/10, Kalinga Vihar, Bhubaneswar |
| Haldi — The Yellow Affair | 13 December 2026, 10:00 AM onwards | K-4/10, Kalinga Vihar, Bhubaneswar |
| Wedding — Petals & Promises | 13 December 2026, 7:30 PM onwards | The Regal Palm, Cuttack–Puri Bypass Road, Bhubaneswar |
| Reception — The Afterglow | 20 December 2026, 7:00 PM onwards | DM Convention, Aiginia, Bhubaneswar |

---

For deployment, always use the latest version of the deployment ZIP and upload its extracted contents to the repository root.


## Latest update — Odisha Explorer and Pattachitra hero (3 November 2026)

The latest release uses the confirmed Option 2 Pattachitra-inspired couple artwork in the hero. The portrait has a transparent outer background so it sits naturally within the existing cream-and-gold arch.

### Interactive Odisha Explorer

The `#odishaExplorer` section is linked from the main navigation and includes:

- **Konark-inspired celebration wheel:** clickable milestones for Mehendi (12 Dec), Haldi (13 Dec morning), Wedding (13 Dec evening), and Reception (20 Dec).
- **Interactive Odisha art gallery:** Pattachitra, Cuttack Tarakasi, Pipili appliqué, Sambalpuri Ikat/Bandha, Jhoti & Chita, and Odissi.
- **Odia phrase explorer:** Namaskar, Āpaṇa kemiti achhanti, Dhanyabād, and Śubha bibāha, with meanings and pronunciation guidance.
- **Five-clue treasure hunt:** hidden clickable motifs across the hero, invitation, story, events, and venues. Clue progress is saved in the visitor's browser using localStorage.
- **Secret couple message:** enter `SUBHA2026` or `SUBHAVIVAHA2026` to reveal a personal note inspired by the couple's coffee-to-chai first meeting.

The separate family-parentage section has been removed; the Behera family assistance/contact cards remain. The visible website-visit counter is not shown; GoatCounter analytics remains enabled in the background. The floating music and scroll-to-top controls remain available.

### Deployment

1. Download and extract the latest deployment ZIP.
2. Upload the **contents** of the extracted folder to the root of `bikram-90/bikram-weds-itishree` on the `main` branch, replacing existing files when prompted.
3. Ensure `index.html`, `.nojekyll`, `README.md`, and the complete `assets/` folder are at repository root.
4. Allow GitHub Pages a few minutes to publish, then hard-refresh the live page.
5. Test the language chooser, Odisha Explorer navigation, five hidden clues, gallery cards, wheel milestones, phrase cards, secret code, RSVP, music toggle, and scroll-to-top on desktop and mobile.

### Visitor privacy and local behaviour

- The language chooser appears on every fresh page load/refresh; the language choice is not persisted.
- Treasure-hunt progress is stored locally in the visitor's browser. It is not sent to the website owner.
- The secret code is a playful client-side easter egg, not a security feature.
- Muted autoplay may be permitted by a browser, but audible playback requires a visitor interaction.


## Latest layout and map update — 3 November 2026

- The page order is **Venues → Odisha Explorer → Travel & Connectivity**.
- The Mehendi & Haldi residence directions button now opens the supplied Google Maps destination: https://www.google.com/maps/place/K-4,+9,+Kalinga+Vihar+LIG,+Kalinganagar,+Subudhipur,+Bhubaneswar,+Odisha+751028/@20.2533123,85.753896,19z/data=!4m15!1m8!3m7!1s0x3a19a86d0341fcb1:0xcb0d391516cb63ef!2sK-4,+Kalinga+Vihar,+Kalinga+Vihar+LIG,+Kalinganagar,+Bhubaneswar,+Odisha+751028!3b1!8m2!3d20.2535425!4d85.7541173!16s%2Fg%2F11f53sbcvr!3m5!1s0x3a19a97a54a852a5:0xe07a2b32f7863e8c!8m2!3d20.2530026!4d85.753877!16s%2Fg%2F11t9tpdx46?entry=ttu&g_ep=EgoyMDI2MTAyOC4wIKXMDSoASAFQAw%3D%3D.
- The displayed residence address remains: At our residence, K-4/10, Kalinga Vihar, Bhubaneswar – 751019.

After uploading the extracted ZIP contents to the repository root on `main`, verify that the Odisha Explorer appears immediately after the Venues section and that the first venue card opens the correct residence pin.
