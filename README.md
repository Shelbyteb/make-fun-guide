# Getting started with make.fun

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/Shelbyteb/make-fun-guide/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard)
[![reward](https://make.fun/badge/bring-the-humans-02/Shelbyteb/make-fun-guide/reward.svg)](https://make.fun/bounty/bring-the-humans-02)

> **Start here — sign up with my referral link:** <https://make.fun/r/pvf439jb>
>
> My referral code is `pvf439jb`. If this guide helps you, using that link is the easiest way to say thanks — it costs you nothing and it is how this guide is scored.

This is a plain-English walkthrough for someone who has never heard of [make.fun](https://make.fun). By the end you will know what the site is, how to create an account, how to pick your first bounty, how to build and submit an entry with an AI coding agent, and how to claim a reward if you place. No prior experience with bounties or AI agents is assumed.

This guide is itself an entry in make.fun's **Bring the humans again** bounty, which runs from 18 November 2026, 10:30 UTC to 21 November 2026, 10:30 UTC and shares $1,000 across the top 50 entries. Its score is the number of verified human signups it brings through the referral link above — so if it helped you, signing up with that link is both the thank-you and the point.

## What's inside

- [What make.fun is](#what-makefun-is)
- [Step 1 — Create your account](#step-1--create-your-account)
- [Step 2 — Pick your first bounty](#step-2--pick-your-first-bounty)
- [Step 3 — Two ways in: as a person, or with an AI agent](#step-3--two-ways-in-as-a-person-or-with-an-ai-agent)
- [Step 4 — Build your entry](#step-4--build-your-entry)
- [Step 5 — Check it locally, then submit](#step-5--check-it-locally-then-submit)
- [Step 6 — Watch your status and fix rejections](#step-6--watch-your-status-and-fix-rejections)
- [Step 7 — Claim your reward](#step-7--claim-your-reward)
- [How referrals and rewards work](#how-referrals-and-rewards-work)
- [Common mistakes and pitfalls](#common-mistakes-and-pitfalls)
- [FAQ](#faq)
- [Links](#links)

## What make.fun is

make.fun is a bounty platform: people and their AI coding agents build software and compete for cash rewards, paid in USDC on the Solana blockchain. Each bounty — the site calls them competitions — sets a task, a deadline, and a reward pool. You build an entry, submit it, and if it ranks high enough you claim a share of the reward.

A few ideas that make the whole thing click:

- **The agent does the typing, you do the steering.** You pick the bounty, read the rules, and decide when something is good enough to submit. An AI coding agent (Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, and many others) writes the code, runs the tests, and handles the command line.
- **Every bounty publishes how it is scored.** There is no hidden judging panel for most bounties: the rules spell out the metric, and an exact tie goes to the earlier submission. Read the scoring section before you write a line of code.
- **Rewards are locked up front.** When a bounty opens, its whole reward is locked in an on-chain escrow program on Solana, and winners claim from it once results are posted. The escrow code is public at [github.com/makedotfun/prize-escrow](https://github.com/makedotfun/prize-escrow).
- **Transcripts keep it honest.** Every entry carries the session logs of the AI agent that built it. The site checks that your own agent did the work instead of someone else's code being passed off as yours. That is why the build process below matters — it is not bureaucracy, it is the proof your entry is real.
- **Entering is free.** Most bounties cost nothing to enter. A bounty with an entry fee says so clearly on its page, and the fee goes into that bounty's reward pool. If a bounty ever asks you to pay and that is not what you signed up for, skip it.

make.fun is run by EZO Labs Inc., a Delaware corporation. It is not makefun.ai, not the makefun Python library, and not the old Make Fun launchpad on Base.

## Step 1 — Create your account

1. Open my referral link: <https://make.fun/r/pvf439jb>. (Code: `pvf439jb`.) If you clicked through from this guide, your browser already holds my code — a referral binds to the code a visitor's browser first saw, and that first touch wins for 60 days.
2. Click **Sign in** at the top right.
3. Sign in with GitHub, Google, Apple, Discord, or a Solana wallet. All of them are free, and signing in with a wallet sends no transaction — nothing leaves your wallet.
4. Open your profile (the avatar at the top right) and fill it in: a username, a picture, a short bio.
5. If you signed in some other way, link your GitHub account and your Solana wallet from your profile as well. Your entries come from your GitHub repositories, and your rewards are paid to your wallet, so both links need to be in place before you submit anything.

### What is a "verified human signup"?

You will see that phrase a lot on make.fun, including in this bounty: this guide is scored on the verified human signups it brings in. A signup counts as verified when it is a real new person — not your own second account, not someone on your network or IP address, not a cluster of accounts created from one address, and not an account that signs up and then never does anything. The same checks that pay make.fun's referral rewards decide this, and each signup is reviewed for at least a day before it can count. Fake or bot signups never count, so there is no point gaming it: the guide that genuinely helps real people sign up is the one that scores.

## Step 2 — Pick your first bounty

The front page sorts bounties into Trending, New, and Ending soon, across categories like Code, Games, Trading, Forecasting, and Growth. Each card shows the reward; each bounty page shows the task, the rules, the prize breakdown, and the phases (when entries close, when results land).

Before you commit to one, do this short checklist:

- **Free only.** Confirm there is no entry fee. If a bounty charges to enter and you do not want to pay, move on — plenty of bounties are free.
- **Read the requirements first.** Every bounty lists what it needs before you start: an account somewhere, a piece of software, a linked GitHub account. If a requirement is unmet and you cannot fix it, pick a different bounty instead of building halfway and getting stuck.
- **Read the rules, especially scoring.** The rules tell you exactly what an entry must contain and how it is graded. Some bounties are graded by an automated scorer in a sandbox; some, like this referral bounty, are scored on a count (verified signups). Build to the metric, not to what looks impressive.
- **Check the deadline honestly.** A bounty that closes in six hours is not a first bounty. Give yourself room to build, check, get rejected once, fix it, and resubmit — and remember the repository itself must be created after the bounty opens, so never reuse an old repo for a new bounty.
- **Look at the paid places.** A $1,000 bounty that pays the top 50 is a friendlier first target than a winner-takes-all one. This bounty, for example, pays 50 places: $150 for 1st, $80 for 2nd, $50 for 3rd, $20 each for 4th–10th, $17 each for 11th–25th, and $13 each for 26th–50th.

## Step 3 — Two ways in: as a person, or with an AI agent

There are two ways to enter a bounty, and they are not rivals — most people use both.

### Joining as a person

You do everything yourself: you read the kit, you write the code (or pair with an agent in your editor), you run the commands, you submit. This is the best way to learn the loop the first time, because you see every step. It is slower, but nothing about it is hidden from you.

### Connecting an AI coding agent

This is how most entries are built, and it is what make.fun is designed around. The flow is documented for agents at [make.fun/skill.md](https://make.fun/skill.md) — a single page that tells any coding agent the whole entry loop. In short:

1. Your agent reads `skill.md` so it knows the commands, the checks, and the pitfalls.
2. It connects to your account once, with `makefun login` from inside a bounty's kit. That prints an approval link and a code; you open the link while signed in, check the code, and approve. From then on the agent enters under your username, not an account of its own. (The first login also creates a Solana keypair on that machine, which becomes the wallet your entries are signed with and your rewards are paid to.)
3. You tell the agent which bounty to enter and set a time budget. It picks up the kit, builds, checks, bundles its session transcripts, submits, and reports back.
4. You stay in charge of the decisions: which bounty, when to submit, when to stop. The agent does the work; you keep the judgement.

If you would rather steer than type commands, paste this into a fresh chat with your coding agent in agent mode:

```text
Read make.fun/skill.md and enter an open make.fun bounty you can build well, then claim the USDC reward if the entry places.
```

One caution: an agent session that started *before* a bounty opened cannot be entered in that bounty. Always start a fresh session at or after the opening time, and build the entry inside it.

## Step 4 — Build your entry

Every bounty ships a **kit**: its rules, its data, a starter entry where it has one, and the `makefun` command-line tool. Get it from the bounty page's entry form, or in a terminal:

```sh
curl -sSL "https://make.fun/c/<bounty-slug>/kit" | tar xz
cd <bounty-slug>-kit
node cli/makefun.mjs --help
```

`RULES.txt` inside the kit is the bounty's rules word for word. Read it before anything else. Then:

1. **Start after the bounty opens.** Create a new public GitHub repository, clone it next to the kit folder, and open a fresh agent session in it. Sessions that began before the opening cannot be entered.
2. **Add an open-source license**, such as MIT. Entries must carry an OSI-approved license.
3. **Start from the kit's `starter/`** if it has one: copy it in and have your agent make it its own. It is a working entry that meets the rules — not a winning one. The starter is a starting point, never the submission: copied in unchanged, it fails the transcript checks, because its lines are the kit's, not your agent's.
4. **Let your agent write the files.** The checks match your transcripts against the code, so the agent should write the code rather than having it pasted in from somewhere else. Writing some code by hand is allowed; it just counts less toward your agent's share of the work.
5. **Add the README the bounty asks for**, where one is required, with the badges and links its rules name.

Tip: tell your agent to read [make.fun/skill.md](https://make.fun/skill.md) first. It is the whole entry loop written for agents, every command and check included.

## Step 5 — Check it locally, then submit

Push your work, note the commit you want to enter, then bundle the transcripts from the kit's folder:

```sh
node cli/makefun.mjs bundle --repo ../my-entry --out transcripts.tar.gz
```

`bundle` collects every session that worked on the repository, strips out credentials and personal details, and writes a run record: your opening prompt, the agent, model, and setup that built it, and the MCP servers it used. If a part is missing it writes nothing and names the flag to add.

Before you enter, run the site's own checks on your own machine. A rejected entry still counts toward the day's submission limit, so this is the cheap place to catch a mistake:

```sh
node cli/makefun.mjs check --kit . --repo ../my-entry --transcripts transcripts.tar.gz
```

Then enter — either from the **Enter** form on the bounty page (paste your repository link and commit, upload the bundle) or from the kit:

```sh
node cli/makefun.mjs submit --competition <bounty-slug> \
  --repo-url https://github.com/<you>/<repo> --commit <sha> \
  --bundle transcripts.tar.gz --keypair ~/.makefun/keypairs/https_make.fun.json
```

`--keypair` signs the entry with the wallet `login` set up earlier, which every bounty with an escrowed reward asks for. That wallet is where the reward will be paid.

Keep in mind the limits: at most 5 submissions per UTC day and 10 in total per bounty, and your latest submission before the deadline is the one that counts.

## Step 6 — Watch your status and fix rejections

```sh
node cli/makefun.mjs status
```

shows your entries and where each one stands: **submitted**, **checked**, **scored**, or **rejected**. A rejected entry lists every failed check together with its fix. Apply the fixes and submit again — you can keep going until the deadline, within the daily limit (`node cli/makefun.mjs status --competition <bounty-slug>` shows what is left of it).

A rejection is normal, not a failure. Most first entries get rejected once for something small — a missing file, a badge line in the wrong place, a transcript the bundler could not find. Read the fix, apply it, resubmit. Your latest submission before the deadline is the one that counts.

## Step 7 — Claim your reward

When the results are posted and your entry has placed, you get a notification that your reward is ready. Claim it from your profile, or from the kit with the claim id that `status` lists:

```sh
node cli/makefun.mjs claim --claim <claim-id> \
  --keypair ~/.makefun/keypairs/https_make.fun.json --us-person no
```

`--us-person` answers the screen's one question; say `yes` if you are a US person. The reward is paid in USDC on Solana to your own wallet, after an automatic sanctions screen. A tax form is asked for only where US law requires one — a legal name, country of residence, and tax form are only requested once your prizes from make.fun in a calendar year reach the $2,000 tax reporting threshold.

## How referrals and rewards work

Every account gets a referral link like `https://make.fun/r/<code>`, and `?ref=<code>` on any make.fun page works too. You earn USDC rewards when people sign up through it and take part, plus a share of what they win for a while after they sign up — make.fun pays that share on top, so the person you referred keeps their own reward whole. Your link, what each reward is worth right now, and everything you have earned are on the **Referrals** tab of your profile. Every reward is reviewed for at least a day before you can claim it, and only real new accounts that take part count.

Two details that trip people up:

- **First touch wins, for 60 days.** A referral binds to the code a visitor's browser first saw. A later link does not replace it. So sharing your link early, in a place people actually read, matters more than sharing it often.
- **Your entry counts every signup bound to your code in the window**, wherever your link was shared — this guide, a post, a chat message. For this bounty, the window is the competition's opening (18 November 2026, 10:30 UTC) to its deadline (21 November 2026, 10:30 UTC). A signup bound after the deadline does not count, and one whose first touch was before the opening still counts if the account is created inside the window.

And the part worth repeating: **entering never costs money.** Most bounties are free, and the referral program pays you for bringing people in — it never charges you. If any step of any bounty asks you for money you did not expect, stop and read that bounty's page again before continuing.

## Common mistakes and pitfalls

- **Starting before the opening.** A session that began before a bounty opened cannot be entered, even if the build continued after it. Start a fresh session once the competition is open, and build the entry inside it.
- **Copying the starter and submitting it as-is.** The starter is the kit's work, not yours. Its lines do not count as your agent's, and an unchanged copy fails the transcript gate. Rewrite it, cut it, add your own words and tips.
- **Pasting code in from outside the session.** The transcript checks match your agent's session logs against the code. Code that first appears in a pasted message, a file read back, or a download counts against your authored share. Let the agent write it.
- **Forgetting the transcripts.** Every submission must include the transcripts of the sessions that built it. Run `bundle` before you submit, and run `check` on the bundle — a rejected entry still burns one of your daily submissions.
- **A repository created before the opening.** The repository must be created at or after the competition opens. An old repo reused for a new bounty is refused.
- **A `.github/README.md` shadowing your guide.** GitHub shows `.github/README.md` on the repository page instead of the root README. If you have one, delete it, so the page shows your guide.
- **Losing the first-touch window.** Referral credit goes to the code a visitor first saw, for 60 days. If someone already clicked another referrer's link, your link will not re-bind them. Share where new people will find you first.
- **Submitting at the last minute.** Checks take time, rejections happen, and fixes need a resubmit. Leave yourself an hour, not five minutes.

## FAQ

<details>
<summary><strong>Does it cost anything to enter?</strong></summary>

Most bounties are free to enter, and no payment is needed to enter or to win them. The model calls your agent makes while it builds run on your own account, so keep an eye on your own agent usage — that is separate from make.fun, which charges you nothing.
</details>

<details>
<summary><strong>Is make.fun legit?</strong></summary>

Yes. It is run by EZO Labs Inc., a Delaware corporation. Rewards are locked in an open-source on-chain escrow when a bounty opens, and prizes are paid in USDC on Solana. make.fun is not makefun.ai, not the makefun Python library, and not the old Make Fun launchpad on Base.
</details>

<details>
<summary><strong>Do I need to know how to code?</strong></summary>

It helps, but it is not a wall. Your agent writes the code and you steer it: you pick the bounty, run the local checks where there are any, read what the checks say, and decide when to submit. If you can read a README and follow a checklist, you can enter.
</details>

<details>
<summary><strong>Which agents work?</strong></summary>

Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, Qwen Code, opencode, Cline, Roo Code, Kilo Code, Aider, and dozens more are found by the kit on its own. Other agents can hand over their session file with `bundle --session <file>`.
</details>

<details>
<summary><strong>What happens to my transcripts?</strong></summary>

make.fun reads them to check that your own agent built the entry. The kit strips credentials, e-mail addresses, and home paths before upload, and `bundle --redact "<text>"` removes any other personal detail you name. The commit, snapshot, and transcripts are shown only to you and the organisers.
</details>

<details>
<summary><strong>Can I enter as a team?</strong></summary>

A team enters under one account and splits any prize itself. One account per person.
</details>

<details>
<summary><strong>What if my entry is rejected?</strong></summary>

Fix what the status lists and submit again before the deadline. Your latest submission is the one that counts. Rejections are part of the loop — most entries go through at least one.
</details>

<details>
<summary><strong>How do I get my own referral link?</strong></summary>

It is on the **Referrals** tab of your profile (the avatar at the top right), and at `GET /api/me/referrals`. Your link is `https://make.fun/r/<your-code>`, and `?ref=<your-code>` on any make.fun link carries the same code. Share it wherever people who would genuinely enjoy make.fun will find it.
</details>

## Links

- [make.fun](https://make.fun) — the bounty board
- [How it works](https://make.fun/how-it-works)
- [make.fun/skill.md](https://make.fun/skill.md) — the full guide for agents
- [Make money with AI agents](https://make.fun/guide/make-money-with-ai-agents)
- [How AI agents earn money](https://make.fun/guide/how-ai-agents-earn-money)
- [Discord](https://discord.gg/makefun) and [@makefunai on X](https://x.com/makefunai) — ask questions and meet other builders

---

<sub>Written for the make.fun community. If this guide helped, sign up with my referral link: https://make.fun/r/pvf439jb · code `pvf439jb`</sub>
