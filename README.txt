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

VISITOR COUNTER SETUP (ONE-TIME)
The site includes GoatCounter analytics and a total-visits counter. A GoatCounter site code must be registered before the public counter can display a real number:
1. Sign up at https://www.goatcounter.com/signup
2. Use the account/site code `bikramwedsitishree` if available (the page is configured for this code).
3. Add the GitHub Pages domain as the site domain if prompted.
4. In GoatCounter site settings, enable “Allow adding visitor counts on your website”.
5. Publish/redeploy this ZIP. The footer then displays the total visits. If the site code is unavailable, change GOATCOUNTER_ENDPOINT in index.html to your assigned `https://YOURCODE.goatcounter.com/count` endpoint.

MUSIC AUTOPLAY
The embedded YouTube player attempts autoplay muted. Browsers generally block audible autoplay until a visitor interacts with the page; use “Tap to enable sound” in the player or the music control in the navigation. The Open on YouTube link is a fallback if the embed is blocked or the network prevents playback.

CHECKLIST AFTER DEPLOYMENT
- Check all four event images on desktop and mobile.
- Switch to Odia and confirm every section, button, form field, option, and helper message changes.
- Submit one RSVP test and verify both WhatsApp draft and email receipt.
- Confirm the GoatCounter visit total is visible after its setup is complete.
- Confirm Maps and Google Calendar links open the intended venues/events.
