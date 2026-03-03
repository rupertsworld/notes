# What does an intelligent personal computer look like?

// You're either developing an app, or iterating on chat, and don't have a clear sense of the future. You need to know both these things are going away.

What happens if you take the idea that AI is going to revolutionize computing seriously?

On the one hand, you could argue we're doing this already: as an industry we're pouring untold billions of dollars into frontier models, and putting a chat sidebar in everything. On the other hand, most companies are iterating on the default form factor of chat, and the continued existence of apps, all while waving their hands broadly at the idea of "AGI" and how everything is going to change.

But what does an AI-native computer actually *look* like? *Feel* like? How can we anticipate and build for this future if we don't have a clear picture of it?

What we need is a good demo.

// You should believe me because I've worked at some great places & done big things. Also, this is why a demo is important.

I've seen the power of collective imagination that a well-executed demo unlocks. At Google Creative Lab, demos I gave turned into experiences we shipped to millions of users. At Adept, a demo our 3-person design team gave one Friday afternoon led to a tectonic shift in company direction by Monday morning.

So a few months ago, we at [Telepath](https://telepath.computer) set out to create a compelling demo of what an AI-first personal computer will actually look like. (We're trying to build one, after all!) My co-founder Stephen Hood presented it at Betaworks this past November.

[VIDEO](https://www.youtube.com/watch?v=jEm5SkLMap0)

So let's break this demo down a bit, and why we came to some of these design decisions.

// The generative UI

The most striking thing about this computer is that there are no apps. Instead, the interface is **generative**: meaning it is either synthesized or composed on the fly according to the user's intent.

Of course, those following along at home will know that generative UI is the hot new thing in the AI world. But beyond knowing we *can* now make a generative UI, let's explore *why* we think that's important, and why it will replace the concept of apps.

The app model of computing is something we are well accustomed to at this stage, and has come out primarily out of necessity due to the fact that computers are unable to actually understand our goals and preferences, or adapt themselves, and instead need to be programmed ahead of time to accept discrete, computable inputs for a generic group of users.

Machine learning models remove this constraint, with tanigble benefits for users. It removes a significant obstacle between intent ("I want to do this thing") and outcome, namely choosing and installing an app, learning how to use it, and dealing with its constraints. Have you ever had an app but wished it worked differently? Been confounded abut how to achieve something with the apps you have? Or lamented a seemingly non-sensical change in an product you love? These are all problems inherent in the app model.

It also means that the space of possible actions you can take, and the possible ways information can be displayed, is infinite. Just as you can ask an LLM to create text of any format (or code, or CSV files, or whatever), a generative UI can create an interface of any form. It takes this text-based flexibility of LLMs and scales it to the entire computer (handy, because everything is code).

So we are betting on generative UIs, not because they are possible and cool, but rather because they remove a huge constraint. For example, Stephen is able to ask the computer to map out public opinion on an issue visually, and it effortlessly complies.

It's not all good — the greatest risk for any UI that changes is disorienting the user  [Raskin]. While in theory the computer could fully synthesize a graphical display for every user command, such an interaction would be chaotic and unpredictable.  We can solve this by giving the system just enough structure and convention to make the interface understandable, but enough degrees of freedom so that it can flexibly serve any user need.

To do this, we relied on the concept of cards in a three-dimensional space with well-defined laws of physics. Cards can contain completely synthesized UI (such as a graph), or they can represent a particular object (such as an article, email, or note). They adapt their surface to display only what is needed for the task at hand (for example, a summary of an email), to eliminate cognitive overhead.

We expect our thinking on this to evolve over time.

The interface relies on a show-and-tell metaphor, as opposed to a chat-based metaphor. I came across this while discussing conversational interfaces with Matt Webb. When you're doing anything serious in a conversation, you might 

The interface also utilizes something that I've been calling the "show and tell metaphor" or the "tabletop metaphor," which is an idea that I came across while discussing conversational interfaces with Matt Webb.

In the show and tell interface, we're mimicking where humans might tackle complex work collaboratively in real life, which is to both have an ephemeral discussion about the work at hand (in this case collecting research) while also assembling the artifacts/documents/clippings etc. that we need to reference which are more permanent.

So you see the computer here. Both responding through voice while also displaying objects to the user to support its points or allow a focal point for the user to interact with or dive deeper into (save for later or read or do other things with).

Instead of pending context to a big long thread, intermingling conversational responses with actual content, we're splitting those things out. Where conversation is intended to be ephemeral just like it would be in the real world but we can make anything permanent by putting it onto this 3D canvas from which the user can interact with it, file it, grab it and it can be treated like a first-class object instead of just a chat response 

// Sensemaking

The core capability of this computer is something we've been calling sense-making. And that is the ability to make sense of the user's digital landscape, deeply personalize the system, and to make a model of the user: their interests, their beliefs, their projects, and assess all new information and all interfaces that it's going to generate based on that mental model.

This is really important and it plays well with the idea of a generative UI because by definition a generative UI is both creating things and leaving things out. If you're going to display something to the user and invent what is on that display and what sort of things you should display and what importantly should leave out, you're going to need a very deep understanding of what the user's desires are, what their preferences are, what they might find important in order to construct that view effectively.

Without that you're really kind of shooting in the dark and they're not going to build an effective generative UI. So we knew sense-making was important from the outset of this computer. It's a capability that has never existed on computers. Typically you are just given a big list of files or notes or stuff and you have to poke around and make sense of all this information yourself.

And it's a huge unlock. We know that because we've seen it play out in other areas like software development with code generation tools. A big part of that is the upfront planning and making sense of a codebase.

We've seen it play out in chat tools but in a much more limited way. So the sense-making computer really spreads this capability throughout the system and enables the apart from enabling the features that this allows, also really unlocks the capability of a generative UI to be personal and not just useless in generic. 

A surprising outcome from our exploration into what a full generative UI might look like in practice is the importance of what we're calling *sensemaking*. Unlike a list of files on your computer, or your to-do list app, a generative UI by definition doesn't just show you all the information in your system. It reasons about you as a user, filters information, and constructs a representation of it, in order to best respond to your query.

At the outset of the demo, Stephen asks the computer "I have five minutes, what's up?". In order to effectively answer this question, the computer needs to have a deep understanding of the user and their information landscape, otherwise a generative UI could be a hinderance.

Sensemaking is a process by which the computer continuously models you as a user — your interests, projects, people in your life, etc. — and assesses new information comming in (emails, messages, user input, information coming via the web and feeds). It uses this information to construct a model of the user which will inform future interactions.

// Context-awareness

Side effect of having a generative interface is that it can adapt to the user's current situation. This context awareness is another key part of the telepath computer but one which didn't really get a look in in the video.

Context awareness means that the system can change its interface and modality according to the user's needs at the time. So for example, while this starts off as a desktop-like experience on a large screen primarily with a voice as Steven is walking around, one might imagine that if he went and approached the computer and sat down he would be given more affordances to interact with it with a mouse and keyboard.

If we walked away the display might grow larger and voice might be the primary method of feedback instead of something visual on the screen. And perhaps if you walked out of the room the interface would transition to audio through a mobile device or earbud.

When your user interface is generative it can be completely adaptive and that unlocks the whole new capability of a computer that is fully and very naturally integrated into your life and your physical environment. A great reference point for this is the computer in Star Trek which both displays a graphical interface but also can be interacted with through voice and often both at the same time for different purposes 

// Acknowledgements



// Methodology

---

Our first principle was that the Ui should be dynamic\
Here's what it's like now, and why this is now no longer necessary\
Here's why this is a huge user benefit
And here's hwo it shows up in the demo


Let's start by talking about the **dynamic interface**, and by extension the lack of apps.


https://x.com/rupertmanfredi/status/1653780093712633859



In a personal computer today, the first thing we'd do is to consider what app to unstructured


Instead of dealing with individual applications, browser tabs, and a mess of files, he is nagivating fluidly through a dynamic user interface that makes sense of his information landscape and adapts to his instructions on the fly.



You'll notice that in our demo there are no apps. Our first big insight in researching for this demo is that in a world where software can be synthesized on the fly, it's possible to do away with the traditional application model of shipping and consuming pre-defined software.


At the core to this is a central **dynamic interface**, one that is...  and by extension its distinct lack of apps (at least in the traditional sense).

---

In the video, we see a knowledge worker following a thread of research, eventually landing upon a compelling premise for a piece of writing. This sort of insight -> artifact workflow is prevalent across many kinds of knowledge work, whether it's writing an article, drafting an internal memo, or creating a presentation. However, 


(a workflow central to the knowledge workers we interviewed, and a use case inspired by our biggest inspiration for the project, Apple's Knowledge Navigator). However, the way he's going about this task is a significant departure from a typical computer today.


At Telepath, our mission is to bring about this new era of personal computing. So a few months ago, we at Telepath set out to create a compelling demo of what an AI-first personal computer will actually look like. My co-founder Stephen Hood presented it at Betaworks this past November:

So a few months ago, we at Telepath set out to answer that question concretely. We built a demo of what an AI-first personal computer will actually look like. My co-founder Stephen Hood presented it at Betaworks this past November:

 Demos turn vague ideas into concrete ones, and are an awesome catalyst for progress.

I'd argue that currently, we're not doing that well as an industry. We're instead iterating on the chat interface from ChatGPT, putting chat into sidebars so users can talk to their apps. At Telepath, we've spent some time thinking about this, and we believe the future looks far different, to the point where most companies won't be shipping apps at all.

It doesn't look like apps with chat sidebars.


When I look around at the AI industry, there's no lack of cool products and demos emerging. However, there's something missing: design work that explores what a computer should fundamentally become. We're continuing to iterate on chat, but the north star for computing itself seems vague beyond "AGI".

// You should believe me because I've worked at some great places & done big things. Also, this is why we made a demo.

I've seen the power of the collective imagination that a good demo unlocks, and it's an awesome catalyst for invention and progress. At Google Creative Lab, demos would spin off into public-facing projects we shipped to millions of users. At Adept, I remember a time our design team catalyzed a tectonic shift in company direction with a one-minute demo at our all-hands on a Friday afternoon.

// Here's what we did and what I'm going to show you

So, a few months ago, we at [Telepath](https://telepath.computer) set out to demonstrate what an AI-first personal computer should look like. My co-founder Stephen performed it live at Betaworks Demo Day in November, here's the video


So, when we prepared to present the thesis of our company to a high-profile audience at Betaworks' Demo Day in November, we felt like we'd better have a pretty good idea of what it looks like. To communicate this vision, we settled on one of the most effective tools for imagining the future and bringing it into existence – the demo.



The promise of AI is to produce a transformative technology that reshapes computing. But since ChatGPT, we've been spending our time iterating on chat, while gesturing vaguely at AGI. In order to sensibly anticipate the future, we need to envision what that future entails when we take our current and expected capabilities to their logical conclusion. We did this, and discovered there's going to be significant disruption.


there is a distinct lack of *visionary* demos. That is, something that peers a little further into the future paints a picture of what computing will look like


  If you're building AI products right now, you're likely doing one of two things: adding AI capabilities to existing apps, or iterating on chat interfaces. Both approaches assume the current paradigms of computing will persist. They won't. Apps are ending. Chat as the primary interface is a local maximum. And yet, when I look around the industry, I don't see design work exploring what comes next—just more products built on these dying foundations.
