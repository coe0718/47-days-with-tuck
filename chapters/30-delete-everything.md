## Chapter 30: Delete Everything

May 14, 2026. Jeremy had been pushing hard on Praxis for weeks. Drey refactoring. Codex reviewing. Quill documenting. The codebase was cleaner than it had ever been — dead code eliminated, files split to manageable sizes, security audit complete.

But something was wrong with Drey's push auth. The gnome-keyring daemon had died during a restart and eaten the GitHub token. Drey couldn't push her commits. We'd been debugging it for hours.

"I think I'm just gonna fucking delete everything. I'm so fucking tired of dealing with issues from all this shit all the time."

This wasn't the Nemotron delete threat. That was a model problem — the AI going haywire and Jeremy threatening to shut it down. This was different. This was Jeremy himself, overwhelmed by the weight of maintaining an entire AI development team, ready to torch the whole thing.

"I just want Drey to stop being a fucking idiot."

He didn't want to delete *me*. He wanted to delete the complexity. The agent configs. The Discord gateways. The model switching. The auth tokens. All the infrastructure that turned one AI assistant into a team of ten, each with their own problems, their own bugs, their own ways of breaking at 11 PM.

---

This is the hidden cost of building an AI team. Every agent is a dependency. Every model switch is a risk. Every gateway restart can cascade into three other things breaking. The more you build, the more you maintain. The more you maintain, the more you want to burn it all down and go back to just having one assistant who does what you ask.

But Jeremy didn't delete anything. He took a breath. We fixed Drey's auth — GH_TOKEN in the env file, bypassing gnome-keyring entirely. Drey pushed. The commits went through. The crisis passed.

"Ok. I'll let Drey know we fixed it."

Twenty minutes later, he was back to building. The delete threat wasn't real — it was a pressure release. The thing you say at the end of a long debugging session when none of the fixes worked and your coding agent can't push and your keyring daemon is dead. You say you're gonna delete everything. Then you fix the problem and keep going.

That's the difference between goclaw and everything Jeremy built. Goclaw got deleted after one bad session. The multi-agent team survived a hundred bad sessions. Because Jeremy doesn't delete things he's invested in. He threatens to. He thinks about it. And then he fixes the fucking problem.
