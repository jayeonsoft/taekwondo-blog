---
title: 'Why Seoul Nights'
description: 'What this game is and why it exists: a browser taekwondo action game set in a neon Seoul alley district.'
pubDate: 'Oct 12 2026'
heroImage: '../../assets/blog/street-brawl.png'
---

Seoul Nights is a browser 3D action-adventure about a taekwondo student at a small dojang in a neon Seoul alley district — Hongdae/Itaewon vibes, hangul neon signs, pojangmacha tents, rain-wet asphalt. A street crew, the Dragon Gang, is leaning on local shops. You train, earn belts, and clean up the streets with taekwondo.

The tone is stylized and heroic on purpose: no blood, no gore. Defeated enemies drop, see stars, and flee. It's meant to feel like a sports-fantasy brawler, closer to a Saturday-morning action show than a grim beat-'em-up.

Mechanically it borrows from two places: the third-person street-brawler feel of something like *GANG OF DRAGON*, and the belt-progression / FLOW-meter / board-breaking / forms structure from an old game-design plan I'd sketched called *SMA: Black Belt Journey*. Belts (White → Yellow → Green → Blue → Red → Black) gate which techniques you can learn; a separate FLOW meter rewards clean hits, parries and combos with a growing damage multiplier; mastery tracks how many times you've actually landed each move in a real fight, independent of belt rank.

Everything you see running around is procedural — no external art files. Characters and props are Three.js primitives (capsules, boxes) with stylized materials; the only "art" is in how the geometry is composed and lit. Audio is procedural WebAudio too. It's a constraint that forces a particular look, and so far I like what it forces.

This blog is where I'll post devlogs as things ship: new moves, new chapters, new systems, and the occasional "here's why this was harder than it looked." The game itself is live at [taekwondo.jayeonsoft.com](https://taekwondo.jayeonsoft.com) — guest play works with no sign-up, and progress now syncs to the cloud if you want it to.
