# HANDOFF: social posting for Ivy Cassel and Elif Kessler (written 2026-10-16, updated 2026-10-16 about 10:35 IST)

Read this first. It covers both repos: aliwaziri10/ivy-cassel-books and aliwaziri10/elif-kessler-books.

## Who and how to work with him
- The user is **Zia Waziri** (Z-I-A, W-A-Z-I-R-I). Voice-to-text garbles names; verify spellings. Pen name is **Elif Kessler** (with an E). Voice-to-text has produced Alif, Alex and "Elif Tesla"; all of those mean Elif Kessler. Always write it E-L-I-F.
- He wants **one step at a time**, and **every copyable item (URL, name, text) in its own code block** so it has a copy button.
- He gets frustrated when steps are skipped or guessed. Do not assume he has an account; ask. When he says "I created it", confirm exactly WHAT he created (the Gmail, the Instagram, or the Page); this caused a mix-up on 2026-10-16.
- Times are always given in IST (Indian time), never UTC or GMT.
- Memory is off on his Claude account, so nothing carries over except this file.

## Hard rules (from novels/FROZEN_DO_NOT_EDIT.md in aliwaziri10/Voxel, dated 2026-10-16)
- Never edit or push to any Kindling Line or Amity Falls folder in Voxel. Read-only.
- Two pen names, two separate reader promises. Never mix them or link them.
  - Ivy Cassel = romantasy, series The Kindling Line.
  - Elif Kessler = slow-burn small-town romance, series The Amity Falls Series (4 books, finished).
- The real repo is aliwaziri10/Voxel, NOT Wazzaboyzz/Voxel.
- Never ask him to paste tokens or keys in chat. They go only into GitHub repo secrets.
- Do not use fake Facebook profiles or fake birth dates. Everything is owned by his one real Facebook account (Zia Waziri); Pages carry the pen names.
- Keep the pen names separate from his real name: he chose NOT to invite his personal friends to the Elif Kessler Page.

## Books and links (links given by Zia; Amazon blocks automated reading, so titles were matched by ORDER, not verified)
Elif Kessler, Amity Falls: 1 Where the Frost Doesn't Reach https://a.co/d/0gndbYmd, 2 What the Valley Still Owes https://a.co/d/02KQnb51, 3 What the Blood Remembers https://a.co/d/0gKBZ0so, 4 The Secret She Kept Forever https://a.co/d/04fD8jSn
Ivy Cassel, Kindling Line: 1 Borrowed Years https://a.co/d/015rGBsc, 2 Keep Me Past the Fire https://a.co/d/0c839mM0, 3 Count Me Through the Dark (proofread, NOT yet published, shown as coming soon).
ACTION: ask Zia to click all 6 links and confirm each opens the right book.

## CONFIRMED done
- Both repos exist and are pushed: tools/make_queue.py, tools/poster.py, config.json, images/, queue/posts.json, queue/group_posts.md, SETUP.md, .github/workflows/post.yml (cron Tue/Thu/Sat 14:30 UTC) and build.yml. Ivy queue = 11 posts, Elif = 16. Dry run tested locally.
- **Facebook Page "Elif Kessler" is FINISHED (2026-10-16 about 10:15 IST).** Page address: https://www.facebook.com/profile.php?id=61595203121191 (the number 61595203121191 is the Page ID as read from the address bar; treat it as the likely FB_PAGE_ID but verify in Graph API Explorer). Category Author, bio, green "EK" profile picture, cover photo, all set. Setup choices: WhatsApp skipped, "invite friends" skipped (on purpose), Page notifications on his profile ON, marketing emails OFF.
- **Action button set: "Learn more" linking to the Book 1 link** (https://a.co/d/0gndbYmd). IMPORTANT: as the admin he does NOT see this button on his own view of the Page. It only shows in the public view. Checked in a private window: visitors see Learn more, Message and Follow. In the button list, "Learn more" sits under the group "Link to your group or app", so it is below the contact options and needs scrolling.
- Gmail account **elifkessler123@gmail.com** is created and belongs to Zia (he confirmed it; spelled E-L-I-F).

## IN PROGRESS: Elif Kessler Instagram account
- NOT created yet as of 2026-10-16 about 10:35 IST.
- Zia wants to control it from his existing Instagram login (ziawaziri@gmail.com), whose displayed account is **wazzaboyzz** ("Wazza Boys"). He was logged into instagram.com as wazzaboyzz in Chrome.
- Plan: from that login, add a NEW account through the account switcher (Add Instagram account, then Create new account). On the website this is under More (bottom of the left sidebar) then Switch accounts. Menu names may differ; ask what he sees.
- Details to use: email elifkessler123@gmail.com, full name Elif Kessler, username elifkessler.books (fallback elifkessler123). He picks the password himself and never pastes it in chat. Real birthday only. Instagram will email a confirmation code to the Gmail.
- Mix-up to avoid: he once landed on meta.ai (Meta's AI chat site) instead of Instagram. The Instagram address is https://www.instagram.com/

## NOT done (everything below is still to do)
1. Finish creating the Elif Kessler Instagram account (above). Then switch it to Professional (Creator), category Author. Then link it to the Elif Kessler Facebook Page (Instagram: Edit profile, Page, connect).
2. Meta developer app (developers.facebook.com), Graph API Explorer: permissions pages_manage_posts, pages_read_engagement, instagram_basic, instagram_content_publish. Get FB_PAGE_ID, FB_PAGE_TOKEN, IG_USER_ID. Make the token long-lived (verify on Meta's page). Add them as repo secrets in elif-kessler-books, then run the post-to-social workflow once.
3. The whole Ivy Cassel chain: he has NO Gmail for Ivy yet. Create one, then Instagram, then a Facebook Page "Ivy Cassel" (category Author), link them, then step 2 above for ivy-cassel-books. Then make profile and cover images (reuse the Elif method in warm red/gold #2b1210, #7a2e1f, #f2b36b).
4. Repos must be PUBLIC (Instagram fetches card images from raw.githubusercontent.com). Confirm.
5. Author websites: a generator was built (two static sites with schema markup, sitemap, llms.txt) and sent as book-sites.zip, but NEVER deployed. Optional later: add to the repos and enable GitHub Pages.
6. TikTok: not started. Posts go private until TikTok's audit passes (takes weeks). Skip until Facebook and Instagram work.

## UNVERIFIED (treat as hypotheses)
- Click-by-click Facebook/Instagram steps came from a third-party guide (Leadsie) and from third-party articles, not Meta's own help pages (those returned no step text). Meta's screens change; ask what he sees. Example: an early guess that "Learn more" had been removed from Facebook was wrong; it was just lower in the list.
- Whether Meta app review is needed for posting; the docs read did not say.
- Whether GitHub keeps scheduled workflows alive on a quiet repo. Check the Actions tab after a month.
- Amity Falls Book 2 blurb is thin (the notes in Voxel are archived stubs).
- Page ID 61595203121191 was read from a screenshot of the address bar.

## Tooling notes
- The GitHub connector can read repos it has access to, but its file-write tool returned 403 on elif-kessler-books and create_repository returns 403. Writes work by attaching the repo with add_repo (access: push), cloning it, and committing and pushing with git. New repos must be created by Zia on github.com/new first. Binary files (images) work through git, not through the file-upload tool.
- Plan is Free: no browser control, no computer control, no scheduled tasks. GitHub Actions does the scheduling.
- WebFetch cannot open a.co / Amazon links (robots disallow).
