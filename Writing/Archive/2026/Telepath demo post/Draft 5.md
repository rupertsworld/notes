# What does an intelligent personal computer look like?

What happens if you take the idea that AI is going to revolutionize computing seriously?

You might argue we're already doing this as an industry: we've spent untold billions on frontier models, hype is at fever-pitch, and it seems every app on your computer now has a chat sidebar.

On the other hand, I've found there's a surprising blind spot around *what* exactly comes next. Most companies are waving their hands broadly at the idea of "AGI", and yet at the same time continue to iterate on pre-existing form factors, app distribution models, and user behaviors that are anchored firmly in status-quo.

So, what does an AI-native computer actually *look* like? *Feel* like? And how can we anticipate and build for this future if we don't have a clear picture of it?

What we need is a good demo. I've seen the power of collective imagination that a well-executed demo unlocks. At Google Creative Lab, demos I gave turned into experiences we shipped to millions of users. At Adept, a demo our 3-person design team gave one Friday afternoon led to a tectonic shift in company direction by Monday morning.

So a few months ago, we at [Telepath](https://telepath.computer) set out to create a compelling demo of what an AI-first personal computer will actually look like. We're trying to build one, after all.

My co-founder Stephen Hood presented it at Betaworks Demo Day this past November:

[VIDEO](https://www.youtube.com/watch?v=jEm5SkLMap0)

In the video above, Stephen plays the role of a knowledge worker approaching his computer with five minutes to spare. He sees a new piece of information, and follows a thread of research before landing on a compelling premise for a piece of writing, which he puts aside to follow up on later.

This workflow — synthesizing a large amount of information down to a usable insight — is a central, critical part of many kinds of knowledge work: writing an article, drafting a company memo, deciding on product strategy, or creating a presentation. However, the way Stephen approaches this problem with the Telepath Computer is a significant departure from a typical, legacy computer today. Instead of dealing with endless feeds, content scattered throughout apps, browser tabs, and tedious workflows, he navigates fluidly through a calm, dynamic interface that helps him make sense of his information landscape, and responds directly to his intent.

Let's break down some of the key ideas behind this demo, and why we think they are an inevitable part of our future.

## The generative interface

The most striking thing about this computer is that there are no apps. Instead, the interface is **generative**, meaning that a significant portion of the user interface is synthesized and/or composed on the fly in response to user intent, as opposed to being programmed ahead of time by a team of developers and shipped.

This manifests itself as a series of cards that materialize as Stephen talks with his computer, representing all sorts of things from objects of discussion (an article or an email, for example) to dynamic displays of information (like a chart showing public opinion on a topic). There is no strict restriction on operations that can be taken with these objects – when Stephen asks the chart to filter commentary from over a month ago, he doesn't have to go hunting through a menubar to see if there's a "filter" button, or switch apps to one that can filter – he just speaks and the system complies.

![[graph.png]]

This brings us to the primary benefit of a generative interface: it massively closes the gap between intent and outcome. For many tasks, it's easy to express our goal in natural language and have the computer work out the exact steps to achieve it (so long as this system can be made predictable & reliable). It's much harder to find the right app or multiple apps, learn a new interface, work around any constraints, and perform all the steps yourself (provided the app actually has all the features you need).[^1]

The net effect of this is not just that we can achieve more tasks with less effort and frustration, but also that for everyday users *agency* over their computer skyrockets. A generative interface means the space of possible actions, and the possible ways information can be displayed, is infinite. Have you ever used an app but wished it worked differently? Been confounded about how to achieve something with the apps you have? Lamented a nonsensical change in a product you love? These are problems inherent in the app model, that go away when software is generative.

## Structure amidst flexibility

The greatest risk for any generative interface is disorienting the user. Good software design gives users a conceptual model of the system, so they can accurately predict what will happen when they perform an action. If we allow an agentic system free reign over our computer screens without structure or constraints, aren't we setting our users up for a chaotic and unpredictable environment? How will they know what they *can* do, and what will happen when they *do* it?

One solution is to package up generative software in app-like bundles, and try and keep the same metaphors we have today. In other words, a generative UI just means anyone can generate their own app. This approach is tempting — we're already seeing several startups coalescing around it — however, it's a skeumorphism that constrains our thinking to the idea of making and bundling apps the old way, not having a dynamic interface that responds to our intent on the fly.

Instead, we solve this problem by giving our interface a well-defined "laws of physics". We provide a logical structure, through a 3D space where the computer can place the cards on which its interfaces are painted. Cards adhere to the same interface conventions, and behave the same way within the space, while permitting arbitrary UI on their surface. 

![[strategic-note.png]]

This structure enables what I've been calling the "show and tell" metaphor — mimicking how humans tackle complex work in real life: an ephemeral discussion about the work at hand, while assembling artifacts and references on a shared surface. This is a departure from chat, where conversational responses and actual content intermingle in one long thread. Here, we split them out. Conversation is ephemeral, just like in the real world. But anything can be made permanent by placing it onto the canvas, where the user can interact with it, file it, grab it — treating it like a first-class object rather than just a chat response.

## Deep personalization

At the outset of the demo, Stephen asks the computer: "I have five minutes, what's up?"

To answer this question effectively, the computer needs a model of the user and their information landscape. It has created this model through constant analysis of the user's notes, emails, and other information sources, as well as their behaviour while interacting with the system. In response, it assembles a dashboard showing the status of nine items that Stephen might want to attend to within that timeframe.

![[dashboard.png]]

This is *deep personalization*: the ability to make sense of the user's digital world, construct a model of them — their interests, beliefs, projects, values, relationships — and assess all new information and all generated interfaces against that model.

One discovery we made during our design process was that deep personalization is not just a useful feature for agentic action-taking; it's also a *requirement* for an effective generative interface.

By definition, a generative UI is both deciding what information to show, and crucially, what to leave out. Our interfaces today are ineffective in this regard: their only option is to show us everything. Every email, message, note, webpage, document, and notification, constantly pouring unfiltered into our screens for us to handle manually. (One exception is social media, though this is done in a very limited domain and with an algorithm that's entirely *out* of our control — another reason these computers need to be under our control).

Telepath's generative UI solves this problem by acting as an intelligent filter, with the ability to anticipate what information will be most important for us for any given moment or task. In order to do that effectively you need a deep understanding of the user, otherwise the system is bound to make decisions that either remove important information, or highlight something irrelevant. When the interface and the information presented within it is a creative decision made at runtime, we need to ensure that the system is well-equipped to make those decisions accurately and reliably for the UI to be effective.

## Process & acknowledgements

We created this demo through a process that combined equal parts evidence and imagination[^2]. We interviewed computer users to identify general problems that presented themselves as fundamental to the computer, across many use cases. Then we zeroed in on specific knowledge synthesis & artifact creation workflows to investigate those further. We combined insights from these interviews with our forecasts of where we saw capabilities emerging, especially around local models (which will run constantly on-device far more efficiently in the future), voice synthesis, and code generation. We made educated guesses of where the future is headed, read up on historical context, and watched a bunch of sci-fi and prior art, before sketching the first concepts and iterating from there.

On that note, it's important that I acknowledge work that inspired us. Foremost, the Apple Knowledge Navigator concept spearheaded by John Sculley, which while comically dated in some ways is a great example of the creative power a product demo can have. It predicted the web, voice assistants, and touch-screen tablets long before any of these existed, and you'll see many nods to that video in our demo of the Telepath Computer.

Other notable mentions:

- [Mercury OS](https://www.mercuryos.com/) by Jason Yuan, a speculative vision for a fluid, intent-driven operating system based around modular cards that influenced Telepath's card metaphor. 
- [Desktop Neo](https://desktopneo.com/) by Lennart Ziburski, which was a great example of how to take emerging capabilities (multi-touch, voice control) and apply them to real user benefit.
- The film *Her*, not necessarily for its depiction of AI (there's a lot we don't want to emulate there...) but rather its humanistic, depth-based, textural screen design that encouraged us to play with depth.
- Matt Webb, whose thinking on conversational interfaces helped shape our "show and tell" metaphor.

I hope this work encourages others in the industry to consider more deeply an optimistic vision of where they want this technology to go to, with more clarity & fidelity than just saying "AGI". And, to share that broadly to the world so we can discuss and create that future together in the open.

If you'd like to follow along with Telepath's progress on making this a reality and get access to our Alpha program, we'd love to welcome you [here](https://telepath.computer).

[^1]: If you want proof of this, ask your nearest computer programmer how much code they write themselves vs. how much they now generate using natural language instructions.

[^2]: With evidence alone, you can only iterate. With imagination alone, you are only guessing.
