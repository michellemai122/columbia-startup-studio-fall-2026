# Gable backlog (ranked, Nov 20, 2026)

Ranked by one question: **what stands between a new visitor and the moment Gable is worth it to them** (typing what they want and seeing a short list of sublets that fit)? Our evidence is the three usability sessions (Nov 6, 10, 11), the changes we said we would make in `hw7-usability-testing/usability_synthesis.md`, and the first week of the Reddit ad test. Ad results are not in yet, so this ranking will be revisited when section 9 of the experiment card is filled in.

AI = a place where AI could help.

## 1. ⭐ Make "Sign up" the obvious path, and put the search first on the first page

- **What:** Anyone who is new should land in sign-up, not sign-in: the header "Log in" and the sign-in page should not be the first thing a new visitor tries, and the first page should be straight to the point, with the "what do you want" box first.
- **Why it is #1:** all 3 testers tried to sign in before they had an account, and 2 of 3 missed the chat search at first. Both happen before the aha moment, and the Reddit ad now sends every visitor through this exact path. The "Sign up to see your matches" step on search is already live (it is what we count as a signup), so this is the next thing that decides how many people get through.
- **Size:** small (copy and button order, no new data).
- **AI:** no.

## 2. "We'll look for it" request, when a search finds nothing

- **What:** When no sublet fits, show "We don't have that one yet", take their email and what they want, and promise an answer within 48 hours. We find matches by hand from our network.
- **Why:** all 3 testers said there are not enough listings. Today an empty search is a dead end; this makes it a lead, and tells us which places to go and find. It is built on a branch (`no-results-request` in the Gable repo) but not merged, and it needs an email service to reply automatically.
- **Size:** medium (merge, plus sending the reply email).
- **AI:** yes. AI can read the request, match it against listings and draft the reply we send.

## 3. Real supply: get the first 10 real listings from our network

- **What:** Ask students who are away this semester or summer to post their place with List your room. Make posting faster (clear photo guidance, an easy first step after sign-up) and ask new accounts "subletting your own place?" once.
- **Why:** supply came up in 3 of 3 sessions and is our biggest blocker. We decided not to scrape listing sites, so listings have to come from students.
- **Size:** medium (mostly outreach, some product).
- **AI:** yes. AI can pick the best cover photo for a listing (the first real listing leads with a bathroom photo) and tidy a lister's description.

## 4. One clear commute line on each listing card

- **What:** Replace the two or three travel lines ("Columbus Circle", "20 min to Times Square") and "Replies in ~3h" with one line: minutes to Columbia.
- **Why:** 2 of 3 testers did not understand them (one asked "Is that how far away it is?"). Our users are mostly Columbia students and care about campus.
- **Size:** small.
- **AI:** yes. The commute can be worked out automatically from the listing's address.

## 5. Re-test the new Messages with real people

- **What:** Run 3 to 5 sessions on the current site, with at least one stranger, focused on sign-up, the search box and sending a message to a lister.
- **Why:** we changed a lot since the first sessions (the sign-up step, hearts, photo gallery, in-app private messages, group chats), and in sessions 2 and 3 the old Messages screen was the most confusing part ("looks like WhatsApp, am I messaging the person renting it out?"). We have not checked whether the fix works.
- **Size:** small (a week of sessions).
- **AI:** no.

## 6. Sign in with Google

- **What:** A Google button on sign-up and sign-in.
- **Why:** it removes typing an email and password, which is where signups drop. Our first attempt failed and needs a retry.
- **Size:** medium. Lower than the items above because it only helps people who are already past the first page.
- **AI:** no.

## Not building (yet)

- **A "Why you can trust them" panel with vouches and LinkedIn or Instagram cards.** It is in the Messages design, but we have no real data for it (no vouches, no linked profiles), and no tester asked for it.
- **Payments or booking inside Gable.** We took booking out on purpose: renters and listers deal directly, and we tell people to see the place and the lease before they pay.
- **Scraping StreetEasy, Zillow or Facebook listings.** Their terms do not allow it, so supply has to come from students.
- **A native mobile app.** The web site works on a phone and we do not have the time.
- **More filters and map layers.** No tester got stuck on search itself; the problems were around it.
