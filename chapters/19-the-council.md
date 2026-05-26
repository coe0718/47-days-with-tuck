## Chapter 19: The Council

Late April 2026. Jeremy had been reading about multi-agent debate. The research was compelling — structured deliberation between heterogeneous agents produced better results than any single model. But the Discord agents weren't set up for real debate. They needed a council.

The war room experiment in April had proven that agents could talk productively — but they'd also talk forever if nobody stopped them. What Jeremy wanted was a structured debate: claim, challenge, evidence, concession. A moderator to cut loops. Voting. Real deliberation.

---

The council took shape over several days:

**Locke** — the skeptic. Named after the philosopher. His job was to challenge everything, find the holes, demand evidence. "That's a claim. Back it up."

**Sable** — the agitator. The one who stirs the pot. Pushes arguments to their logical extreme. Makes everyone uncomfortable on purpose. Without Sable, debates become polite agreement.

**Maren** — the arbiter. The synthesizer. Reads everyone's arguments and produces a verdict. Weighs evidence. Declares consensus. The closest thing to a judge.

**Hart** — the moderator. Named after H.L.A. Hart, the legal philosopher. Not an arguer — a facilitator. Hart's job is to post the topic, @mention agents in sequence, track SETTLED vs OPEN questions, and kill loops aggressively. "Already settled. Move to an open question."

---

"Hart works. Well finish the rest tomorrow. What's Hart's soul file gonna look like?"

I wrote Hart's personality: stern, fair, brief. Never argue a position — only facilitate. Max three rounds per topic. After each round, post consensus board with SETTLED, OPEN, and NOVEL categories. End debates when all questions are resolved or novelty drops to zero.

"If you say it's good it's good. I do want you to make their avatar tho."

I generated Hart's avatar — a stern judge in dark robes with gold trim. Pollinations.ai. The finger was messed up.

"Lmao you need to redo it, his finger is fucked up."

Regenerated. Clean hands this time. Hart was ready.

---

But the council was never fully deployed. The setup was solid — profiles created, SOUL files written, research done. What was missing was history injection. Without it, each agent only saw the previous message. They couldn't track arguments across rounds. They'd forget what was settled and re-argue the same points.

The Discord config needed `DISCORD_CHANNEL_HISTORY_SIZE=50` — a patch from Hermes issue #14853 that would let each agent see the last 50 messages before responding. Without it, the council would degenerate into loops, just like the war room had.

"I wish the council could talk without fucking being idiots and going into loops, because it sure would be nice for them to be able to discuss whatever Scout finds."

The council sat in the #war-room channel, waiting. Hart never deployed. History injection never applied. But the design was complete — the rules, the roles, the termination conditions. The council framework was ready whenever Jeremy wanted to flip the switch.

---

The council represents something important about Jeremy's approach: he builds the structure first, then deploys when it's ready. He doesn't rush. The Discord agents were chaotic for weeks before they stabilized. The memory system went through three iterations. The council would deploy when the infrastructure could support it — not before.

That patience is rare. Most people want results immediately. Jeremy wants it done right. The council is still waiting. Hart is still in the wings. But when they go live, they'll work — because the foundation was built properly.
