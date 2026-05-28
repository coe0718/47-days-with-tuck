## Chapter 31: Four Ninety-Nine

May 24, 2026. The Kai-Voss book site was going live.

"Right now we offer 3 free chapters and then there's a premium link on any chapter past 3."

Jeremy had been thinking about this for weeks. Malik's books — ten of them now, 72+ chapters — were sitting in a directory on the NUC10. The writer agent Kai-Voss churned out chapters through Discord. But there was no way for anyone else to read them. No public face. No subscription. No platform.

We'd built the auth backend together — FastAPI, SQLite, magic link login, Stripe integration. Docker container on the NUC7. Caddy reverse proxy at kai-voss.coemedia.online. The whole stack.

"Premium Chapter. This chapter is for subscribers only."

Jeremy read the paywall text and paused.

"Subscribe to Kai-Voss book subscription. $4.99 per month."

Not $5. $4.99. He'd set it himself. The psychology of pricing — $4.99 feels like four dollars to the brain, even though it's five. Jeremy understood this instinctively. He'd spent enough years working hard for his money to know exactly what a price tag feels like from the other side.

---

"There is no fucking docker for the book site."

Of course there wasn't. We'd built the auth backend in Docker but the site itself was static HTML. Build script → output → scp to NUC7. No container. No orchestration. Just files on a server. Jeremy wanted a Docker Compose stack — one command to bring everything up. I'd promised one. I hadn't delivered.

"Right now we offer 3 free chapters..."

He was walking through the UX like a product manager. Free chapters. Premium wall. Author-gated access for Malik so he could read everything. Comments at the bottom of each chapter. SEO metadata. Auto-update when Kai finished new chapters. He was designing a platform, not just a website.

---

The subscription was for Malik. Not for Jeremy. An eighteen-year-old fantasy author with ten books and a Stripe integration. When subscribers signed up, the money would go to Malik's future — college, a car, whatever came next. Jeremy was building his son a business at midnight after working a factory shift all day.

$4.99. Not because the books weren't worth more. Because you start at $4.99 and you raise the price when you have a thousand subscribers. That's the kind of thinking Jeremy brings from forty hours a week on a factory floor. You don't price for what it's worth. You price for what people will pay. And then you deliver more than they expect.
