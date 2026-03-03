# We need to re-think the whole stack of computing.

The entire tech stack so far is a result of computers not understanding us:

- Ever since the first computers, the fundamental unit of computation has been boolean logic operating on bits.
- We told them what to do by explicitly patching pathways through these logic gates. These were essentially the first programs, and the first interface – the way we told computers what we wanted them to do.
- Over the years our interfaces to this got more user-friendly. We developed punchcards, and the Von Neumann architecture to store programs in memory, then higher-level abstractions like operating systems and the command line.
- Later, a huge shift that moved from text-based linear programs to a desktop-based graphical user interface with menus, buttons, clicking and dragging. The concepts of "apps" as bundles of functionality we can ship over the internet to your computer.
- But underpinning it all, is this. All that activity is translated down to this one-or-zero bit, and logic gates that operate on it. The consequence of this is that *someone* needs to explicitly instruct a computer what to do. Sometimes that's the maker of the device itself, sometimes it's the operating system author, sometimes the application author, and sometimes it's the user. But it's always *someone* explicitly instructing.
- This is what all of us probably do for our careers. We tell computers what to do.
- And we've gotten really good at it! We've developed an entire stack to help us tell computers what to do – we ship applications to users, have operating systems to give those apps higher-level abstractions to deal with, we've developed protocols and file formats to allow interoperability (or at least we try), and we have a sophisticated GUI to allow users to enter the discrete subset of instructions we've determined that they are allowed to make. This is the modern computing stack.

But now, we have this new fundamental material that *does*:

- Then these came along. This is a neural network, but we've had similar machine learning systems for a while now. The interesting thing about machine learning is that it is a mathematical system that relies on *learned* associations and behavior instead of *pre-programmed* behavior. That makes these systems really great at, for example, detecting a stop-sign if you're a self-driving car. There's no way to effectively specify every iteration of a stop sign in code, you need to learn the fuzzy associations between pixels from hundreds of thousands of images.
- Here are some completely novel properties of machine learning models that make them a radical departure from conventional computing:
	- They are probabilistic, not deterministic.
	- They are generative, meaning
	- They can handle fuzzy problems, they don't require precise inputs & output formats
- But right now, we're focused on peppering our existing computers with bits of machine intelligence. We're putting AI chatbots in apps, creating sidebars, and developing computer use agents to browse the web and put things in shopping carts. But we aren't *yet* treating these models as fundamental primitives of computing.
- *Tell the tale of the horse cart & adding the combustion engine to it.*
- But soon we will begin unraveling that structure and rethinking the pieces that were built in a pre-machine intelligence world. This is how we get to the true form of the new personal computer.

# What will that new kind of machine look like?

- My company, Telepath, is focused on creating a new kind of personal computing experience, built from the ground up with machine intelligence. Let me show you a demo of what that looks like
- [DEMO]
- 

At the core of our stack is how we package & distribute software at the moment: apps.

Why apps exist:

- First and foremost, because we need to write programs to tell the computer explicitly what to do at all times. "Computers" *must & can only* follow explicit instructions.
- Because users can't easily make their own software, we need others to make & ship it. This means we freeze functionality and interface ahead of time, and the user can use that to edit the data underneath. That’s the layer they indirectly play with.
- Because we need components of the system to work well together, we package it in an app where we can author all the components to fit together (but if things are squishy, you don't need to). When we need separate pieces of the software created by different authors to interoperate, then we utilize standards (protocols, formats, etc) to allow this. 

The app model has been wildly successful (see app store, web app ecosystem, etc.) – it allows us to distribute software at scale, and form many businesses around solving users problems.

But it also leads to downsides. We can never completely solve a user's problem, we're incentivized to solve a large set of problems for average users (image of feature requests). The app model leads us to confine functionality, appearance and behavior based on what the author thinks is right, and the subset of scenarios the author considers, as opposed to the needs of the user (in general, or in the current moment).

Of course, now: we *don't* need to write programs to tell the computer explicitly what to do, users *can* create their own software at scale, components of systems *can* work together without being explicitly programmed to.

And allowing the user/system on the fly has huge benefits. Applying the flexibility of LLM output to *everything* not just text. 

Unsure exactly what happens here, but prediction that we break things down into file-like objects with types, views, and functionality. We might have default couplings of these things, but they aren't the be-all and end-all. We will see new distribution & monetisation models for software as a result. Perhaps a bifurcation of small and large pieces.

Smalltalk analogy? Where this decoupling has happened before.

# What does that mean for the web & software?

If the web was just content, I don't think much would change. But because it's content, display, and functionality all bundles into apps, it probably will change a lot.

The web is not a set of technologies (podcast), it's a set of values applied to technologies – and it can be instantiated in lots of ways.

A spectrum – where authorship is important, more of this will happen at the author side. Where it isn't more of it will happen at the consumer side. But regardless, it will not be guaranteed that your content will have your design/functionality. The final evolution of responsive design!

The huge, highly-capitalized players are fighting for their lives too! And this happened back in the early web era too.

- We ought to all be curious and start to play an active role in how things go here. 
- Moving from web apps to data stores. 
- ... does this industry just go away? Maybe... except for designing the systems themselves, and specialist applications.
- A lot more power shifting to the OS

---

Algorithms vs. learned parametrizations. The "program" isn't written in the gates, it's encoded in weights that were discovered through training. The boolean substrate is doing something categorically different than it does in classical programming.

Right now these models supervene on bits, but that's not necessarily always going to be the case. ML models are to bits what logic gates are to vacuum tubes. We may find a better layer underneaeth.

Metaphor of "jelly" and "bricks". Squishy vs  rigid.

Maybe we want to focus specifically on what software becomes & how we distribute it. Like what a web app breaks down into, as opposed to the other parts fo the stack

Apps & protocols were the only way to ensure interoperability. Will we really need protocols that much anymore?

- **Agentic kernel.** Much like we have many computational processes constantly happening on our computers, automated network requests, etc. this will be occurring constantly with a symphony of agentic/"squishy" processes orchestrated by an agentic scheduler.
	- "Sensemaking" as a core part of that process. An understanding computer.
- **Dissolution of apps.**
- **Change of how we store & retrieve data.** It will be less important that things are stored in a particular directory on disk, and more about how one piece of information relates to others, semantic meaning about that data which can now be automated, etc.
- **Network of information, not applications**
