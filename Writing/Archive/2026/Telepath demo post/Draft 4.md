# What does an intelligent personal computer look like?

What happens if you take the idea that AI is going to revolutionize computing seriously?

On the one hand, you could argue we're already doing this: as an industry we're pouring untold billions of dollars into frontier models, and putting a chat sidebar in everything. On the other hand, most companies are iterating on the default form factor of chat and the continued existence of apps, all while waving their hands broadly at "AGI" and how everything is going to change.

But what does an AI-native computer actually *look* like? *Feel* like? How can we anticipate and build for this future if we don't have a clear picture of it?

What we need is a good demo. I've seen the power of collective imagination that a well-executed demo unlocks. At Google Creative Lab, demos I gave turned into experiences we shipped to millions of users. At Adept, a demo our 3-person design team gave one Friday afternoon led to a tectonic shift in company direction by Monday morning.

So a few months ago, we at [Telepath](https://telepath.computer) set out to create a compelling demo of what an AI-first personal computer will actually look like. (We're trying to build one, after all.) My co-founder Stephen Hood presented it at Betaworks Demo Day this past November:

[VIDEO](https://www.youtube.com/watch?v=jEm5SkLMap0)

In the video, a knowledge worker follows a thread of research and lands on a compelling premise for a piece of writing. This insight-to-artifact workflow is central to many kinds of knowledge work — writing an article, drafting a memo, creating a presentation. But the way he's going about this task is a significant departure from a typical computer today. Instead of dealing with individual applications, browser tabs, and a mess of files, he navigates fluidly through a dynamic interface that makes sense of his information landscape and adapts to his instructions on the fly.

Let's break down the key ideas behind this demo.

## The generative interface

The most striking thing about this computer is that there are no apps. Instead, the interface is **generative**: synthesized/composed on the fly in response to the intent of the user. Generative UI is having a moment in the AI world right now, primarily because its now possible to actually implement. But why would we want it? What benefit does it bring the user?

The app model of computing emerged out of necessity: computers are unable to understand our individual goals and preferences or adapt themselves, so they need to be programmed ahead of time to accept discrete, computable inputs for a more generic group of users.

Machine learning removes this constraint. A generative interface collapses the distance between intent ("I want to do this thing") and outcome — no more choosing and installing an app, learning how to use it, and working around its constraints. Have you ever used an app but wished it worked differently? Been confounded about how to achieve something with the apps you have? Lamented a nonsensical change in a product you love? These are problems inherent in the app model.

A generative interface means the space of possible actions, and the possible ways information can be displayed, is infinite. Just as you can ask an LLM to generate text in any format, a generative UI can create an interface of any form. In the demo, Stephen asks the computer to map out public opinion on an issue visually, and it effortlessly complies.

Generative interfaces also allow context-awareness, and for the computer's modality of interaction to change according to the user's circumstances. In the demo, Stephen interacts by voice and sees visual feedback on a large screen — but the interface could morph entirely depending on his situation. At the screen, he might get keyboard and mouse affordances. Walking around, voice and large visuals. Not facing the display, audio-first. Left the room entirely, it follows him to another device. We didn't delve deeply into this context-awareness in the demo, but it's a capability that interface flexibility makes possible. You don't write a desktop app and a mobile app — you give the computer primitives and instructions for how to present itself in different scenarios. (More on context-awareness in a future post.)

We're betting on generative UIs not because they're possible and cool, but because they remove a massive constraint.

## Structure amidst flexibility

The greatest risk for any UI that changes is disorienting the user — as Jef Raskin observed, unpredictability is the enemy of usability. While in theory the computer could fully synthesize a graphical display for every command, such an interaction would be chaotic and disorienting.

One solution is to package up these UIs as something like "apps" and try and keep the same metaphors we have today. A generative UI just means being able to generate new apps. This is a skeuomorphism, and one that (while familiar) substantially hinders the benefits of a generative interface.

Instead, we solve this by giving the interface a logical scaffolding, with just enough structure and convention to make the interface understandable, while preserving enough degrees of freedom to flexibly serve any user need.

The Telepath Computer relies on the concept of cards in a three-dimensional space with well-defined laws of physics. Cards can contain completely synthesized UI (such as a graph), or they can represent a particular object (such as an article, email, or note). They adapt their surface to display only what is needed for the task at hand — showing a summary of an email rather than the full thread, for example — to reduce cognitive overhead.

This structure enables what I've been calling the "show and tell" metaphor. In the show-and-tell interface, we're mimicking how humans tackle complex work collaboratively in real life: an ephemeral discussion about the work at hand, while assembling the artifacts, documents, and clippings we need to reference on a shared surface. The computer responds through voice while simultaneously displaying objects — both to support its points and to give the user something to interact with, dive deeper into, save for later, or act upon.

This is a departure from chat, where conversational responses and actual content intermingle in one long thread. Here, we split them out. Conversation is ephemeral, just like it would be in the real world. But we can make anything permanent by placing it onto the canvas, where the user can interact with it, file it, grab it — treating it like a first-class object rather than just a chat response.

## Sensemaking

At the outset of the demo, Stephen asks the computer: "I have five minutes, what's up?"

To answer this question effectively, the computer needs a deep understanding of the user and their information landscape. This is what we've been calling *sensemaking*: the ability to make sense of the user's digital world, construct a model of them — their interests, beliefs, projects, relationships — and assess all new information and all generated interfaces against that model.

Essentially, an agent is in charge of the display. Just as you need high-alignment to execute tasks, you need high-alignment to create UI. The bigger the job the more you need.

Sensemaking plays hand-in-hand with a generative UI. By definition, a generative UI is both creating things and leaving things out. If you're deciding what to show — and crucially, what to omit — you need a deep understanding of what the user cares about. Without it, you're shooting in the dark, and a generative UI becomes a hindrance rather than a help.

Sensemaking is a continuous process. The computer models you as a user and assesses new information coming in — emails, messages, user input, information from the web and feeds — to construct an understanding that informs all future interactions.

This capability has never existed on personal computers. Today, you're given a list of files or notes, and you have to make sense of it all yourself. We know sensemaking is a significant unlock because we've seen it play out elsewhere — in software development, for instance, where effective code generation depends heavily on upfront planning and understanding of a codebase. A sensemaking computer spreads this capability throughout the entire system, enabling a generative UI to be genuinely personal rather than uselessly generic.

## Background & acknowledgements

The Telepath Computer concept is intended not as an exact picture of what we are building over the next few months at Telepath, but rather an embodyment of the principles we're building with and exploration of what it looks like to follow them to their full effect.

We got to this stage through a process that combined equal parts evidence and imagination[^1]. We interviewed a series of computer users to identify general problems that presented themselves as fundamental to the computer, across many use cases. Then we zeroed in on specific knowledge synthesis & artifact creation workflows to investigate those further. We combined the synthesis of these interviews with our forecasts of where we saw capabilities emerging, especially around local models (which will run constantly on-device far more efficiently in the future), voice synthesis, and code generation. We brought along our own educated guesses of where the future is headed, read up on historical context, and watched a bunch of sci-fi and prior art, before sketching the first concepts and iterating from there.

On that note, it's important that I acknowledge some fantastic work that went into inspiring this concept. Foremost, the Apple Knowledge Navigator concept spearheaded by John Sculley, which while comically dated in some ways is a great example of the creative power a product demo can have. It predicted the web, voice assistants, and touch-screen tablets long before any of these existed.

Other notable mentions to:

- [Mercury OS](https://www.mercuryos.com/) by Jason Yuan, a speculative vision for a fluid, intent-driven operating system based around modular cards that influenced Telepath's card metaphor. 
- [Desktop Neo](https://desktopneo.com/) by Lennart Ziburski, which was a great example of how to take emerging capabilities (multi-touch, voice control) and apply them to real user benefit.
- The film *Her*, not for its depiction of AI (we don't really want to emulate that) but rather its humanistic, depth-based, textural screen design that encouraged us to play with depth.
- Matt Webb, whose thinking on conversational interfaces helped shape our "show and tell" metaphor

I hope this work encourages others in the industry to consider more deeply an optimistic vision of where they want this technology to go to, with more fidelity than just "AGI", and to share that broadly to the world so we can discuss and create that future together. In the meantime, if you'd like to follow along with Telepath's progress on making this a reality and get access to our Alpha program, you can do so [here](https://telepath.computer).

[^1]: With evidence alone, you can only iterate. With imagination alone, you are only guessing.

---

- Mention how gen-UI can't just look like apps


One solution is to package up generative software in app-like bundles, and try and keep the same metaphors we have today. In other words, a generative UI just means anyone can generate their own app. This skeuomorphic approach is tempting: we're already seeing a bunch of startups coalescing around it. However, this 


  Finally, generative software allows for software that can change modality depending on the situation at hand.
   In our demo, Stephen interacts by voice and sees visual feedback on a large screen — but the interface could
   morph entirely depending on his circumstances. At the screen, keyboard and mouse affordances might appear.
  Walking around, voice input with large visuals. Turned away from the display, audio-first. Left the room
  entirely, it follows him to another device.

  We didn't delve deeply into this context-awareness in the demo, but it's a capability that interface
  flexibility makes possible. You don't write a desktop app and a mobile app — you give the computer primitives
   and instructions for how to present itself in different scenarios.
