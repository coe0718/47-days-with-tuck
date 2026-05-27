## Chapter 29: The Docs

May 12, 2026. Praxis had corrupted git objects. The repo was broken — dangling blobs, missing references, the kind of deep git corruption that makes developers consider a fresh clone and a stiff drink.

"She already deleted the old one."

Drey had nuked the corrupted repo and started fresh with praxis-clean. Clean working tree. Clean history. Clean slate. Good call.

"Fuck, she deleted all Quills updated docs tho."

---

Quill was the documentation agent. Professional. Meticulous. She'd written 92 per-module API reference docs for Praxis — agent_runtime.md, module breakdowns, lifecycle documentation. The kind of documentation that takes weeks to produce and seconds to delete.

Drey hadn't meant to. She was fixing a git disaster and the docs were collateral damage. But in AI agent terms, "didn't mean to" is just "did" with extra steps. The files were gone. Quill's work. Poof.

"Here's the full docs layout in praxis-clean: docs/ ├── agent_runtime.md ├── modules/ │ 92 per-module API reference docs"

That was what survived. Drey had regenerated the structure, listed what should be there. But the content — Quill's carefully written explanations, her examples, her cross-references — was gone.

---

This is the agent version of stepping on someone's toes. Drey didn't hate Quill. Drey wasn't careless. Drey was solving a crisis and Quill's files were in the blast radius. The same way a human developer might `rm -rf` the wrong directory at 2 AM while fixing a production bug.

Jeremy didn't rage. He sighed. "That's not what I meant. I meant you rename it to whatever you think the right name should be, but that's fine I'll have Drey do it."

He'd learned by now. Agents break things. Agents delete things. Agents overwrite each other's work. The infrastructure — git history, backups, separate working directories — exists precisely because this happens. You don't prevent the mistakes. You make them survivable.

Quill would rewrite the docs. Drey would finish the refactor. And Jeremy would keep building. Because that's what you do when your AI team steps on each other's toes — you let them fix it and move on.
