# CHAPTER EIGHT
# Personal Software as a Service

*The template existed because custom was expensive. That is the only reason it existed.*

Think about the last time you built a website.

If you are old enough, you remember when building a website meant hiring someone. A developer, probably a designer, possibly an agency. The cost was real — not because websites were technically difficult in some absolute sense, but because the people who knew how to make them were scarce relative to the demand. Custom was a luxury not because it was inherently expensive but because the skilled labor required to produce it was.

Then templates arrived. Squarespace. Wix. WordPress themes. A competent person with no technical background could produce something that looked professional in an afternoon. The bespoke website did not disappear — there were still agencies, still developers, still budgets for organizations that needed something the templates could not provide. But for most people, most of the time, the template was good enough. And good enough at low cost reliably defeats excellent at high cost for the majority of use cases.

This was not a technology story. It was an economics story. The barrier was cost. When cost fell, access widened. The template won not because it was better than custom but because it was close enough, and close enough for free beats excellent for thousands of dollars almost every time.

Now think about what happens when AI makes custom the same price as template — when the bespoke website costs the same as the Squarespace website and takes the same afternoon.

The template's value proposition does not erode. It evaporates. Not because the template is worse than it was. Because the reason you ever accepted it is gone.

That is Personal Software as a Service.

## What Nobody Will Build for You

There is a category of software that has never existed, and its non-existence has always made perfect sense.

Call it the sensible-for-one. The dashboard that would transform how a particular team tracks their particular work, configured precisely to the decisions they actually make rather than the decisions a product manager imagined they might make. The workflow tool that reflects the real sequence of how a specific organization does a specific thing, rather than the idealized sequence that looks clean in a demo.

Adobe will not build Mastercard's image editing tool. Not because it is beyond Adobe's capability, but because the economics of building for one customer never worked. The development cost, the maintenance overhead, the support burden — these are fixed costs that only amortize sensibly across a large enough user base. Adobe builds for millions and accepts that the tool will fit none of them perfectly. Mastercard uses Photoshop and accepts the gap between what the tool does and what they specifically need, because the alternative was always a custom development budget that could not be justified.

That logic is dissolving. When execution is cheap enough, the sensible-for-one becomes buildable. Not by Adobe, who has no incentive to narrow their market. By Mastercard itself, or by whoever they ask, in a fraction of the time and cost that made the calculation impossible before. The software is not a product in the traditional sense — it will never be sold, never be marketed, never be maintained by a team of engineers whose salaries depend on its continued existence. It is simply the tool that fits, built because building it is no longer prohibitively expensive. And the sensible-for-one includes the sensible-for-career: when execution is cheap, the artifact that proves what you can do and the product you are trying to sell are the same thing. The demo is the portfolio. The portfolio is the product.

An entire industry — the software-as-a-service industry — was built on the gap between custom and template. The business model was: we will build a tool that is 80 percent of what you need, charge you a monthly subscription, and you will accept the 20 percent gap because building the 100 percent version costs more than the gap is worth. When that gap closes, the subscription model does not automatically fail. But the companies that built for that gap will have to find a different answer to the question of what they provide that you cannot now provide for yourself.

## Where PSaaS Does Not Arrive

Not everywhere. And the places where it does not arrive are instructive about why.

Financial services has a layer of infrastructure — EMVCo, SWIFT, ACH, clearing and settlement systems — that has genuine structural protection. Not regulatory protection, which can be removed by a change in administration. Structural protection: a coordination solution that required decades and the participation of thousands of institutions to build. No single actor can unilaterally replace it. The alternative to the current clearing infrastructure is not a better clearing infrastructure. It is coordination failure across the entire global financial system.

The same logic operates at smaller scales. A franchise network's legacy CRM — the system through which the franchisor tracks every franchisee's operations, clients, and compliance — is a miniature version of the same coordination lock-in. No single franchisee can unilaterally replace it. The data is held in the franchisor's system, often without easy export. The franchisee who wants to adopt a better tool has to run both systems during the transition, doubling operational complexity at the moment they are most vulnerable. PSaaS has to work around this kind of lock-in, not replace it — which in practice means building scrapers and integrations that extract the data the franchisee already owns but cannot easily access.

PSaaS arrives at the product layer above this infrastructure — the interfaces through which consumers and businesses interact with their money, the advisory services, the credit models. None of those are protected by the structural logic that protects the protocol layer. They are protected by incumbent advantage and switching cost, which are real but not permanent.

This distinction matters because it is the clearest boundary condition in the book. The structural protection at the protocol layer is not about execution cost. It is about the coordination cost of replacing something that thousands of institutions agreed on over decades. AI does not reduce that cost. It does not even address it. When someone claims that everything is disrupted, the protocol layer is the honest counterexample.

But the product layer above it — the layer most people in financial services actually work in — is a different story. The bank whose value was in the relationship and the judgment has an easier path than the bank whose value was in the analysis and the report. The analysis is being commoditized. The judgment is not. If you work in financial services and you are not certain whether your value is in the protocol layer or the product layer, that uncertainty is the answer.

## What Changes When the Tool Is Shaped by You

When the software is shaped entirely by your context — your workflow, your specific needs, your taste in how information should be organized — something about the relationship between you and the tool changes.

Software has always been a cognitive prosthetic. You do not just use a spreadsheet; you think through it. The structure the tool provides becomes the structure of your thinking, at least for the duration of the work. Your notebook is not separate from your thinking. Your calendar is not separate from your sense of time. The tool that organizes your work is not separate from the work.

What PSaaS introduces is the possibility that the tool was shaped by the thinking before the thinking happened. Not a preference saved in settings. The software reflects a genuine model of how you work, what you value, what decisions you actually face. The gap between the tool and the thing it represents — a gap that has always been present, always required cognitive overhead to bridge — closes.

What this does to identity is genuinely unclear, and I want to say that plainly rather than resolve it prematurely.

Chapter Seven described the end of borrowed identity — professional roles carrying more self-definition than people realized, and what happens when that carrier dissolves. PSaaS introduces a related but different question. If the software is shaped by you, and the software becomes a significant portion of how you do your work, and that work is a significant portion of how you understand yourself — where does the software end and you begin? The identity that detaches from the title does not disappear. It may reattach to the tools that now carry the work — tools shaped by the person, reflecting the person, becoming difficult to distinguish from the person's professional self.

That question is open in a way I think is important to preserve rather than resolve. The economic argument for PSaaS is solid. The question of what it means for a person's relationship to their tools, their work, and their sense of themselves when the tools become genuinely biographical — that question I hold loosely. Chapter Ten will say so explicitly, with a confidence score attached.

## What PSaaS Is Not

PSaaS is not personalization. Netflix has been doing something called personalization for years. It is a template that adjusts to your behavior. PSaaS is the absence of the template. The distinction is fundamental.

PSaaS is not a product category. There is no company that will sell you PSaaS. It is an emergent property of what happens when execution costs approach zero. You will not subscribe to it. You will arrive at it the way organizations arrive at any capability that used to require specialists: first with surprise, then with wonder at why you waited.

And PSaaS is not automatically good. A tool shaped entirely by one person's model of their own work reflects that person's blind spots as faithfully as their strengths. The template, for all its limitations, embodied the accumulated decisions of a product team that had thought carefully about common use cases. The bespoke tool embodies the thinking of whoever specified it, which may be sophisticated or may be a calcification of how someone has always done something in a way that prevents them from discovering a better way.

There is a harder version of this. I built a synthetic media platform in four days — fifteen AI columnists with maintained voice consistency and ideological positioning across the political spectrum. The economics work. The quality is high enough that a casual reader would not know the writers are not human. I proved the concept and refused to deploy it commercially. Not because it was bad. Because the taste function — the same function this book has been describing in rooms and teams — fired on the decision to build, not on the thing being built. The depth function heard what was possible. The taste function said it wasn't good enough — not in quality, but in ethics. The authority function, which in this case was me and only me, said no.

That is PSaaS meeting its own boundary condition. The sensible-for-one that is dangerous-for-everyone. The framework applied not to a product decision but to a moral one, with all three functions present and held by a single person. The decision was don't ship. The economic argument was strong. The judgment overruled it.

The assumption that personalized is always better — that assumption requires scrutiny the field has not yet given it.

The website analogy is useful precisely because it is not exotic. Everyone has either built a website, paid for one, or accepted a free template and quietly resented the parts that did not fit. The journey from bespoke to template to AI-enabled bespoke is not a journey that requires technical sophistication to understand. It requires only the willingness to notice that the reason you accepted the template was always economic, and to ask what follows when the economics change.

*Custom was never the luxury. The economic barrier was the luxury. We just got used to thinking they were the same thing.*

