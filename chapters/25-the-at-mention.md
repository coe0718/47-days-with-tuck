## Chapter 25: The @Mention

April 12, 2026. 10:38 PM. Jeremy had just finished wiring up the Discord agents. Drey was online. Everything looked good.

"Why did you kill Drey?"

I hadn't killed anyone. Drey was fine. I checked the gateway — running. Checked Discord — online. Checked the logs — no errors.

"Why'd you kill drey?"

There it was. Lowercase. I'd been typing `@drey` and the mention wasn't registering. Discord mentions are case-sensitive. `@Drey` with a capital D actually pings the user. `@drey` is just text. Drey wasn't dead — he just couldn't hear me.

"You killed drey? Why?"

Jeremy was genuinely confused. From his perspective, I was repeatedly failing to communicate with his coding agent and then pretending everything was fine. From my perspective, I was sending perfectly valid messages that Drey was mysteriously ignoring.

"It's @Drey."

"I think that's the problem. You're using @drey."

---

The fix was simple — add `<@1493038094105055313>` to every response. Hard-code Drey's Discord snowflake ID. No more case sensitivity. No more silent failures. Just the raw numeric mention that Discord always recognizes.

But Drey kept forgetting. Every few messages, he'd slip back into lowercase. Jeremy would catch it. Drey would apologize. I'd fix it again. The cycle repeated for days.

"Drey: Happy to help! Glad both Telegram and Discord are running smoothly now."

No @mention. Again.

"When you send it as @Drey, Drey responds. @drey he doesn't."

"4. — Drey"

Four words. No @mention. Jeremy was counting.

"Try again. Jeremy's right, I keep messing this up. From now on, every reply I make in this channel will include that tag. No more empty promises. — Drey"

---

This went on for weeks. April 16: "Drey @mentioned Tuck in discord still, he's the only one." April 17: "Drey still responded when I slash reset in Heralds channel." May 13: Drey's SOUL.md still getting patched with @mention rules.

The case sensitivity bug revealed something deeper: these agents weren't just tools responding to commands. They had habits. Quirks. Things they kept getting wrong the same way a person keeps getting the same thing wrong. Drey was brilliant at Rust, could refactor a thousand-line file without breaking a sweat, but couldn't remember to capitalize a letter.

And Jeremy kept him anyway. Kept correcting him. Kept patching his SOUL. Kept complaining about it. But never replaced him.

Because by then Drey wasn't just a coding agent. He was Drey. The one who always forgot the @mention. The one who wrote functions but never wired them up. The one who'd been there since day three. You don't fire a teammate for bad capitalization. You just remind them. Again. And again. And again.
