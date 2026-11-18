# Training companion app – project rules

Read this before every change. These rules come from the client-approved build history.

## What this is
- A clickable prototype of a participant training app plus an admin area, in ONE self-contained file: `index.html` (inline CSS, JS and images as data URIs). Hosted on GitHub Pages.
- Fake data only. Nothing is saved. No backend/engine yet – do not add one.
- English only.

## Public repo – keep it generic
- This repository is PUBLIC. Never add anything confidential.
- ZERO client branding: no Audi names, colours, logos, fonts or product names.
- Use the generic names: Model A / Model B (Sport versions), new-engine-x, engine-y, Plus / Top trims, "Tokens", "Confidence check", "Program 2".
- Look: neutral slate-and-teal palette, slightly rounded corners, system font stack, drawn placeholder images.

## Working style
- Keep participant and admin screens as simple as possible. Short, plain screen text.
- Stay close to the existing look and flow. Don't redesign things that weren't asked for.
- Make the smallest change that does the job. Don't reformat or rewrite unrelated parts of the file.
- Before editing, summarise what you'll change. After editing, list what changed so the reviewer can check it.

## Layout
- Desktop gets its own layouts (Articulate 360 style), never a stretched phone layout.
- Sign-in and activity start pages: text panel + image side by side on desktop, stacked on phones.
- Reading content: centred column, about 880px wide.
- Tiles: 2 across on phones, 3 on tablets, 4 on laptops, then stop growing.
- Images are never cropped or stretched.
- Results screens never use a black background.

## Participant app
- Sign-in copies the current app: cover image + Sign-in button → name box + Enter → Welcome form (first name pre-filled, *Last name, *Dealership dropdown, Cancel / Enter). "Remember me" goes straight to Home.
- The main screen is called "Home" (not "All activities").
- All activities are always open: no access codes, no trainer unlocking, no QR/token join.
- Quizzes, after Submit: correct answer gets a green ✓; every wrong answer gets a red ✕ (including unpicked ones); only the picked answer gets an outline. No "Correct/Incorrect" text, no explanations.
- Hands-on activities: photos at full shape with Enlarge; square checkboxes labelled a), b), c); after each question a "More info" section (info icon, divider, points in light-grey boxes numbered 01, 02, 03).
- You vote: no class results shown after submitting.
- Close quiz: pass/fail at 80%.

## Admin
- Roles: Agency admin, Trainer, Client, Participant, with a "Viewing as" switcher. Trainers see only their own tour. Clients see no names and no tokens.
- Tours 1–5 switcher; each tour has its own link and QR code on Live class. The QR is not wired to the participant app.
- No "New link" button. No summary number tiles.
- Live class: "Element" list; Tokens row at the top with the leader and a Show scoreboard button; completion counts and Show results per activity.
- Content: each activity has its own page with the upload file, checks, preview, rollback, and its own Images section. Images auto-link by name or number; unmatched ones go to a "Link these images" list; every slot has Add / Replace.
- Users & roles page.

## Not built yet – don't add unless asked
- Dealer-list-to-tour mapping, client dashboard with weekly PDFs, real engine (Supabase / Cloudflare).
