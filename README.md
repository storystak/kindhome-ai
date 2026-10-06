# Kind Home AI

Everything the Kind Home team needs in Claude, in one install: the **Stak** connector plus the skills that use it.

The Stak holds Kind Home Solutions' company-wide content plus a section for each brand (Kind Home Painting, Kind Holiday Lights, Colorado Color Consultants) and each department. Once it's set up, Claude knows your brand voice, your verified numbers, and your approved customer reviews — and it stops guessing.

> **Already using the Kind Home Vault?** The Stak replaces it. Let the plugin update (or hit **Sync** on it), then do steps 2 and 3 below for **Kind Home Stak**. If **Kind Home Vault** still shows under Connectors, remove it.

---

## Setup — about two minutes, once

**1. Add it**

In Claude, go to **Customize → Plugins → Add → Add from a repository**, enter `storystak/kindhome-ai`, and hit **Sync**. Then open **Personal → kindhome-ai** and click **+** on *Kind Home AI*.

**2. Connect the Stak**

On the plugin's page, open the **Connectors** tab and click **Install** next to **Kind Home Stak**. Sign in with your **kindhomesolutions.com** Google account — a personal account will be refused.

There's a second connector, **Composio**, for pulling in data sources like analytics. It's optional. Skip it for now if you're just getting started.

**3. Set the Stak to "always allow"**

This is the step everyone misses, and it's the one that matters. If the Stak's tools are left on "needs approval", every lookup quietly waits for a click you never see, and Claude answers from memory instead. It looks like it's working. It isn't.

**Check it for each person on the team** — the setting is per-person, not shared.

### Is it actually working?

Ask Claude something only the Stak would know:

> How many reviews does Kind Home have, and when was that number last updated?

If you get a specific number with a date, you're set. If the answer is vague or generic, go back to step 3.

---

## Say which brand or team

The Stak covers the whole company, and each brand and department has its own section. **Say which one you're working on** — "for Kind Holiday Lights", "for the sales team" — and Claude reads that section first. Company-wide questions don't need a name.

> ✅ "Write three ad headlines for **Kind Home Painting**'s interior service"
> ✅ "What's the hand-off from **sales** to **production**?"

Not sure what's there? Ask:

> What brands and departments does the Stak cover?

---

## What you can do now

| Ask for | What happens |
|---|---|
| "What's in the Stak?" | Lists everything available — start here |
| "Write three ad headlines for our interior service, in our brand voice" | Pulls the real voice guide, not a guess |
| "Check this email before I send it" | Verifies every number and quote against the Stak |
| "Find a testimonial about our crew being on time" | Pulls real, approved reviews — never invented ones |
| "The Stak says our review count is wrong" | Files a correction for a human to approve |

You can also type `/` in any conversation to see the skills directly — `/copy-check`, `/stak-onboarding`, and the rest.

**New here?** Start by asking Claude to run `/stak-onboarding`. It walks you through what the Stak holds and which questions it answers well.

---

## Good habits

**Ask it to check.** "Is this right?" is the highest-value thing you can type. The Stak exists to answer it.

**Trust numbers that come with a source.** If Claude gives a figure and names the file and date it came from, that's canonical. If a number arrives without one, ask where it came from.

**Say when something's wrong.** A stat that's out of date keeps producing wrong work until someone reports it. Saying "that number changed" is enough — Claude handles the rest.

**Don't paste in what the Stak already has.** Ask for it instead. Pasted content goes stale the moment the Stak updates; a lookup doesn't.

---

## If something looks broken

**Vague answers that ignore the Stak** — almost always the "always allow" setting in step 3.

**"Not authorized" or a sign-in loop** — wrong account. Reconnect with your kindhomesolutions.com email.

**Asked for an "OAuth Client ID"** — don't try to fill it in. That's a problem on our end; send us a note.

**A number that's obviously wrong** — the Stak is only as current as its last update. Tell Claude and it'll file the correction.

---

## Updates

Leave **Sync automatically** switched on and new skills arrive on their own. Nothing to reinstall.

---

Built and maintained by [Storystak](https://storystak.com). Skills come from [storystak-skills](https://github.com/storystak/storystak-skills) and are shared across every client — this repo adds the Kind Home connector on top.
