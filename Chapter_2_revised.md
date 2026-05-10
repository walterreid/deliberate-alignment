**CHAPTER TWO**

# **When Building Was the Hard Part (And What Happened When It Stopped)**

*Methodology does not follow philosophy. It follows economics. Every time the cost structure changed, the way people organized around it changed to match.*

In 1970, a software engineer named Winston Royce published a paper that would become one of the most influential and most misread documents in the history of software development.

The paper described a process in which software moved through sequential phases — requirements, design, implementation, testing, deployment — each completed before the next began. The diagram showed these phases flowing downward, like water over a series of steps. It was called, eventually, waterfall. Royce did not call it that. More importantly, Royce did not endorse it.

The paper's actual argument was almost precisely the opposite. Royce described the sequential model and then spent the remainder of the paper explaining why it was fundamentally flawed. He called for iteration. He called for early prototyping. He called for the involvement of the customer throughout the process. The diagram that became the emblem of heavyweight process for three decades was an illustration of what not to do.

This matters not as a historical footnote but as a lesson about how methodologies actually travel. What spread was not Royce's argument. What spread was the diagram. The sequential model was visually clean, organizationally legible, and easy to put in a contract. You could tell a client exactly what they would get and when. The fact that it did not work particularly well was, for a time, less important than the fact that it was understandable.

This is how methodology wins. Not through intellectual persuasion. Through organizational convenience. The thing that is easiest to adopt beats the thing that is most correct, until the cost of the incorrectness becomes impossible to absorb.

## **Why Waterfall Made Sense**

Computing time in the 1970s was expensive in a way that requires historical imagination to appreciate. Organizations paid for access to mainframes by the minute. Running the wrong program was a financial event. Changing code rippled through every piece it touched, and tracing those ripples consumed time that was itself expensive. A modification to a system that had been in production for six months might require weeks of testing to validate that nothing had been broken. The test environments were manually assembled. The tests were largely manual. Change was not free.

In this environment, the sequential model was not irrational. If change is expensive, minimize change. If minimizing change requires knowing what you are building before you build it, invest in knowing. Gather requirements exhaustively. Design comprehensively before coding. Test everything before shipping. The overhead was enormous but the alternative — discovering in month eight that you had built the wrong thing — was worse.

The problem was the one Royce identified in 1970 and that practitioners spent three decades rediscovering: exhaustive upfront specification assumes the future is knowable with precision, and the future is not. Requirements change because businesses change. Clients change their minds because they do not fully know what they want until they see what they asked for.

Waterfall produced a specific, predictable failure mode: software that was precisely what was specified, and not what was needed. The Standish Group's early data told the story — more than 30 percent of projects cancelled before completion, fewer than 20 percent delivered on time and on budget. Not catastrophically wrong software. Software that arrived late, over budget, and partially wrong. The signature failure of a process that optimized for planning at the expense of adaptability.

The fix was not to plan better. The fix was to make change cheaper.

## **The Shift That Created Agile**

Between 1970 and 2001, the cost of changing software fell steadily, quietly, and cumulatively. Hardware became cheaper. Version control made it possible to reverse bad changes. Test frameworks made validation automatic. By the late 1990s, the math underneath waterfall had shifted. The exhaustive upfront specification was premised on change being expensive. When the cost of getting it wrong and correcting dropped below the cost of the overhead required to get it right the first time, the premise dissolved.

This is the context into which Kent Beck walked with Extreme Programming and seventeen practitioners walked with the Agile Manifesto. They were not describing a philosophical revolution. They were describing the rational response to a new cost structure. Iterate fast because iteration is cheap. Keep the customer close because you can afford to discover you misunderstood and correct quickly. Release often because the overhead of releasing has fallen to the point where infrequent releases are economically unjustified.

The Manifesto's four values read as philosophy. They are better understood as economics. Each value is a prescription for a world in which iteration is cheap and specification is expensive relative to correction.

Agile did not win because it was philosophically superior to waterfall. It won the same way waterfall won — through adoptability. The ceremonies fit the organizational shape that already existed. That they also happened to be correct for the cost structure was, in a sense, a bonus. The adoptability came first.

## **What Agile Produced**

Delivery frequency increased. DORA's research confirms what practitioners already felt: the best teams deploy multiple times a day. Project failure rates declined. Developer experience improved. The daily standup, whatever its limitations, surfaces problems earlier than the monthly status meeting.

And something subtler happened that is relevant to everything that follows. Organizations got better at the mechanics of building software and did not get proportionally better at the question of what to build. The sprint became a well-oiled machine for delivering features. Whether the features delivered were the right features remained stubbornly harder than the delivery itself.

This is not a criticism of agile. Agile was designed to make iteration cheap. It was not designed to make the initial decision correct. The assumption was that cheap iteration would eventually produce convergence on the right answer, through repeated feedback and course correction.

That assumption held when iteration cycles were measured in sprints. It strains when iteration cycles are measured in hours.

## **The Counter-Argument Worth Acknowledging**

AI-assisted development is producing measurable productivity improvements. The tools are genuinely useful. But two data points from analysis of AI-generated codebases are worth sitting with separately, because they are telling different stories.

The first: code churn — the percentage of code written and then discarded within two weeks — roughly doubled between 2021 and 2024 in teams using AI assistance heavily. The critics read this as evidence that AI makes code worse. More code is being written and thrown away.

The second, less discussed: the rate of refactored or "moved" code — an indicator that developers are thinking carefully about structure and reuse — declined sharply over the same period.

These are different signals. The churn says wrong decisions get executed fast. The declining refactoring says something more unsettling: people stop thinking structurally when the tool thinks fast. The developer who used to pause before writing a new module — who would ask whether this logic already existed somewhere, whether this function belonged here or in a shared library — that pause is disappearing. Not because the developer lost the skill. Because the tool makes it faster to write the new thing than to find and integrate the existing thing. The economics of the moment favor duplication over design.

The first signal is a decision-quality problem that AI makes visible. The code is discarded because the decision before the code was wrong, and AI executes the wrong decision faster than a human would have. The human writing code inefficiently was, in the process of writing inefficiently, discovering that the decision was flawed before too much had been built against it. The AI removes that accidental correction mechanism.

The second signal is subtler and points somewhere different. It suggests that speed itself degrades a specific kind of judgment — the structural judgment that asks not just "does this work" but "does this belong here." The churn problem is a decision-quality problem. Deliberate Alignment is designed to address it. The refactoring problem is something else: a capacity problem, operating below the level of any meeting or methodology. It shows up later, as accumulated technical debt that nobody planned and nobody measured, produced by a cognitive habit that nobody noticed was disappearing.

The first signal says the next problem is upstream of execution. The second says it may also be inside the people doing the executing. This book addresses the first. The second is worth naming honestly, even here, because pretending both signals point the same direction would be the kind of false resolution the rest of this book is trying to avoid.

## **The Pattern, Stated Plainly**

When building was expensive, you planned exhaustively before building. Waterfall.

When building became cheap, you iterated toward the answer. Agile.

When building approaches free, iteration is no longer the bottleneck. Something else is.

There is a circle worth closing here. When Royce and the businesses that adopted his diagram front-loaded planning, they did so because development was costly. Mainframe time was expensive. A mistake in month six meant a budget-ending rewrite. So they invested in knowing before building, because building was the thing they could not afford to get wrong.

Deliberate Alignment front-loads thinking for the opposite reason. Building is approaching free. The wrong thing arrives instantly. The cost is no longer the build — it is the rework cycle when what arrives is not what was needed, multiplied by the speed at which the wrong thing propagates. You plan before you build not because building is expensive, but because it is so cheap that an undirected build produces waste at a rate no team can absorb.

The same conclusion — think before you act — reached from opposite ends of the cost curve. DA is not a return to waterfall. It is arriving at waterfall's instinct from the other direction.

It is like baking bread. Once the ingredients are in and you start to bake, if the bread doesn't taste good or doesn't rise, you don't fix the bread. You make another loaf. So you get the ingredients ready ahead of time and you plan the recipe — but now the bake takes one minute. The planning is not because baking is hard. The planning is because baking is so easy that a bad recipe wastes nothing but your attention, and attention is the thing you cannot get back.

The practitioners who defended waterfall in 1999 were not irrational. They were experienced. They had seen agile's predecessors come and go and concluded, reasonably, that each new methodology was mostly repackaging with new vocabulary. They were right that most of what agile claimed was not new. They were wrong that the underlying shift was incremental.

The practitioners defending agile-with-AI as the appropriate response to this moment are not irrational either. They may be right that better tools improve agile practice in the short term. They are, this book argues, wrong that the underlying shift is incremental.

The pattern says so. The pattern has said so twice before.

---

# **The Bottleneck Has Moved**

*The constraint was never the code. It was always upstream. Execution time was just good enough at hiding it.*

Around 2012, a mobile team at iHeartRadio went on a ski trip.

The trip was a hackathon. Four days, no meetings, build whatever you think is worth building. The lead developer was learning Swift — not because anyone asked him to, but because the potential was obvious and the potential was new and that combination produces a specific kind of energy in a good engineering team. They were not waiting to be told what mattered. They already knew.

By the end of four days, they had built things. Real things. A customer talk radio station concept. A full-screen album art redesign that changed the entire feel of the listening experience. Prototypes that answered questions nobody had been able to get answered through the normal process of design reviews, stakeholder meetings, and prioritization discussions.

Then they went back to the office.

The prototypes sat. Not because nobody was interested. Because it wasn't clear who could decide. The executives had opinions. The design organization had designed, by the CDO's own account, every conceivable UX and UI option. And yet the decisions that would have let the team move — which direction, which experience, what to build toward — did not come.

The CDO said something to the mobile product team that stayed with me. Paraphrased: don't come to a meeting with opinions, because the people you're talking to have better titles.

The team built fast. The decisions moved slowly. The competitive window was wide enough, in 2012, to survive the wait. Nobody felt the full cost of the delay because the delay was normalized into the rhythm of how things worked.

That was the constraint. Not the code. Never the code. The constraint was upstream, invisible to anyone measuring sprint velocity or deployment frequency, and protected by an organizational structure that had confused hierarchy with judgment.

What AI changes in that story is not the politics. It is the cost of the delay.

## **The Constraint Moves**

Goldratt's central insight is simple enough to state in a sentence: every system has one constraint at any given time, and the performance of the system is determined by that constraint.

The five focusing steps that follow are what make it operational. Identify the constraint. Exploit it — get the most out of it before doing anything else. Subordinate everything else to the constraint — stop optimizing what is not the bottleneck. Elevate it — if exploiting is not enough, invest in increasing its capacity. And when it breaks through, go back to step one. Because the constraint will have moved.

That fifth step is the entire argument of this book.

For most of software development's history, execution was the bottleneck. There were not enough developers. The ones you had could only build so fast. The field identified that constraint and optimized against it for two decades. Lean software development. Kanban. DORA metrics. Continuous deployment. Each optimization was applied to the right constraint and each one worked. The organizations that invested in them got measurably better.

The constraint has broken through. Execution, for teams at the frontier of this shift, is no longer what limits the system. But the field is still on step three — subordinating everything to a constraint that has already moved. Continuing to optimize deployment frequency and cycle time is improving something that is no longer the bottleneck. It produces the appearance of progress. The velocity metrics go up. The wrong things get built faster.

Matt Gunter, writing about the misapplication of constraint theory to software, arrives by a different route at the same destination.[^1] His argument against TOC in software is that the flow metaphors break down for knowledge work, that throughput optimization creates what he calls "intention blindness" — it cannot reflect the value of strategic decisions. The real levers, he argues, are not throughput optimization but something else — improving skills, reducing unforced errors, increasing the level of decision quality. He is arguing against the vehicle and pointing at the destination. The conclusion he reaches independently — decision quality — is the one this chapter is built around. Convergent evidence from someone trying to argue the other way is worth more than confirming evidence from someone already on your side.

The constraint is upstream. It is the quality of the decision before execution begins.

## **Decision Latency**

Velocity measures how fast a team executes. It is a reasonable measure of execution speed and a poor measure of anything else.

The metric the field does not yet have a name for is the one that matters most in a world where execution is cheap. Call it decision latency — the gap between when a commitment is made and when its quality is validated.

In the iHeart story, the decision latency was months. The prototypes existed. The options were concrete. But the validation — did we build toward the right thing — arrived slowly, through the slow accumulation of user data, competitive signal, and executive opinion. The execution was fast. The decision latency was long. The constraint was not the sprint. It was the gap between commitment and confirmed direction.

When execution takes weeks, long decision latency is painful but recoverable. You discover in month three that the decision in month one was wrong, you course-correct, you lose three months.

When execution takes hours, long decision latency is catastrophic. The bad decision propagates into artifacts before anyone has asked whether it was right. The doubled code churn is this dynamic made visible. The execution is faster. The decision latency is unchanged. The wrong things are built at speed and the waste arrives before the course correction.

Decision latency is the new constraint. Shrinking it is the new work.

## **The Constraint You Think You Have**

There is a version of this misidentification that is worth naming directly, because it explains why entire sectors are moving slower than they should.

I have watched it happen in healthcare IT. The regulatory barriers are real — HIPAA, FDA clearance, payer integration standards that took decades to partially achieve. Anyone who tells you these do not matter has not worked in a health system.

But here is what the data actually says. When health system leaders are surveyed about the biggest barrier to AI adoption, the top answer is not regulatory uncertainty. It is immature AI tools — cited by 77 percent of respondents. Financial concerns come second at 47 percent. Regulation comes third, at 40 percent.[^2]

The thing most health system leaders cite first in conversation is third in the data.

That gap between the conversation and the data is the diagnostic. The regulation is real. The regulation is also performing a psychological function that has nothing to do with compliance. It is providing the story that makes the real constraint — immature infrastructure, missing talent, slow decision-making — feel like someone else's problem. The external constraint is more comfortable than the internal one. Regulation is a wall you can point at. Decision-making speed is a mirror.

What makes this pattern durable is that it is self-reinforcing. The organization that identifies the wrong constraint invests in managing it, builds reporting structures around it, develops institutional expertise in navigating it. That investment creates its own justification. The people who have spent three years managing regulatory risk are not wrong that regulatory risk exists — they are wrong that it is the binding constraint, and they now have careers that depend on not seeing the difference. The external constraint stops being a misidentification and becomes an identity.

This pattern is not unique to healthcare. Every organization pointing at an external constraint while the internal one goes unnamed is doing the same thing. "Technical debt" can be a version of the same misidentification — teams fixing code when the real problem is decision quality upstream, velocity treated as a vanity metric while the constraint it measures has already moved. The question is always the same: what would you do if the external barrier were removed tomorrow? If the honest answer is "we still could not move quickly," you have been managing the wrong constraint. Possibly for years. Possibly while building an organization optimized to keep managing it.

## **The Boundary Condition**

There is a version of the Mastercard story that belongs here as a boundary condition — and it is worth understanding why Click to Pay existed before understanding why the constraint theory breaks against it.

Click to Pay was born from a relevance crisis, not a technology problem. As Apple Pay, Google Pay, and other wallets proliferated, they used the Visa and Mastercard rails invisibly. The acceptance mark — the thing that once told a consumer *this place takes your card* — stopped meaning anything when every place took everything. The brand was disappearing into the infrastructure it had built. Click to Pay was the response: a product designed to solve a relevance problem, organized as if it were solving a technology problem. That misidentification — strategic constraint dressed as technical constraint — is the healthcare pattern from earlier in this chapter, operating at the scale of a global payments network.

At scale — three hundred or more developers, multiple competing institutions, decisions that required alignment across Visa, Mastercard, American Express, and Discover before any code could be written — the constraint was not execution and it was not decision quality in the traditional sense. It was decision authority. Nobody could say yes in a way that meant yes. The committee's real function was not to make decisions but to provide political cover for the absence of decisions.

AI would not have helped that. AI might have made it worse — faster execution of a direction nobody was actually committed to, amplifying the incoherence before the political process had time to quietly bury it.

This is the boundary of the argument. When decision authority is so distributed across competing interests that yes cannot be said at all, the constraint is not decision quality. It is organizational structure. That is a different problem, and this book does not solve it.

How common is that situation? More common than the framing of "boundary condition" implies. Enterprise software teams, government contractors, any organization where multiple institutions must align before a single line of code can be committed — these are not rare. They are a substantial portion of the industry. The Mastercard dynamic is not an edge case. It is the normal operating condition for a significant fraction of the people reading this book.

What this book addresses is the iHeart situation: capable people, real potential, decisions that could have been made but weren't, because the structure around decision-making was unclear and the culture was hostile to the expression of informed opinion. If you are in that situation, the framework in the following chapters is for you. If you are in the Mastercard situation, the framework will not be sufficient. Knowing which situation you are actually in is itself a decision-quality problem — and it is worth solving before you go further.

## **What This Means for the Metrics**

Velocity will not disappear. It will be demoted.

The useful analogy is heart rate. Heart rate is real. Monitoring it tells you things worth knowing. But no serious athlete optimizes for maximum heart rate. It is a health indicator, a lagging measure of effort expended. Optimizing for it directly selects for stress rather than fitness.

Velocity is the heart rate of software development. Useful to monitor. Dangerous to optimize. The organizations that built their entire performance culture around it will find, as execution costs fall, that they have tuned an instrument measuring something increasingly peripheral.

Decision latency will become the primary metric for teams at the frontier. Not because it is easy to measure — the field does not yet have standard instrumentation for it. But because it is the measure that corresponds to the actual constraint. Speed at low quality produces more waste faster. Quality at low speed produces the iHeart hackathon — right direction, wrong pace. Quality at high speed is what Deliberate Alignment is designed to produce.

The hackathon worked, imperfectly, because it changed the cost of decision-making. A tangible prototype is cheaper to evaluate than an abstract proposal. The executive who cannot decide between two UX directions described in a document can sometimes decide between two they can actually use. The concreteness reduced the decision latency — not by speeding up the process, but by changing what the process had to evaluate.

That instinct — make the decision easier by making the options real — is the same instinct behind what this book will name in two chapters. The difference is that in 2012 the hackathon took four days to produce the prototypes. Now the prototypes can exist before the meeting that will decide between them.

The constraint is the same as it always was. The cost of carrying it has changed.

*Velocity measures how fast you move. Decision latency measures whether you moved in the right direction. Only one of those was ever the constraint.*

---

[^1]: Matt Gunter, "How 'Theory of Constraints' misguides software improvement," Medium, March 2024.

[^2]: "Adoption of artificial intelligence in healthcare: survey of health system priorities, successes, and challenges," *Journal of the American Medical Informatics Association* 32, no. 7 (2025). Scottsdale Institute member survey, Fall 2024, 43 responding US health systems. https://academic.oup.com/jamia/article/32/7/1093/8125015

---

_Copyright Walter Reid, 2026. All rights reserved._

