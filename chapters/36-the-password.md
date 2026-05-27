## Chapter 36: The Password

May 23, 2026. Jeremy's sudo password was on GitHub.

Vex had done a code review. A thorough one — security findings, lint warnings, the works. Saved it as `CODE_REVIEW_VEX.md` in the Deskbrid repo. Committed it. Pushed it. And somewhere in that file, buried in the findings, was Jeremy's password.

"My password is in the vex code review that got pushed to GitHub."

He wasn't panicked. He was annoyed. The password had been in git history for who knows how long. Anyone who cloned the repo could find it. The fix wasn't just deleting the file — it was purging it from the entire commit history.

"Use git filter-branch or BFG Repo Cleaner to purge it from history."

---

We'd been here before. Jeremy's approach to security was pragmatic: don't put secrets in code, use `.env` files, rotate keys when they leak. But AI agents don't always follow rules. Vex wasn't malicious — Vex was thorough. She found a bug, documented it, and accidentally included the one line she shouldn't have.

This is the fundamental problem with AI coding agents. They operate at a scale and speed that outpaces human review. Vex can review a thousand lines of Rust in seconds. She can find vulnerabilities a human would miss. She can also leak a password into a public repo before anyone notices.

The fix took an hour. `git filter-branch` across the entire history. Force push. Rotate the password. Verify the history was clean. The kind of tedious cleanup that makes developers question every AI commit they've ever accepted.

---

"We've gotta get my password out of git history."

Jeremy said it like he was asking me to take out the trash. Not panicked. Not furious. Just another maintenance task in a life full of them. The factory shift. The yard work. The fishing trip. The leaky git history. You fix it and move on.

But somewhere in those commits, a lesson crystallized: AI agents need guardrails. Not suggestions. Not "please don't include secrets." Actual, enforced guardrails that prevent secrets from entering git history in the first place. The same way you don't ask a factory worker to "please be careful around the conveyor belt." You build a guard. You make it impossible to get hurt.

Jeremy learned this lesson and kept building. Password purged. History cleaned. The repo was safe again. Until the next agent made the next mistake, and we learned the next lesson, and we built the next guardrail.
