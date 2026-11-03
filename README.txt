BIKRAM & ITISHREE — GITHUB PAGES DEPLOYMENT
Release prepared: 03 November 2026

FILES
- index.html: website entry point (keep at repository root)
- .nojekyll: prevents GitHub Pages from filtering asset paths
- assets/: local artwork, logos, and Odia decorative motifs

MANUAL DEPLOYMENT
1. Extract this ZIP.
2. Open https://github.com/bikram-90/bikram-weds-itishree
3. Confirm the main branch is selected.
4. Choose Add file > Upload files.
5. Upload the CONTENTS of this extracted folder (index.html, .nojekyll, README.txt, and assets/).
6. Commit directly to main.
7. In Settings > Pages, confirm Deploy from a branch / main / (root).
8. Check Actions for the Pages deployment, then visit:
   https://bikram-90.github.io/bikram-weds-itishree/

RSVP EMAIL DELIVERY
The RSVP form opens a WhatsApp message and submits the same message to the email endpoint using FormSubmit's AJAX service.
The first live submission may trigger a one-time activation email. Open the destination mailbox and confirm the FormSubmit request. Submissions are held until that address is confirmed.

IMPORTANT PRIVACY NOTE
The current recipient address in index.html is bikramwedsitishree@yopmail.com, preserved from the existing website configuration. YOPmail states that inboxes are public and password-free; anyone who knows the inbox name can read messages. Do NOT use this inbox for guest information you expect to remain private. Before launch, replace RSVP_EMAIL in index.html with a private mailbox that you control, then make the first test submission and confirm FormSubmit at that private mailbox.

VISITOR COUNTER (GOATCOUNTER)
The page uses:
- Tracking endpoint: https://bikramwedsitishree.goatcounter.com/count
- Script: https://gc.zgo.at/count.js
- Public counter path: TOTAL (GoatCounter's documented site-wide total)

In GoatCounter Settings:
1. Set “Your site” to https://bikram-90.github.io/bikram-weds-itishree/
2. Keep “Allow adding visitor counts on your website” checked.
3. “Dashboard viewable by” controls dashboard privacy; it does not prevent the public counter from displaying.
4. “Individual pageviews” can remain unchecked; GoatCounter says this does not disable aggregate analytics.

If the footer says “Check ad-blocker” or “Temporarily unavailable”, test in a private/incognito window with extensions disabled. Privacy/ad-blocking extensions may block gc.zgo.at or the GoatCounter domain. GoatCounter also caches public counter responses for up to four hours, so the displayed total may not update immediately.

MUSIC
The soundtrack starts muted where the browser permits muted autoplay. The single speaker icon at the bottom-right toggles mute/unmute. Browsers do not permit a website to force audible autoplay before user interaction.

CHECKLIST AFTER DEPLOYMENT
- Check all four event images on desktop and mobile.
- Switch to Odia and confirm every section, button, form field, option, and helper message changes.
- Submit one RSVP test and verify both WhatsApp draft and email receipt.
- Confirm the GoatCounter visit total is visible after its setup is complete.
- Confirm Maps and Google Calendar links open the intended venues/events.

LATEST UPDATE — 3 NOVEMBER 2026
- A language selection screen now appears whenever the website is opened or refreshed. Visitors choose English or Odia each time; the choice is not remembered between page loads.
- The English transliteration has been updated from “Shubha Bibaha” to “Subha Vivaha”.
