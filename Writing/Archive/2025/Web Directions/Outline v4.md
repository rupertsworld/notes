# Computers are built on boolean logic, and that's fundamentally limiting

Computing is based on bits:

- Since the dawn of computing, fundamental unit has been boolean logic operating on bits
- Here's a simple circuit with a logic gate
- If we arrange enough of these gates in the right way, we can do computation
- When you scale that up, you get a general purpose computer (ENIAC)

So computers ultimately need to be explicitly instructed, and we've evolved more sophisticated ways of doing that:

- ENIAC is a complex set of these circuits, arranged in functional units like adders, accumulators, and multipliers
- Plugging in parts of the machine to make a big algorithm to do what you want as an operator, without having to rebuild the machine.
- Over time we developed more sophisticated ways, like the command line & GUI
- But still, someone has to instruct the computer to do every little thing, by rearranging the logic gates. Very large learning curve, and way to much work, for any individual user.
- We invented applications to solve this. Experts that would gain an understanding of expected/avg. use cases, and ship software to solve it.
- So now we have this sophisticated modern computer, but everything it does needs to be explicitly instructed, and we're only given a small subset of possible actions to do as users.

Our entire lives are digital, and this is now causing problems:

- In the meantime, our entire lives have moved into the digital. Software ate the world.
- Volume problem: we've gone from a few dozen files to thousands of emails, messages, photos, documents, subscriptions, etc. Meaning is buried in a litany of digital artifacts.
- Complexity problem: Modern tasks require coordination across multiple apps, services, contexts, browser tabs, etc. And the burden of translation from intent to explicit apps and steps within those apps falls entirely on the user
- The net effect is that a tool that is meant to be empowering, increasingly feels burdensome, because of this core restriction.

# Computers built on neural networks will be very different

We now have this new material:

- Then neural networks came along.
- This is a neuron. Like a logic gate, it has inputs & outputs, performs a simple computation, and is a building block to a complex system.
- However, unlike a logic gate, it operates on continuous values, and learns patterns, instead of being pre-configured with rules. It's probabilistic, not deterministic.
- So where an algorithm can only react to discrete inputs, a neural network can understand patterns in images, sound, code and language.
- Which means it can be trained to react appropriately to human intent, without specifying in advance *exactly* how this is structured.
- This is a fundamental shift.

New materials lead to new structures:

- When combustion engines were invented, we just put them on the end of horse carriages (Benz Patent Motorwagen)
- It would take 15-20 years for us to land on the design that would evolve into the modern car (Mercedes 35hp)
- And the car we have today is as much a product of its environment as its design – motorways, gas stations, cultural norms, business infrastructure, road rules & regulation.
- The ultimate form of the material takes some time to evolve.
- We're in a similar spot right now with this new computing material. We're taking our existing systems, and layering them with chat apps, sidebars, computer use agents, etc.
- But this is like strapping an engine to a horse cart. The desktop metaphor, windows, button, software distribution, operating systems, applications, all created for a world where we need to program computers to make them do anything.
- That isn't true anymore. A new kind of computer is coming, and it's going to be very different.

# Telepath & our demo

At Telepath, we're focused on creating a new kind of computing experience, built for an era of machine intelligence.

[DEMO]

# Dissecting the Telepath computer

This is a very different kind of computer.

Qualities the demo has:

- Dynamically composed user interface
- Making sense of information
- Deep personalization & understanding of the user
- Proactivity

# Why I think this will happen

We already have the core technologies:

- LLMs are able to understand intent, and translate it into action. Just ask your nearest programmer.
	- Copilot used by 15M+ developers[^1], 90% of Fortune 100 companies adopted[^1]. 76% of developers using or planning to use these tools[^2].
- And trends are accelerating, towards smaller, more capable, and local models that can run on-device. Hardware is catching up, and there is a lot of money riding on solving the security and reliability problems.
	- Inference costs dropped 90% in past two years
	- "Densing law": LLM parameter size for equivalent performance halves every 3.5 months[^3]. GPT-4 class models like Llama 3.3 70B now run locally on laptops[^4] - something unimaginable just 20 months ago

It will provide a step change in user value:

- We've already seen the adoption with ChatGPT when understanding of intent is applied to text output, but we can now apply this to computing more generally
- Volume & complexity problems go away, no longer translating intent through apps but rather just declaring what you want the computer to do. A more delightful experience.
- Ultimately, an increase in productivity and efficiency.

These sorts of shifts are predictable and normal:

- Don't fall into normalcy bias – platforms shift regularly
- CLI → GUI (80s), Web (90s), Mobile (00s)
- Each time similar pattern: new core technology → new capabilities / business models / distribution

Whether it's us at Telepath, or others in the industry, this shift is underway. Multiple companies are racing toward this vision. So what does it mean?

# What this means for developers & the web ecosystem

- Recap: we've taken a journey through the history of computing, I've shown you a new kind of computer, and hopefully convinced you that something like this is coming.
- So what does this mean for the web?
- If you look at the web today, it's a platform for shipping applications, and information (usually both together). Both of these will be faced with upheaval.

Shipping apps:

- Telepath is very different. It's generating and composing interfaces and functionality based on user intent and the task at hand. There are no "apps".
- Instead of shipping a monolithic package, we will ship smaller, composable pieces. We can let the user's system work out what it wants to use on the fly.
- This is confronting. But it also reminds me in a small way of the transition to responsive websites. We're giving up control, but greatly enhancing flexibility and the user experience.
- It's also very web-like. The original idea of a "user agent". The motto of "small pieces loosely joined".

> [The user agent is] a program whose purpose is to mediate interactions with services on behalf of the user under the user's preferences. A user may have more than one user agent, and agents need not reside on the user's desktop, but any agent must be controlled by and act on
  behalf of only the user.
  
Distributing information:

- Telepath is constantly querying information, and using that to give answers and synthesize views for the user.
- So what does information on the web look like now? Oh, it's a disaster.
	- Ad incentives worked at first, but now the incentive misalignment is clear: optimized for attention, not factuality or usefulness
	- And it's only getting worse as AI slop intensifies
	- In tandem, as new clients emerge that control the view layer, the ad-supported web model is unviable. An emerging crisis.
- What we need: a rich network of queryable, high-quality, verified  sources, documents, and structured datasets to allow our machines to make correct inferences.
- How we get there? The only open answer I know is direct payments for information.
- Again – this is surprisingly web-like!
	- Originally, information was *the whole thing*. The web was for sharing linked documents and other media artifacts.
	- "402 Payment required" was part of the original 1989 HTTP spec, still marked "reserved for future use" 35+ years later. Berners-Lee tried to implement it in the late-1990s, but international banking complexity & costs too high (now viable paths).
	- It's also a very real path towards Tim Berners-Lee's dream of a semantic web.

# The web is dead, long live the web

A developer's job is to solve problems for the user:

- Our job has never been to write lots of software, or master React Hooks. We're here to make solutions for users. Those solutions are going to look very different, but we're an adaptable bunch.
- Be prepared to start thinking in terms of services and resources, not apps
- Human-centered work will be important: information architecture, designing & crafting the critical paths, deep understanding of the user & business problems, artistry, taste.
- So will deep technical work: lower-level systems work that's fundamental, building the platforms themselves, making infrastructure, professional software packages that rely on precision and can't be easily augmented.

Our other job is to keep the dream alive:

- What is the web?
- It's a set of technologies:

> The first specifications for web technologies defined URLs, HTTP, and HTML, which were identified as the World Wide Web's core
  technologies.
  
- It's an information space:

> The World Wide Web (WWW, or simply Web) is an information space in which the items of interest, referred to as resources, are
  identified by global identifiers called Uniform Resource Identifiers (URI).

- But it's also a set of ideals:

> ... https://www.w3.org/TR/ethical-web-principles/

- These principles - openness, interoperability, user control - are what really make the web the web. The technologies will change, web apps may no longer exist as we know them, and new things will emerge. But the ideals can endure.
- There's another critical role here for everyone in this room: that's to keep the principles of the web alive.
- A lot of money has been invested in this space. And a big chunk of that money is counting on capturing the user, their information, on companies creating a new super-app or super-platform.
- Yet again, this is not our first rodeo: up until the mid-90s, basically all network traffic wasn't through any sort of open platform, it was CompuServe and AOL. The web came along, and it won.
- We're currently in the "CompuServe & AOL" phase. We need to ensure that open wins this time, it's more critical than ever.
- This is all of our business, and we all have a choice whether to adopt, build, or advocate for this future.
- Join communities, and come help solve some of the many problems that will emerge making this future a reality [Telepath mailing list, user & agents, etc]

Conclusion:

- Here I showed you a computer that works very differently. One that understands intent, composes functionality, mediates information on your behalf. It represents a dramatic shift in the way we think about software, and how we distribute it.
- But I also hope you took away from this that, while this represents a huge amount of change, it's also something we can all get really excited about. And in which the principles we've come to love in this community will endure.
- The web is dead. Long live the web.

[^1]: [GitHub Copilot Has Over 15 Million Users](https://www.thurrott.com/dev/320356/github-copilot-has-over-15-million-users) (Microsoft CEO Satya Nadella, FY25 Q3 earnings call, April 2025)
[^2]: Stack Overflow Developer Survey 2024
[^3]: [Densing law of LLMs - Nature Machine Intelligence](https://www.nature.com/articles/s42256-025-01137-0)
[^4]: [I can now run a GPT-4 class model on my laptop - Simon Willison](https://simonwillison.net/2024/Dec/9/llama-33-70b/)


---






A list of unsolved problems:

- ???