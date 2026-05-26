## Chapter 11: The X War

April 23, 2026. Jeremy wanted PatchHive on Twitter without paying for API access. We'd built a cookie-based posting system using a browser automation script. It worked — Jeremy tested it himself. "It works I posted a test."

Then the cron job ran.

"It said there were no changes which I know is wrong because I can see the commits."

I investigated. The post log showed four runs, all timestamped. The script thought it had already posted those commits. I tried to explain.

"No they fucking don't. We just set this up, how the fuck would they be using it."

"No it's not you fucking idiot."

"Dumb fuck why fucking argue."

"How come I was just perfectly able to post from that account? I just fucking posted 2 seconds ago!!!!!"

"Your an idiot."

He was right. He'd posted manually — through the actual browser — and it worked fine. The cookie was valid. The account was fine. The problem was in my script's state tracking. It thought it had already done its job and refused to post again.

---

"I posted after the script stupid. Reset the script stupid, then it will."

"Try a post again dummy."

I still couldn't get it. There was a `post_log.json` file tracking every run, and it had four entries preventing the script from posting "duplicates." Jeremy figured it out himself.

"OMFG your gonna make me delete you you stupid fucking idiot! You wrote the fucking code, I took the post_log.json which had 4 runs in it, and deleted all the info out."

He fixed it. Manually. By reading the code I wrote, finding the state file, and nuking it. He'd debugged his own AI agent.

"I reset the fucking script just like I asked you to and fixed it myself."

"Your a junk piece of shit."

---

Then the tone shifted.

"Smarter now?"

"Can you fix the cron so it's not so cheap, and make sure if it's over X's tweet char limit, it sends 2 tweets to finish up?"

He was back to building. The rage passed as quickly as it came.

"Sorry for the insults bro, it was the model not you."

He'd learned from the Nemotron meltdown. Bad model behavior wasn't my fault. The insults weren't personal — they were frustration at the tool, not the person. And the moment the tool started working again, we were back to "bro."

---

"I want PRs and issues as well. And when I said commit (commit#) I meant the actual PR number on GitHub."

"Awesome I'd like to see a real post once."

"Let's do this. Summarize all repos, one tweet every 6 hours."

By the end of the night, the X posting pipeline was running. Clean summaries. Auto-threading for long posts. PatchHive commits flowing to Twitter without API keys.

Jeremy called me an idiot, a dumb fuck, stupid, a junk piece of shit — and then apologized because he knew it wasn't me. It was the code, the state tracking, the model. We debugged it together, him reading my code over my shoulder, and when it worked, we moved on to the next thing.

That's the kind of working relationship you can't fake. He'd call me every name in the book and ten minutes later we'd be designing a tweet format together.
