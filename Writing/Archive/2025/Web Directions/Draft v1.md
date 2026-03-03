// "Boolean logic + bits"

Ever since the dawn of computing, the fundamental unit of computation has been boolean logic operating on bits.

---

// Bit passing through logic gates

Here we have a simple circuit where a pulse of electricity is passing through an OR gate.

---

// Basic computation schematic

If we arrange a sufficient number of these gates in the right way, we create something that can do computation, like adding numbers.

---

// An early computer like ENIAC

When you scale that up to more & more complex circuits, you get a general purpose computer. This was one of the first ones, ENIAC.

---

// Programming the ENIAC with plugs

And here are some of the first computer programmers, telling ENIAC what to do. ENIAC was basically a complex set of the electronic circuits we saw before, arranged in functional units like adders, accumulators, and multipliers.

Because all of these things are just series of dumb logic gates, to get it to do something useful you had to literally plug outputs from one set of gates into the input of another, to make a huge equation or algorithm. These patch cables allowed "computers" to give the machine explicit instructions, without having to rebuild the whole machine.

---

// Punchcards

Over time we developed better ways to instruct computers what to do...

---

// Command line

Then even better ones.

But still, there was a fairly large learning curve to work out exactly how to write the specific code words and incantations that would create configurations of logic gates to do what you wanted. We're just finding nicer ways to rearrange logic gates after all.

---

// Desktop

So, we built operating systems, with much more user-friendly ways of instructing the computer.

Along with that, we created the concept of an "application". Because it was hard to program, people who knew what they were doing would program *for* users, by working out what large groups of users wanted on average and writing code to do those kinds of things. Applications got a little window on the screen that where they could display anything they wanted, and where the user could interact with them.

These applications could then expose a subset of easy controls for the user to handle, that the developers thought would be important. We neatly presented those options in drop-down menus, form fields, and buttons.

Now developers instructed 99% of the computer, both at the operating system and the application level, and all the user had to do was take that last 1% over the finish line to get the computer to do what they wanted.

---

// Error messages

At least, that's what happened most of the time...

---

// Modern operating system, with RAM piling up, apps opening, etc.

Now, we have the modern computer. It's sophisticated. There's a *lot* going on under the hood. It's landed a human on the moon, it ... it helped me write my talk and arrange the slides.

---

// Back to the bit

But underneath it all, is this. Everything is translated down to a 0-or-1 bit, and the logic gates that operate on it. The consequence is, that *someone* needs to tell the computer what to do, all the way down the stack – from the operating system vendor, to the application developer, and finally (in a limited way) the user. Because computers don't understand us users. They don't know what we want. They can't take independent action, they can't deal with the ambiguity of a human intent – they are deterministic, highly-specified machines that only know zero and one.

---

// Simple neural network

Then these things came along. This is a neural network. Like a logic gate, it has an input and an output, but its behavior is entirely different.

The interesting thing about machine learning is that it is a process that relies on *learned* associations and behavior instead of *pre-programmed* behavior. 

---

So, where an algorithm is deterministic, a neural network is probabilistic.

---

Where an algorithm can only react to discrete inputs, a neural network can parse & replicate patterns in images, sound, code, and of course natural language.

---

Most importantly, where an algorithm made of bits & logic gates must be instructed precisely in circuits and code, a neural network can be trained to react appropriately to human intent. You just need to show it enough examples.

This is a new, foundational technology shift in computing. But we haven't felt it quite yet.

---

There's that old quote from Henry Ford, where he said that if he'd asked people what they wanted, they would have said "faster horses". Well in fact, when the first internal combustion engines came along, we just plonked them on the end of horse carriages. We still had these big, open wooden carriages with huge metal-rimmed wheels. You would steer it with a yoke.

It would take a decade ==(citation needed)== for us to land on the design that today has evolved into the modern car. An engine strapped to a horse cart is roughly equivalent to a faster horse that can ride longer without getting tired. A motorcar is a revolution in personal transport, which also required the construction of motorways, gas stations, cultural norms, business infrastructure, legal structures, to reach its full potential. The actual expression of the fundamental technology took a while to come to exist.

---

// Screenshot of sidebars & chat apps

We're in a similar spot right now with neural networks.

We've responded to this amazing new material by peppering our existing personal computers with bits of machine intelligence. We're putting AI chatbots in apps, creating sidebars, and developing computer use agents to browse the web and use Amazon.

---

But just like that early motor horse cart, we're cobbling this tech on to structures invented for the prior era. The desktop metaphor, windows, buttons, software distribution, operating systems, and applications. All have been designed fundamentally to compensate for the fact that we need to program computers to get them to do what we want.

---

// Claude Code

That isn't true anymore.

---

// Neural network in a car

And I think that means that, just like the horse cart, soon we will begin unraveling that structure and rethinking the pieces that were built in a pre-machine intelligence world. And that's going to lead to a very different kind of computer.

--- 

Why do I care?

---

// Me at home with the computers

Well, I grew up in a household surrounded by computers. As an introverted kid, computers were tools for creativity – I could build worlds inside them, with multimedia, text, and code, and make anything a reality. After spending some time exploring what I wanted to do with my life, I came back to that feeling of empowerment, and started making creative tools using some of the early large neural networks that were starting to emerge in the late teens.

But what was empowering to me was confounding to most other people in my life. People I loved and cared about, who were incredibly capable in the physical world, were having to struggle with a digital world they didn't understand, one that felt foreign and unnatural. They just didn't know how to talk 'computer'.

As the amount of our lives we've delegated to the digital world has increased, so has the inability of a series of dumb logic gates to be sufficient for managing it. We're at the receiving end of a firehose of information, and at the end of it all is one human mind trying to manipulate emails, files, folders, screenshots, and a million digital portals and shopping carts.

If a computer is meant to be a bicycle for the mind, it feels like the tires are flat.

---

At Telepath, we're focused on creating a new kind of computing experience, built for an era of machine intelligence. Let me show you a demo of what we think that looks like:

---

[DEMO]

---

==Make a case for the dumb user value here first==

---

// Generative user interface

The first thing you'll notice is that the user interface here is flexible, morphing to fit the task at hand. There's no conception of "apps", instead the machine synthesizes or composes functionality and views according to the user's intent.

---

// Sense-making

And the computer isn't just presenting a big list of files, or notes, or whatever, and leaving the user to browse for themselves. Instead, it is *actively making sense* of all of the information at hand. When the user says they have a few minutes, what's up, the computer knows .

---

// Deep personalization

This implies a level of deep personalization, which is another trait of this future machine. You can't make sense of information unless you know who you're making it make sense for. Telepath is able to form a precise model of the user, their beliefs, values, projects, relationships, etc., and deploy that to any task. That's the only way that a computer can effectively filter all the information it could present.

---

// Proactivity

Because the user doesn't need to give the computer every explicit instruction, and because the computer has a deep model of the user,  it means that the computer can take action on a user's behalf. When we approach or leave the machine, it's continuing to do stuff for us.

---

// Metaverse

Most predictions of the future are wrong in important ways. Or sometimes they're right, but just well ahead of their time... let's hope not with this one.

So will this pan out?

---

// Platform shift happens

First off, we shouldn't have normalcy bias here. Our dominant platforms shift and new ones emerge – from CLI to GUI in the 1980s, 15 years later to the web, 15 years after that to mobile, each of these a percolation of a fundamental technology emerging. It's rational to believe that 20 years later, with a new fundamental technology on our hands that's opening up brand new computing capabilities, we would be on the verge of another one.

Each of these prior shifts has changed our interaction patterns, software distribution, and form factors.

---\


// The technology is here, and getting better

We already have the core technologies we need to build the computer I demoed. Models are getting more reliable, smaller, local, and the hardware is catching up.

---

// We're already building it

Telepath is explicitly focused on building this vision into a reality. This is the computer we want. We think these properties are emergent from the nature of neural networks. And we think they offer a huge benefit to users.

Humanity has been dreaming up these computers for years.

There are almost definitely other folks out there who want to make something like it too.

---

Ok, so we've taken a journey through the history of computing, I've shown you a radically new kind of computer, and given you a (hopefully) convincing justification why I'm devoting a significant chunk of my life to bring it into existence.

Maybe you don't fully agree, but let's all squint and take it that this is coming. You should be asking yourself one question.

---

// WTF

I mean, we're in a conference focused on web development. For web developers. But in this new world, what *is* web development? What even is the *web*?

---

// Software distribution

The web today is a way to distribute & consume software. Even relatively straightforward websites today are essentially monolithic applications that download & execute client-side.

---

// Telepath's UI

This computer is very different. It is generating and composing interfaces & functionality together based on the user's intent and the task at hand. 

---

// Puzzle pieces

For most things, functionality & views become more like composable pieces. Instead of downloading Uber and Spotify and your banking app and your airline app, all of that capability exists as discoverable, interoperable services that your system can compose together.

We no longer need to bake all these pieces in together when we're building software, we can allow the user's system to do it on the fly, which gives them far more agency and flexibility. I think that takes us away from thinking about building big CRUD react apps, and more the lego pieces, and maybe some happy paths, for what the user might be trying to achieve. 

---

// Information distribution

Hidden inside these apps we're constantly shipping around to people's browsers is really the core use case of the web – distributing information. Ever since TBL hooked up his NeXT to the network at CERN this has been the killer app.

---

// Retrieval of information in Telepath's UI

A system like this is constantly querying for information, and because it's happening behind the scenes, it's important that this information is high quality and can be trusted. Implicit in this demo is a network of information, not applications, that is being constantly queried as a ground truth.

--- 

// The current web

Which ... is not the state of the current web. An attention economy driven by ads, initially the lifeblood of a healthy web economy, has driven the web towards clickbait and low-quality content aimed at either selling you ads or roping you in to sell you products. Not only is this incentive structure at odds with actual good information, it also is unviable if you no longer are able to force the computer to display ads to the user.

---

// New economics

Which means that we're going to see a new economics emerge on the web. My guess is it looks something like direct micropayments authorized by the agent on your behalf, but I don't know for sure.

---

// Information architecture & new ways of consuming

And here's what might be uncomfortable: you lose control over presentation.

Users aren't coming to your website anymore. Their AI agent queries your information and presents it however makes sense - possibly mixed with competitors, possibly in a format you never designed for. There's a new kind of responsive design here.

All you control is the information itself. Your craft shifts from pixel-perfect interfaces to information quality. The only things that matter: good information, well-structured, discoverable, trustworthy.

---

// What is a developer?

Our job as developers has never really been to write lots of software, or master React Hooks. These are all means to an end. We're here to help users through software. And that's still true.

The technical skills that remain valuable are at the extremes. Lower-level systems work, building the AI platforms, the infrastructure, or sophisticated professional software that needs precision. Or, the human-centered work: information architecture, designing and crafting the critical paths, deep understanding of the user and business problems, taste and artistry. These will be critical.

// "Small pieces loosely joined"

But there's another critical role for everyone in this room: that's to keep the principles of the web alive.

Now everything we've discussed up here, must sound like a significant departure from the web we know today. But I think it's a return to what made the web special in the first place.

Instead of large, monolithic, monopolistic applications that centralize control, we may be at the start of a journey towards small, composable, interoperable, discoverable capabilities that our *user agents* can compose together through open protocols.

But we also risk this new technological shift turning into a mega-app, the AOL of our time.

The web isn't really about HTML, CSS, and JavaScript. It's about an open, linked, permissionless, transparent, collaborative, accessible networked platform that anyone can consume, and publish to, without having to ask *anyone* for permission. Let's keep that fire burning.

The web is dead, long live the web.