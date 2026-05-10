**CHAPTER THREE**

# **What Agile Got Right (And Why It's No Longer Enough)**

*This is an autopsy, not a eulogy. The patient solved the right problem. The problem changed.*

Every Thursday afternoon, a small team working on a consulting project meets for three hours around a rectangle table with a screen at one end.

For the first fifteen minutes, they run through the ritual: what did you do last week, what will you do this week, any roadblocks. It is a standup stretched to fill its container. It produces the expected output — a shared sense that everyone is accounted for, that progress is happening, that the team exists.

Then something shifts.

From about fifteen minutes in to fifteen minutes before the end, the meeting becomes something else. The screens come out. People show what they actually built. The work connects to other work. Decisions get made in real time because the options are visible to everyone simultaneously. The person who has been working in the background through most of the meeting — quietly building in his code editor while the others talk — surfaces what he has done and it changes what everyone thought was possible.

For two and a half hours, the room works. The alignment that the rest of the week fails to produce arrives, unbidden, in the space between the ritual and the closing roundup.

Then the meeting ends. The week resumes. The work continues, parallel and mostly uncoordinated, until the next Thursday.

This is not a description of agile failing. This is a description of agile's best instinct — get the people together, make the work visible, let alignment emerge from proximity — fighting against the container that agile built to hold it. The sprint is a two-week version of what this team does in three hours. The standup is a daily version of the check-in that the first fifteen minutes provides. The retrospective is the debrief that nobody has time for before the next week starts.

The instinct was right. The container has outlasted its purpose.

## **What the Manifesto Actually Said**

The Agile Manifesto has been both over-applied and under-read. Over-applied: the practices that emerged from it — scrum, kanban, SAFe, the entire apparatus of agile transformation consulting — were built on top of the manifesto's values in ways that its authors would not all recognize as faithful. The ceremonies became mandatory. The roles became job titles. The velocity metric became a performance evaluation. The thing that was supposed to make work more human became, in many organizations, a new kind of bureaucracy with its own vocabulary and its own priesthood.

Under-read: every one of its four values was a deliberate inversion of a specific waterfall pathology. And every one of them points, if you follow it far enough, toward something that has not changed and will not change with the next shift in cost structure.

Customer collaboration is more important now than it was in 2001. Responding to change is more important now. The manifesto's values did not expire. The structures built to implement them did.

## **The Structures That Were Scaffolding**

The sprint is a container for work that takes time to complete. When work completes in hours, the two-week sprint does not accelerate — it becomes a holding pattern. The work is done before the sprint review. The sprint planning session is allocating capacity that has already been consumed.

The standup asks three questions: what did you do yesterday, what are you doing today, what is blocking you. When work moves faster than the standup cadence, the standup is reporting on history rather than coordinating present activity. It becomes a ritual of accountability that nobody believes in but nobody stops performing.

The backlog is a queue for execution capacity. It assumes that the scarce resource is developer time — that ideas are cheap and implementation is expensive, so you maintain a prioritized list and work through it in order of value divided by effort. When implementation approaches free, the backlog is no longer a prioritization tool. It is an anxiety archive. A list of things that might matter, maintained against the day when someone has time to consider them, in a world where time is no longer the constraint.

None of this means these structures were wrong. They were right, for their constraint. The sprint was a rational container for work that genuinely needed two weeks. The standup was a rational coordination mechanism for teams whose work moved at human speed. The critique is not that these structures were badly designed. It is that they were designed for a specific cost structure and that cost structure is changing.

The one agile structure that survives the shift almost unchanged is the one that was always the most honest: the spike. A time-boxed experiment — build it to learn whether it is worth building. The spike was agile's concession that sometimes you cannot know until you see it, that specification is insufficient and you need the artifact itself to evaluate the direction. When execution takes minutes instead of sprints, the spike is no longer an experiment. It is the product. The demo day is the launch. The distinction between exploring and shipping dissolves because the cost of exploring has fallen to the cost of shipping and neither one is large enough to justify a boundary between them.

I built a synthetic media platform — fifteen AI columnists with maintained voice consistency and ideological positioning — in four days. Designer, developer, visionary, marketer. All one person. That was a spike, except the spike was the finished product. And the demo was not for a billion-dollar launch. Maybe it is for the next consulting engagement, or a role that values the judgment more than the job title. When execution is cheap, the portfolio and the product are the same artifact.

One of the sharpest observers of the agile world wrote recently that the biggest threat to agile practitioners is not that AI will replace them — it is that AI will reveal what many organizations already suspected: they never needed agile practitioners. They needed someone to manage Jira.

That is not a dismissal of the people. It is a diagnosis of the structure. The people who were doing real work — understanding what needed to be built, synthesizing conversations into a coherent direction, being present enough with the client to hear what they meant rather than what they said — those people were doing real work before and will be doing real work after. The Jira management was always a side effect of a system organized around execution.

## **The Predecessor Concept**

Before agile had a name, Kent Beck was doing something called paired programming.

The conventional interpretation is efficiency: two developers at the same keyboard produce better code faster because one types while the other watches for errors, because they keep each other focused, because the constant explanation of what you are doing surfaces assumptions you did not know you were making.

That interpretation is not wrong. But it misses what Beck was actually onto.

The pair was not primarily a code quality mechanism. It was a decision quality mechanism. The moment of value in paired programming is not when the second developer catches a syntax error. It is when the second developer says "wait, why are we doing it this way?" and the question surfaces an assumption that, once examined, turns out to be wrong. The typing is almost irrelevant. The real-time interrogation of the decision being made while the decision is being implemented — that is what paired programming was actually producing.

Beck's insight was that two minds on a problem in real time produces better outcomes than one mind followed by a review. The review model has a fundamental flaw: by the time the evaluation happens, significant investment has been made in the direction being evaluated. The cost of changing course increases with every line of code written. The paired model collapses that gap to near zero. The evaluation happens while the decision is still live.

This is the ancestor of what the next chapter will name. Not the typing together. The real-time evaluation of the decision, at the moment of the decision, before the investment has been made.

Beck applied this insight to two developers and a keyboard. The extension is: what if you applied the same logic to the decision that precedes the code? What if the pairing happened not between two developers but between the person who understands what the client needs, the person with the taste to catch where the answer is defaulting to mediocrity, and the person with the authority to commit? What if the real-time interrogation happened at the moment of specification rather than the moment of implementation?

Paired programming was pointing at something beyond code.

## **The Failure That Isn't Agile's Fault**

Return to the Thursday meeting.

The team running the Zansei project — an AI-powered marketing consultation tool for small businesses — has been using a version of agile since October 2025. Weekly standups. Thursday collaboration sessions. A backlog of features and client requests that keeps growing as the client's ambitions expand.

By any agile metric, the team is functioning. They meet regularly. They review work. They plan the next cycle.

And yet the project is accumulating a specific kind of dysfunction that agile was designed to prevent. The product's scope keeps expanding because the person with authority to commit has updated his mental model of what AI can do and generalized it recklessly. New client relationships are producing requirements that don't cohere with each other or with the original product vision. The person doing research to improve the product is producing seventeen-page reports to answer questions that were never clearly enough defined to be answerable. The ads keep running while the funnel produces nothing.

There was a Thursday in February when the researcher presented a seventeen-page report on the site's copy. Half-done, he said. The other half would be ready the following Thursday. The team was spending a thousand dollars a week in ads. Zero people had completed the funnel in the previous seven days. What came over me in that moment was not anger — anger would have been easier. It was something quieter and more final: the realization that I could generate new copy with AI and run an A/B/C test that afternoon, and I was sitting in a room where someone needed seven more days and seventeen more pages to tell me what I already knew. I asked him what single question the research was meant to answer. He flipped through the slides. He rambled something about tests. I told Mr. K to turn off the ads. The meeting continued. The ceremonies continued. The dysfunction that produced the report and the silence and the thousand dollars continued, perfectly intact, because the ceremonies had no mechanism for addressing it.

I can indict the researcher because I have been the researcher. At Mastercard, I produced 127 pages of AI-generated product requirements using the OpenAI Playground. It was thorough. It was well-structured. Leadership was impressed. It looked like momentum. It was articulate noise. I didn't use AI to clarify our direction. I used it to dress up our confusion. And the artifact, polished as it was, gave leadership the ammunition to keep moving — on goals that had little to do with product. The seventeen-page report and my 127 pages are the same failure at different scales: using the tool to produce the appearance of progress when the actual problem — what are we building and why — remained unanswered underneath.

The dysfunction had another dimension that the ceremonies could not see. The team's UX designer was generating design variants at AI speed — using Claude to produce web artifacts that simulated complete pages, full visual options ready for review. An artist generating a hundred looks and feels before lunch. But the developer had no design specification to build against. Each artifact looked complete on its own — a single page of JavaScript, CSS, and HTML — but none of them connected back to the database, to the TypeScript codebase, to the actual product architecture. There was no shared language between design and development. The UX work and the development work were moving at different speeds, in different media, producing fragments that looked whole individually and could not connect.

This is the opposite of what Beck's paired programming was designed to produce. Beck's insight was that two minds on the same problem, in real time, interrogating each other's assumptions, produces better decisions. The Zansei team had two people producing AI-assisted work at different speeds with different tools and no shared specification to translate between them. Not a coordination problem — the ceremonies were coordinating fine. A language problem. The work could not speak to itself.

The agile ceremonies are not catching any of this. They are providing the appearance of coordination while the actual problem — nobody in the room can say no with authority, nobody has the explicit function of maintaining the product's integrity against the gravity of scope expansion — continues unchecked.

This is not agile failing. This is agile succeeding at what it was designed to do — coordinating execution — in a situation where execution is not the constraint.

## **When the Denominator Disappears**

The prioritization framework the team tried to use was weighted shortest job first — WSJF. Divide business value by job size and time criticality. The result is a priority order. It is a rational framework for a world where execution capacity is scarce: given limited capacity, what should we build first?

It stopped working for an interesting reason.

When execution cost approaches zero, job size collapses. Everything becomes equally small. The denominator that used to differentiate the list converges toward a constant, and what you are left with is a list ranked only by business value — which is exactly what nobody can agree on, because the product's identity keeps shifting and the person who could anchor it keeps expanding it.

WSJF is really asking: given scarce execution capacity, what should we build first? When execution capacity is no longer scarce, the question it was designed to answer dissolves. The new question is: given that we can build almost anything, what should we decide to build at all?

That question requires a different kind of answer, and a different kind of room to produce it.

## **The Scaffold Is Coming Down**

The field is producing its own successor frameworks, in real time, without yet having a name for what they are converging toward.

Amazon Web Services, in 2026 guidance for teams building AI-native products, suggested that sprint planning must evolve into what they called "Intent Design" — where architecture defines roles, guardrails, and fallback mechanisms rather than scripting every decision path.[^1] The frame has shifted from "here is the plan we will execute" to "here is the intent we will navigate toward."

What the successor frameworks share, wherever they are emerging, is a common move: front-load the thinking, compress the execution, make the alignment the work rather than the precondition for it. The ceremonies that were designed to manage execution are being replaced, in the organizations that are furthest along, by something that more closely resembles the Thursday meeting working at its best.

Not the ritual fifteen minutes at the start. The two and a half hours in the middle where the work is visible, the options are real, and the decisions are made by the people who have to live with them.

That is not a meeting. That is the methodology.

Agile was right about the values. Customer collaboration matters. Responding to change matters. Working software over comprehensive documentation matters. None of that expires.

Agile was right about the instinct. Get the people together. Make the work visible. Close the gap between building and knowing whether the build was right. These instincts are more important now, not less.

What agile could not have anticipated is that closing the execution gap all the way changes what the gap needs to be closed around. When execution is genuinely fast, the gap that needs closing is not between planning and delivery. It is between the decision and the validated direction. Between what the room understood and what the agent built. Between the intent and the outcome.

The sprint was the right unit when building was the hard part.

The room is the right unit now.

What happens in that room, and who belongs in it, is what the next chapter is for.

*The sprint was a container for work that took time. The room is a container for decisions that must be right. They are not the same container.*

---

[^1]: AWS Prescriptive Guidance, "Operationalizing agentic AI on AWS," section "Evolving software delivery for agentic AI," 2026. https://docs.aws.amazon.com/prescriptive-guidance/latest/strategy-operationalizing-agentic-ai/software-delivery.html

