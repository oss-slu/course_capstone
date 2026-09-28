---
title: 'Onboarding: Commit Identity'
points_possible: 0
due_at: '2026-09-30T21:00:00Z'
submission_types:
- online_text_entry
published: false
assignment_group: "Assignments"
grading_type: pass_fail
---

# Overview

Git stamps every commit with a name and an email address. GitHub shows a commit as yours only if that address is registered to your account. Your work is still in the repository if your registered address is not configured in the commit, but it appears under no name at all.

Today you will choose the identity you want on your professional work, configure it, and confirm it works. It takes about ten minutes.

## What you will do

1. Check what git is currently configured to use.
2. Check whether your existing commits are attributed to you.
3. Choose the email address you want on your professional work.
4. Configure git to use it.
5. Make a commit and confirm it attributes correctly.
6. Repeat the configuration on every machine you commit from.
7. Write a short reflection and submit.

Details for each step follow. Background and reasoning are in [Documentation](#documentation), which you do not need in order to finish.

---

# Activity

**1. See what git is set to right now.**

```
git config user.name
git config user.email
```

If the address ends in `.local`, git invented it from your computer's hostname and it belongs to no account anywhere.

**2. See whether your past commits attributed.**

Open your team's repository on GitHub and find a commit you made. Your avatar beside it and your username linking to your profile means it worked. A plain name with no link means the commit is connected to no account.

Note what you find. You will refer to it in step 7.

**3. Choose your address.**

The recommended choice is your GitHub noreply address. Find it at [github.com/settings/emails](https://github.com/settings/emails), under "Keep my email addresses private." It looks like `12345678+yourusername@users.noreply.github.com`.

If you would rather use your SLU or personal address, read [Choosing your address](#choosing-your-address) first, then add it to your account on that same page.

**4. Configure git.**

```
git config --global user.name "Your Name"
git config --global user.email "your-chosen-address"
```

The name is what you want associated with your professional work. It does not need to match your GitHub username and has no effect on attribution. Only the address does.

**5. Make a real commit.**

You need a commit to verify against, so make one that is worth having. Some options, in rough order of preference:

- Add yourself to your repository's `CONTRIBUTORS.md`. If your team does not have one, create it and add yourself as the first entry.
- Fix something small and genuine in the README or setup documentation, particularly anything that tripped you up during onboarding.
- Any other minor improvement you have been meaning to make.

Push it, then find that commit on GitHub and confirm your avatar appears and your username links to your profile. If it does not, the address in the commit is not registered to your account.

**6. Repeat on every machine you commit from.**

A lab computer, a personal laptop, and a desktop at home are three separate configurations, as is any machine you start using later in the term. Configure the ones you have access to now, and make a plan for the rest.

**7. Reflect, then submit.**

Submit these three lines, followed by a few sentences.

```
Commit: <URL of the commit you verified>
Email: <the address you configured>
Machines: <how many machines you commit from>
```

For example:

```
Commit: https://github.com/oss-slu/example-repo/commit/a1b2c3d4e5f6
Email: 12345678+jdoe@users.noreply.github.com
Machines: 2
```

Please keep that format, since it is read by tooling. The machine count tells us who needs more than one address recorded. If your machines are not configured the same way, say so and we will record each one.

Then write three to five sentences responding to these:

- What was your git identity set to before today, and had you ever chosen it?
- Which address did you settle on, and what decided it for you?
- Which machines still need configuring, and how will you remember to do them?

If something blocked you, submit what you completed and describe what stopped you.

## Requirements

Required, not graded. There is no rubric and no evaluation.

## Bonus, if you finish early

Neither of these is required or part of the submission. Mention them if you do them.

**Polish your profile.**

Your GitHub profile is often the first thing someone looks at after your resume. Attribution puts your work on it. These make it worth looking at.

- **Set a profile photo.** An account with the default avatar is hard to recognize in a commit history or a long pull request thread. It does not need to be a formal headshot, but it should be identifiable as you and consistent across the places you use it.
- **Put your real name in the display name field.** People search for you by name, not by username.
- **Write a one-line bio.** What you work on, and where.
- **Create a profile README.** Make a repository named exactly the same as your username. Its README renders at the top of your profile page. This is the highest-signal item on the list, and most people do not know it exists.
- **Pin your best repositories.** You decide what a visitor sees first. Your team project belongs there.
- **Add a link.** A portfolio, LinkedIn, whatever you want people to find next.

The commits you fixed today also begin filling in your contribution graph. People do look at it, and it only reflects work attributed to your account.

**Sign your commits.**

Configuring your identity states who authored a commit. It does not prove it, since anyone can set `user.email` to any value. Signing attaches cryptographic proof, and GitHub marks commits it can verify.

SSH signing is the simplest approach, and it reuses the key you already use to push:

```
git config --global gpg.format ssh
git config --global user.signingkey ~/.ssh/id_ed25519.pub
git config --global commit.gpgsign true
```

You then add the same public key to your GitHub account a second time as a signing key, at [github.com/settings/keys](https://github.com/settings/keys). Authentication keys and signing keys are registered separately, which is the step people usually miss.

---

# Documentation

Background and reasoning. You do not need any of this to complete the activity.

## How git and GitHub relate

Git and GitHub are separate systems that meet at a single point.

Git runs on your machine. It records a name and email address on every commit, read from that machine's configuration at the moment you commit. It does not verify those values and it does not contact GitHub.

GitHub is an account system. Your account has a username, credentials, and a list of email addresses registered to it.

The connection between them happens when GitHub displays a commit. It reads the email address git recorded, then looks for an account with that address registered. If it finds one, the commit appears as yours. If it does not, the commit is still valid and still in the repository. It is simply linked to no one.

Two things follow from this, and both are useful:

- **An account can have several addresses registered to it.** A commit using any of them attributes to you. This is what makes it workable to commit from a work machine, a personal machine, and GitHub's web editor without all three being configured identically.
- **Each commit records whatever identity was configured at the time.** Git reads the configuration fresh on every commit, so a repository with a local override, or a machine you set up in November, will produce commits under a different identity with no warning.

## Why this matters

Your commit history is a public professional record. It accumulates while you work, and it is difficult to reconstruct afterward.

Whether a commit becomes part of that record depends entirely on the address it was made with. Repository access and organization membership play no part in it. You can push a commit, have it reviewed, have it merged, and still have it attributed to nobody. Nothing in the process tells you so.

The sprint summary you receive counts commits, so this affects the feedback you get. That is the smaller reason. The larger one is that when someone looks at your GitHub profile in a year, they see the work connected to your account and nothing else.

## Choosing your address

You have three reasonable options.

| Option | Example | Attribution | What it publishes |
| --- | --- | --- | --- |
| GitHub noreply address | `12345678+yourusername@users.noreply.github.com` | Always works. The address belongs to your account by definition. | Nothing. |
| Your SLU address | `you@slu.edu` | Works once you add the address to your GitHub account. | Your university address, in every commit, permanently. |
| A personal address | `you@example.com` | Works once you add the address to your GitHub account. | A personal address, in every commit, permanently. |

Two things to weigh.

Consider what you are willing to have permanently public. A commit address is not retractable. It remains in the repository history and in every clone anyone has made of it.

Consider also how portable the address is, and how long it will keep reaching you. Your SLU address is yours for life under university policy, so it will not stop working when you graduate. That cuts both ways, since publishing it is a longer commitment than it might appear. Most other institutions reclaim addresses after you leave, so this is not an assumption to carry to your next school or employer. The noreply address does not depend on a mailbox at all, which is one reason many open source contributors prefer it.

## Fixing earlier commits

If step 2 turned up unattributed commits, you can often repair them. Add the exact address those commits used to your GitHub account, and GitHub will connect them. You do not need access to that mailbox for this to work.

This will not work for an address that is not real, such as anything ending in `.local`. GitHub will not accept one. If your earlier commits used an address like that, say so in your submission and we will record it directly so the work is still counted.
