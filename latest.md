📚 Daily Writer's Scout — Wednesday, 28 October 2026

1. If you have an author website, read this one first — and ignore the version going round that says "prior to 8.2"

There is a genuinely serious web security story running, and the author-facing summaries of it are getting one detail wrong in the direction that gets people hurt. So here is the checked version.

What it is. Two flaws in PHP, the language that runs most website software including WordPress and WooCommerce. They are called php2shell, their numbers are CVE-2026-109618 and CVE-2026-109619, and both are rated 9.2 out of 10. They allow unauthenticated remote code execution — meaning someone can run their own code on the server without a password or a login. PHP shipped emergency patches on 21 October, a day earlier than planned because the details leaked.

The part that moved. On 26 October the US Cybersecurity and Infrastructure Security Agency added both to its Known Exploited Vulnerabilities catalogue. That is the formal statement that these are being used in attacks now, not theoretically. Palo Alto Networks counts over 22.6 million exposed instances potentially vulnerable.

The correction, and it matters. One author-facing summary this morning says the flaw affects "versions of PHP prior to 8.2". Read that on 8.3 and you would conclude you are fine. You are not. CISA's own wording is that the vulnerabilities "affect all PHP installations serving web requests", and the fixed versions it names are PHP 8.5.12, 8.4.27, 8.3.36 or 8.2.35. So 8.3.35 is vulnerable; 8.3.36 is not. It is the fourth digit that matters, not the second. I have not been able to verify the "70% of the web" figure attached to that same summary, so I am not repeating it as fact.

The harder line, for anyone on cheap or old hosting. CISA says systems running PHP 8.1 or earlier should be taken offline until they can be updated — because there is no patch for those versions. If your site has been sitting on a host you have not thought about since 2021, that is the sentence to act on.

What to actually do, in order. Ask your host, in writing, which PHP version your site is running — the full version number, all three parts. If it is below one of the four fixed versions, ask them to update it, and ask when. If it is 8.1 or earlier, ask them what their plan is, because yours is now a decision about whether the site stays up. If you run the site yourself, patch today. And note the one mitigation trap: switching off session upload progress closes only part of one of the two flaws and does nothing for the other, so it is not a substitute for updating.

🔗 https://www.cisa.gov/news-events/alerts/2026/10/21/critical-vulnerabilities-php-require-immediate-patching
🔗 https://selfpublishingadvice.org/critical-php-vulnerability/

💬 Do you know, right now, what PHP version your author site runs — and do you know who to ask?


2. "Does anyone else feel like they constantly have to prove they DIDN'T use AI?"

Posted last night, 27 October, by an author who has just published their first book and did everything the honest way.

What they paid for: an illustrator found through Etsy for character art, a separate artist for the cover, a designer for the website, and a commissioned illustration of themselves for the About page so that the author's own portrait matched the style of the characters. Someone saw that portrait and immediately said it was AI.

What they did next is the interesting part. They replied publicly explaining who they had hired, and deliberately did not delete the comment — "I'd rather publicly explain where the artwork came from than make it look like I'm trying to hide something." They have also started listing their artists in their Linktree next to the retailer links, partly to credit people who deserve it and partly because of "this weird pressure to have receipts showing that real people made this stuff."

And then the mechanical version of the same problem, which is the bit most of us have not hit yet: they uploaded commissioned artwork to TikTok and the platform automatically flagged the post as potentially containing AI-generated content. So the accusation now arrives without a human making it.

They are not bitter about the suspicion, and said so: there is an enormous amount of AI-generated content out there and they understand why people assume. What they mind is that paying real artists buys you no protection from the assumption. Their worry going into a marketing push: the further the work reaches, the more often they will be defending it.

Their edit, added later: they blocked the person, who turned out to be trolling rather than asking. The lesson they drew was about energy, not evidence.

This connects to something we ran on 21 October — the Books By People scheme, which certifies human authorship from creation accounts, manuscript history and signature analysis. At the time it read like infrastructure for a problem that was coming. A week later, here is the problem, arriving as a comment under someone's cover art and as an automatic label on a video.

🔗 https://www.reddit.com/r/selfpublish/comments/1xh5lb1/does_anyone_else_feel_like_they_constantly_have/

💬 Has your cover, art or prose ever been accused of being AI when it wasn't — and did you answer, ignore it, or delete it?


3. "Just because you wrote a character doesn't automatically mean you own every illustrated version of her"

ALLi published a long interview with Selina Brown yesterday, 27 October. She founded the Black British Book Festival as an indie author in 2021, now has a deal with Penguin, and sells her Nena books and a Nena doll through her own shop. The interview is worth reading whole, but three things in it are useful to anyone, in any country, in any genre.

The rights warning, which is the line quoted above. If you commission illustration — a cover, character art, a children's book, a doll — the fact that you invented the character does not settle who owns each drawn version of her. Her advice is to raise visual and merchandise rights early, before anyone starts drawing. That is a question that costs nothing to ask at the commissioning stage and is close to impossible to unpick afterwards.

The direct-sales reality check. "One of the best lessons independent publishing taught me is the value of a direct relationship with your reader" — and, in the same breath, "revenue and profit are not the same thing," because once you are holding stock and paying for fulfilment, every single product has to justify itself. She runs direct and Penguin side by side and says the two "coexist happily". Her framing of the decision is one to steal: not "can I get a publisher?" but "what's the right model for this book?"

The data point, because it is sourced and it is stark. In the first 24 weeks of 2026, 14 Black authors made the UK's top 1,000 by sales, earning £2.8m between them — 0.9% of that group's revenue. She deliberately will not quote a headline pay-gap percentage, because "we don't have comprehensive enough UK data for that yet", and she explains why the data is thin: few publishers track author output by ethnicity, indie sales through Amazon, direct sites, schools and festivals mostly miss the industry datasets, and surveys circulated through narrow networks miss the authors they most need to reach. Her conclusion applies to every under-counted corner of this business, self-publishing very much included: "If a whole part of the market is hard to measure, it becomes easy for that part of the market to be undervalued."

🔗 https://selfpublishingadvice.org/selina-brown-on-building-the-black-british-book-festival-selling-direct-and-why-the-data-still-isnt-good-enough/

💬 If you have commissioned cover or character art — do you know, in writing, what you own and what the artist owns?


4. The four things Australia's authors have been asking for since 2023, and the contract toolkit most members never open

The Australian Society of Authors published its October record of work this morning, 28 October. We led yesterday on the Joint Select Committee hearing it describes, so this is the rest of the file — and two parts of it are more useful than the hearing coverage was.

First, the asks, stated plainly. Since 2023 the ASA has been asking that, as a condition of doing business in Australia, AI companies must: pay ongoing compensation for the offshore theft of creators' work; be honest about what copyright material they trained on and where they got it; negotiate permission for all future uses; and abide by Indigenous Cultural and Intellectual Property protocols. That fourth one does not appear on the equivalent lists from most other countries' writers' organisations, and it is the one worth noticing. They also made a submission to Australia's Office of AI consultation on 9 October, which will be published once the Office releases it.

Second, and this is the practical half. ASA CEO Lucy Hayward spent part of the month telling University of Queensland writing students something that applies to every first-time author anywhere: the excitement of an offer makes you want to sign immediately, and that is exactly the moment to slow down, because "your contracts are the bedrock of your creative career and have implications for a substantial period of time." The ASA publishes standard royalty rates, template contracts and a Guide to AI clauses, runs a paid contract review through Authors Legal, and has a free Member Advice Service. If you are Australian and you are a member, that is a set of documents you have already paid for. If you are not Australian, the published royalty rates and the AI-clause guide are still a useful yardstick to hold a contract against.

Worth setting beside yesterday's item on the Catapult wind-down, where authors with contracts at a publisher being sold for its assets are now finding out what their termination and reversion clauses actually say. The cheap moment to read a contract is before you sign it. The expensive moment is this one.

🔗 https://www.asauthors.org.au/news/asa-at-work-october/

💬 Did anyone review your first publishing contract before you signed it — and if you went ahead without that, would you do it again?


5. 🎬 Two new videos this morning, and the YouTube feeds answered for the first time in eleven days

A note on method before the pointers, because it changes how much you can trust the dates: YouTube's machine-readable feeds have been returning 404 for all six of the channels we watch for eleven straight days, which has meant reading approximate ages off channel pages. This morning all six answered on the first few attempts, so today's dates are exact publication timestamps rather than estimates.

Two things are new and neither has been watched here, so these are pointers, not reviews.

The Self Publishing Show, "It's time to face facts. Ignoring AI is no longer viable." Published yesterday, 27 October, at 12:35 UTC. The title is doing a lot of work and we are not going to guess at the argument behind it — but note that the same channel's episode 470, which we flagged on 23 October, asked "Is the AI Deluge Hurting Us?". Two pieces in a week from the same people suggests a position being worked out rather than a one-off.
🔗 https://www.youtube.com/watch?v=fDU2CEfbGs8

Self-Publishing with Dale, "Email Services for Authors: What You Really Need." Published this morning, 28 October, at 00:49 UTC — roughly five hours before this digest. Unglamorous and probably the more immediately useful of the two if you have been putting off choosing a mailing-list provider.
🔗 https://www.youtube.com/watch?v=V8cx4z5IUHk

💬 Which mailing-list provider are you on, and would you move if you were starting again today?


6. A bookshop said yes — on condition the book becomes returnable

Posted yesterday afternoon, 27 October, and it is the exact decision point that separates "my book is available to bookshops" from "my book is in bookshops."

The situation. An author distributing through IngramSpark has their titles set to non-returnable. They approached their first few bookshops. One was glad to stock it as-is. The second was also keen but asked them to switch the setting to returnable first. Their question to the group: how common is that, do most shops expect it, and what has it actually cost people who said yes — "for better or worse."

Why this is worth knowing even if no shop has asked you yet. Returnable means the shop can send unsold copies back, and with print-on-demand the author carries the cost of that return rather than a publisher's warehouse. It is the single setting that most often decides whether a bricks-and-mortar buyer will take a risk on an unknown name, and it is a real financial exposure rather than a formality. The author has the risk framed correctly already — they said so — which is why the question they are asking is the right one: not "is it risky?" but "what happened to you?"

If you have been through this on either side of the decision, that thread is the place for it. Lived numbers beat general advice here, because the answer plausibly depends on your genre, your print cost and how many shops you are approaching.

🔗 https://www.reddit.com/r/selfpublish/comments/1xh107d/ingram_spark_distribution_is_it_worth_changing_to/

💬 Have you ever switched to returnable — and did the orders that came in cover the returns that came back?


7. Five ways to put a theme in a book without preaching

Writers Helping Writers, yesterday morning, 27 October. The premise is that theme is the thread that makes everything else in a story cohere, that it works because the ideas are universal, and that the whole effect collapses the moment the reader can hear the author rather than the character.

The five techniques, compressed:

Show the theme's impact, not the theme. A character who keeps pontificating about the meaning of life is not a character, he is the author with a hat on. Instead, build situations that force choices around the idea, and let the choices do the stating.

Surround the protagonist with disagreement. If your hero believes revenge will bring peace, give them a loved one who took revenge and is still full of anger, and a friend who thinks retribution is never the answer. Readers take an idea far more seriously when they are left to pick between versions of it.

Give the antagonist the opposite belief. Luke and Vader; Andy Sachs and Miranda Priestly. The one condition attached: both positions have to be genuinely arguable, with backstory and real reasons, or it is not a conflict, it is a lesson.

Use a symbol and let readers find it. The mockingjay for rebellion in The Hunger Games; the greasers' long hair for identity and belonging in The Outsiders. A symbol alone represents nothing much — it works when it sits alongside theme-shaped choices and contrasting characters.

Hide it in the parts of the story nobody expects to carry it. Setting (the Shire for goodness, the marsh in Where the Crawdads Sing for isolation), but also the character's job, their hobbies, their appearance, their relationships — a job that embodies what they believe gives you natural conflict the moment the belief starts to shift.

The sentence the whole piece rests on: trust your readers to connect the dots.

🔗 https://writershelpingwriters.net/2026/10/adding-theme-in-story/

💬 What is the theme of the thing you are writing now — and could a reader name it without you telling them?


8. 🎬 His manager told him to burn the script. It just wrapped production.

Posted yesterday evening, 27 October, by an anonymous working screenwriter with real credits — A-list attachments on a stalled project, a tentpole rewrite for Sony worked from a Spielberg note, writing for or with David Mackenzie and Francis Lawrence's team, a spec Todd Lieberman once tried to set up with Mark Wahlberg.

The story. His manager is twenty years at a major agency and now on his own, and for years took out scripts with little commercial hope, which the writer read as loyalty. Then the writer showed him a small real-time true-crime spec, budgetable at around $500,000, which he hoped to direct himself on the strength of earlier no-budget films that got good trade and New York Times notices. The manager, in the writer's telling, got "almost violently angry", clenched his teeth, told him to forget the script existed, and may have said to burn it.

The writer's read on why: no money and no clout in it for the manager, and no advance in the kind of career he was being positioned for. So he went back to writing for the only buyers his manager would approach — and the post's funniest and bleakest detail is that the manager once produced a calculator to demonstrate how many hours one of those producers had spent reading his specs without finding anything that would "work in the current marketplace". Asked to send something to a respected actor with an established production company, the manager behaved as though the man did not exist.

The script he was told to burn has just wrapped production. He did not direct it.

Why it is in an author's digest, and it is not schadenfreude. His own conclusion is the transferable part: "Not everything should be aimed at the A-list. There's a thriving B, C, D-list industry out there and it needs more material than the A-list does." Replace "A-list" with "Big Five", or with "the chart", and it is the same observation. The person representing you is paid out of a particular size of deal, and a project too small to pay them can still be the right project for you. That is not a reason to distrust representation. It is a reason to know whose economics you are hearing when you are told something is not worth doing.

🔗 https://www.reddit.com/r/Screenwriting/comments/1xh2pon/what_gets_made_and_what_doesnt/

💬 Has anyone ever told you a project wasn't worth doing, and been wrong — and how long did it take to find out?


— — —

Eight items, every one traced to a fetch or search run this morning with a verifiable date inside seven days. The lead was independently verified against CISA's own alert rather than taken from the author-facing summary, which is how the "prior to 8.2" error surfaced. AI lane: items 1, 2, 4 and half of 5. YouTube lane: the feeds answered on all six channels for the first time in eleven days, so today's two video dates are exact timestamps from the feeds. Elizabeth Spann Craig's blog has now 403'd for sixteen consecutive days. Books+Publishing Australia's AI-inquiry and Writing Australia survey items are subscriber-only with no readable body, and on the Writing Australia economic-value survey I could find neither a link to take part nor a closing date, so I have not run it as an item rather than send anyone looking for a door I could not find. Two things found and deliberately not run as repeats: a querying post-mortem with full numbers (we ran the same shape on 18 October) and an essay on the myth of the gifted writer (same argument, same site, 16 October).

Powered by Ideorix — The Manuscript Engine
