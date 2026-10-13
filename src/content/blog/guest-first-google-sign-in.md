---
title: 'Guest-first Google Sign-In: cloud saves without a login wall'
description: "Why sign-in had to stay optional, and how the save-conflict prompt works when two devices disagree."
pubDate: 'Oct 12 2026'
heroImage: '../../assets/blog/belt-progress.png'
---

Seoul Nights just got cloud saves, and the thing I was most careful about was *not* making that feel like a login wall. The game has always worked fully as a guest — no account, no email, just play — and that had to keep being true after shipping sign-in, not become true "unless you want your progress backed up."

So the entry points are opt-in and low-pressure: a status line and a button on the Player Page and in the Arena's Rankings tab, plus a one-time toast after your first belt promotion that offers to sign in if you haven't already. Dismiss it and it never comes back. Nothing about guest play changes — belt, coins, mastery, cosmetics, titles, secrets, boxing progress, all of it keeps working locally exactly as before.

The part that actually took the most thought wasn't the OAuth flow, it was what happens when sign-in finds *existing* cloud progress that doesn't match the device you're signing in from. Two devices, two different save states, one Google account — picking one silently is the wrong answer either way (you might lose your phone's week of boxing grind, or your desktop's belt progress). So that case gets its own prompt: load the cloud save, or keep this device's save and overwrite the cloud copy. No auto-merge, no "smart" heuristic — just an explicit choice with both options named.

Once you're signed in, syncing is quiet: the full save (not just a ranking name) mirrors to the cloud and keeps syncing automatically every few seconds as you play, backed by its own Durable Object so it can never collide with the leaderboard data. Sign out, and you keep playing on this device exactly as before — nothing is deleted, nothing stops working.

The belt-promotion toast nudge is deliberately the *only* nudge. If you never want an account, the game doesn't ask twice.
