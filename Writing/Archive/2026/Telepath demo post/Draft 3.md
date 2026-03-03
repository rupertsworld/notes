# What does an intelligent personal computer look like?

What happens if you take the idea that AI is going to revolutionize computing seriously?

On the one hand, you could argue we're already doing this: as an industry we're pouring untold billions of dollars into frontier models, and putting a chat sidebar in everything. On the other hand, most companies are iterating on the default form factor of chat and the continued existence of apps, all while waving their hands broadly at "AGI" and how everything is going to change.

But what does an AI-native computer actually *look* like? *Feel* like? How can we anticipate and build for this future if we don't have a clear picture of it?

What we need is a good demo.

I've seen the power of collective imagination that a well-executed demo unlocks. At Google Creative Lab, demos I gave turned into experiences we shipped to millions of users. At Adept, a demo our 3-person design team gave one Friday afternoon led to a tectonic shift in company direction by Monday morning. Demos turn vague ideas into concrete ones, and are an awesome catalyst for progress.

So a few months ago, we at [Telepath](https://telepath.computer) set out to create a compelling demo of what an AI-first personal computer will actually look like. (We're trying to build one, after all.) My co-founder Stephen Hood presented it at Betaworks Demo Day this past November.

[VIDEO](https://www.youtube.com/watch?v=jEm5SkLMap0)

In the video, we see a knowledge worker following a thread of research, eventually landing upon a compelling premise for a piece of writing. This insight-to-artifact workflow is central to many kinds of knowledge work, whether it's writing an article, drafting an internal memo, or creating a presentation. But the way he's going about this task is a significant departure from a typical computer today. Instead of dealing with individual applications, browser tabs, and a mess of files, he navigates fluidly through a dynamic interface that makes sense of his information landscape and adapts to his instructions on the fly.

Let's break this demo down, and explore why we came to some of these design decisions.

## The generative interface

The most striking thing about this computer is that there are no apps. Instead, the interface is **generative**: synthesized or composed on the fly according to the user's intent.

Those following along at home will know that generative UI is the hot new thing in the AI world. But beyond knowing we *can* now make a generative UI, let's explore *why* we think it's important — and why it will replace the concept of apps.

The app model of computing is something we're well accustomed to at this point. It emerged primarily out of necessity: computers are unable to understand our goals and preferences, or adapt themselves, so they need to be programmed ahead of time to accept discrete, computable inputs for a generic group of users.

Machine learning models remove this constraint, with tangible benefits for users. A generative interface removes a significant obstacle between intent ("I want to do this thing") and outcome — namely choosing and installing an app, learning how to use it, and dealing with its constraints. Have you ever used an app but wished it worked differently? Been confounded about how to achieve something with the apps you have? Or lamented a seemingly nonsensical change in a product you love? These are all problems inherent in the app model.

A generative interface also means that the space of possible actions you can take, and the possible ways information can be displayed, is infinite. Just as you can ask an LLM to create text in any format (or code, or CSV files, or whatever), a generative UI can create an interface of any form. It takes the text-based flexibility of LLMs and scales it to the entire computer. In the demo, Stephen asks the computer to map out public opinion on an issue visually, and it effortlessly complies.

So we are betting on generative UIs not because they are possible and cool, but because they remove a huge constraint.

### Structure amidst flexibility

It's not all upside — the greatest risk for any UI that changes is disorienting the user [Raskin]. While in theory the computer could fully synthesize a graphical display for every command, such an interaction would be chaotic and unpredictable. We solve this by giving the system just enough structure and convention to make the interface understandable, while preserving enough degrees of freedom to flexibly serve any user need.

To do this, we rely on the concept of cards in a three-dimensional space with well-defined laws of physics. Cards can contain completely synthesized UI (such as a graph), or they can represent a particular object (such as an article, email, or note). They adapt their surface to display only what is needed for the task at hand — for example, showing a summary of an email rather than the full thread — to eliminate cognitive overhead.

This structure also enables what I've been calling the "show and tell" or "tabletop" metaphor, as opposed to a chat-based metaphor — an idea I came across while discussing conversational interfaces with Matt Webb.

In the show-and-tell interface, we're mimicking how humans tackle complex work collaboratively in real life: an ephemeral discussion about the work at hand, while assembling the artifacts, documents, and clippings we need to reference on a shared surface. The computer responds through voice while simultaneously displaying objects — both to support its points and to give the user something to interact with, dive deeper into, save for later, or act upon.

This is a departure from chat, where conversational responses and actual content intermingle in one long thread. Here, we split them out. Conversation is ephemeral, just like it would be in the real world. But we can make anything permanent by placing it onto the 3D canvas, where the user can interact with it, file it, grab it — treating it like a first-class object rather than just a chat response.

We expect our thinking on this to evolve over time.

## Sensemaking

The core capability of this computer is something we've been calling *sensemaking*: the ability to make sense of the user's digital landscape, deeply personalize the system, and construct a model of the user — their interests, beliefs, projects — assessing all new information and all interfaces it generates against that model.

This plays hand-in-hand with a generative UI, because by definition a generative UI is both creating things and leaving things out. If you're going to display something to the user and decide what to show — and crucially, what to omit — you need a deep understanding of the user's desires and preferences in order to construct that view effectively. Without it, you're shooting in the dark.

At the outset of the demo, Stephen asks the computer "I have five minutes, what's up?". To effectively answer this question, the computer needs a deep understanding of the user and their information landscape. Otherwise, a generative UI could be a hindrance rather than a help.

Sensemaking is a process by which the computer continuously models you as a user — your interests, projects, people in your life — and assesses new information coming in (emails, messages, user input, information from the web and feeds). It uses this to construct a model that informs all future interactions.

This capability has never existed on personal computers. Typically you're just given a big list of files or notes, and you have to poke around and make sense of all this information yourself. We know sensemaking is a huge unlock because we've seen it play out in other areas — like software development, where a big part of effective code generation is the upfront planning and understanding of a codebase. A sensemaking computer spreads this capability throughout the entire system, enabling a generative UI to be personal rather than generic.

## Context-awareness

A side effect of having a generative interface is that it can adapt to the user's current situation. This context-awareness is another key part of the Telepath computer.

Context-awareness means the system can change its interface and modality according to the user's needs at the time. While the demo starts as a desktop-like experience on a large screen with voice as the primary input — Stephen is walking around — one might imagine that if he approached the computer and sat down, he would be given more affordances to interact with mouse and keyboard.

If he walked away, the display might grow larger and voice might become the primary method of feedback instead of something visual on the screen. If he left the room entirely, the interface might transition to audio through a mobile device or earbud.

When your user interface is generative, it can be completely adaptive — and that unlocks a computer that is fully and naturally integrated into your life and physical environment. A great reference point for this is the computer in Star Trek, which displays a graphical interface but can also be interacted with through voice, often both at the same time for different purposes.

## Acknowledgements

*[To be written]*

## Methodology

*[To be written]*
