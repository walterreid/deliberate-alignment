# CHAPTER NINE
# The Three People in the Room

*Mark knew a problem. John heard a problem. Walter built the solution. For now, it takes all three.*

Mark is well-connected in private equity. He knows CEOs the way people in that world know CEOs — through deals, through boards, through the specific texture of trust that gets built when money changes hands and things either go well or they don't. One of the people he knows runs a franchise operation that has been managing its business the way franchise operations managed their businesses twenty years ago: spreadsheets, manual processes, institutional knowledge stored in the heads of the people who have been there longest.

He introduced John to Joe and Keli.

Joe and Keli are ex-bankers. They left the bank to open a Filta Environmental franchise in Deer Park, New York — which is a trade most people understand instinctively — the security and the constraint of the institution, exchanged for the risk and the autonomy of ownership. They knew the pain of their current operation. They could feel the inefficiency every day. What they did not know was what to do about it, or whether what they needed even existed, or whether building it was something that happened to companies their size.

John is a Meineke franchise operator. He is building from the operator's seat, not a boardroom. He sat with Joe and Keli, asked the right questions, watched how they worked, understood the pain not as a description but as a felt thing — the spreadsheet that had to be downloaded, edited by hand, and uploaded again every single week. The vans they couldn't see and the routes they couldn't trust. He came away with something rare: a real understanding of a real problem, specific enough to be solved.

Then he built a prototype.

The prototype was real, in the way that a blueprint is real. You could see the shape of the building. You could imagine living in it. What it could not do was support weight.

He brought it to me.

## What the Prototypes Said

What followed was not a document handoff. It was two competing prototypes.

John's had twenty-plus features — scheduling, routing, invoicing, fleet views. It had sixty-plus migration files, two of which had never been run. It had the ambition of someone who understood the problem deeply and had built at AI speed without an architectural plan underneath. My prototype had none of that. What it had was multi-tenant infrastructure — the foundation that would let the system serve not just Joe and Keli but any franchise operator with a similar problem, cleanly separated, without one customer's data bleeding into another's.

The alignment between us was not a conversation that produced a document. It was a structured comparison, with Claude Opus as participant. Opus saw both codebases and determined that it was actually easier to fix my foundation than to rebuild John's features on top of it. The elegant infrastructure could absorb the features. The features could not retroactively produce the infrastructure. That assessment — an AI holding something like the taste function, able to see which architecture would bear weight — became the decision. We built forward from my foundation and migrated John's feature logic into it.

That is Deliberate Alignment mediated by AI. The AI did not make the decision. It held a structural judgment that neither of us could have held as clearly on our own, because neither of us could read both codebases simultaneously and evaluate which path forward would cost less in the long run. The authority was still ours. The depth was still John's. The taste function — the assessment of which architecture was good enough to build on — was shared between me and a model that could see what I had designed and what John had built and compare them without the politics of whose work was better.

## What the Data Said

What I found when I looked at what John had heard was a problem worth solving and a set of constraints that would only become visible through the data.

Joe and Keli's operation ran on a franchise CRM with 189 columns in its export. Longitude values with apostrophes embedded. Schedule records where status had to be inferred from combinations of date fields because a human always knew — a status column had never been necessary before, so one had never been built.

The schema the prototype had imagined was not the schema the actual data required. The first real work was not building. It was listening to what the data was saying about how the business actually ran, as distinct from how the problem had been described.

This is what Chapter Eight called the sensible-for-one, made concrete. No product manager at a software company was ever going to build for the specific intersection of this franchise's proprietary CRM, this fleet's GPS system, Google's route optimization API, and the particular way this operation had grown. The market was too small. The integration too specific. The combination of constraints too particular to justify the overhead of a commercial product.

From that point, it moved. Each phase had a clear definition of done. The decisions that mattered most were not technical — they were product decisions with technical implications. What system is read-only. Who owns the optimization. How to build for a vendor whose partnership agreement doesn't exist yet without letting that block the whole architecture. These were conversations, not specifications. Each one required understanding the business well enough to know what the constraint was actually protecting.

## What Keli Actually Needed

Here is what Keli actually needed, described precisely.

Every week, she downloaded a spreadsheet from her franchise organization's CRM. She edited it by hand — adjusting routes, accounting for new clients, fitting new vans into sequences the software didn't understand because the software wasn't built for an operation her size. Then she uploaded it back. Four hours, every week, because the franchise CRM claimed to handle routing and didn't, not really, not for a business growing the way hers was growing.

When she added a van, she didn't add a van. She added four more hours.

What she wanted — what she hadn't said in those words but what John heard underneath everything else — was to go to Ireland in the summer. She and Joe had been talking about it for two years. Every time they got close to planning it, the business got more complex and the margin of time they needed to feel safe leaving contracted again. The franchise kept adding features to its CRM that addressed other franchisees' problems. None of them addressed hers.

The software is called RouteForge. It started on February 26, 2026. By early March, there was a working demo. By March 6, a full production system was live — dispatch, invoicing, compliance reporting, analytics, fleet tracking, a customer portal, communication tools, equipment tracking, and job management, across twelve-plus industry verticals. Three people built it.

The comparable commercial tools — ServiceTitan, FieldRoutes, BuildOps, Route4Me — charge between two hundred and four thousand dollars a month and took years of development by teams of dozens. What would have been an eighteen-month product roadmap with a fifteen-person team was built in six weeks by three people who had never worked together before February.

RouteForge downloads the export, runs it through Google's route optimization with their vans and their clients and their times, and uploads it back. It gives Joe and Keli a live view of their trucks through their GPS system, because the franchise CRM claims to offer this and doesn't. It generates compliance reports for health department inspections without touching a spreadsheet. It does the job to be done in a way that no template software could — because no template software would embed with a proprietary franchise CRM, integrate a separate GPS vendor, and re-upload the result via Excel in a loop that the franchise system will accept.

RouteForge is live. Five or six companies across verticals have expressed interest. Joe is pushing for adoption among operators he knows. Keli wants to go to Ireland at the end of the year, and for the first time, the plan has a system underneath it instead of a spreadsheet.

But the adoption barrier is not technology or product. It is the thing this book has not yet named directly: operational lock-in at the customer level. The franchisee who wants to adopt RouteForge has to run it alongside their legacy CRM during the transition — doubling their operational complexity during the period when they are most cost-sensitive and least willing to risk disruption. The real challenge is not having customer testimonials or social proof, and the customers' legacy systems not giving them easy access to their own data. The economic logic is right. The product is right. The transition cost is carried entirely by the customer, and that cost is not monetary. It is attention and risk, which are the scarcest resources a small business owner has.

## The Three Functions, Revisited

Mark was the lead — not in the sales sense, but in the trust sense. He knew the landscape. He knew who had real problems and who had the authority to decide to solve them. He connected the right people. Without him, John never meets Joe and Keli. Without him, the problem remains a spreadsheet.

John was the depth function. He heard what was needed beneath what was said. He understood that Joe and Keli weren't asking for software — they were asking to stop carrying the weight of their own operation's complexity on their personal time every week. He could see the shape of the solution because he understood the shape of the pain. What he could not do was build from that understanding.

I was the execution function — but execution, in this context, included what Chapter Four called taste. The 189 columns, the apostrophes in longitude values, the status fields that had to be inferred from date combinations — those were not just data problems. They were decisions about what the business actually needed versus what the CRM had imagined it would need. Each product decision had technical implications, and each technical constraint had product implications. Knowing which to respect and which to work around required understanding what good looked like before it was built.

The deliberate alignment of those functions is what produced RouteForge. Remove any one and the thing doesn't exist. Mark without John and me is a warm introduction to a problem that stays unsolved. John without Mark and me is a prototype that cannot hold weight. Me without Mark and John is a solution to a problem I don't fully understand, built in a direction that may be technically correct and operationally wrong.

And here is the part that mirrors the book's thesis back at its own author: RouteForge has more execution capacity than depth capacity. We could use more clients in the room and fewer developers. If I sat down with those clients instead of them doing the job, we could design any system that would help them. The bottleneck is understanding, not building. The framework I have spent nine chapters describing is the framework my own venture is constrained by.

## The Dependency That Is Dissolving

Now the uncomfortable part.

John needed me to build what he heard. He needed me specifically — someone with the product instinct and the technical depth to turn his understanding into something real. That dependency is real today. It is also dissolving.

Not because John will become a developer. Because the execution layer between understanding and artifact is compressing faster than any of us have fully reckoned with. The prototype John built — the blueprint that couldn't hold weight — is already closer to the finished building than it would have been a year ago. The distance between what John can produce and what Joe and Keli need is shorter than it was when he first walked into their office.

The book you are holding was written on the assumption that the three functions would remain distinct for long enough to build a methodology around them. That assumption is probably right for the next few years. It may not be right for the decade. The person closest to the client — the person with the depth function, who hears what is actually needed — will need the execution function for less and less time as the execution layer continues to compress.

What that means for the room is what this book has been trying to describe. For now, it takes all three. The room that produced RouteForge required Mark's connection, John's depth, and my execution, working from the same understanding at the same moment — where the handoff was not a handoff because the understanding never had to be summarized and degraded into a document that someone else would misread.

The question is not whether John will be in that room.

The question is what he will need when he gets there.

*Mark knew who had the problem. John heard what the problem was. Walter built the solution. For now, that is three people. The question the next decade will answer is which of those functions the room can hold alone.*

