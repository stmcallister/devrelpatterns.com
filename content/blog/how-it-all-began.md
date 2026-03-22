---
title: "How It All Began"
date: 2026-03-21
draft: false
tags: ["history", "general", "trivia"]
author: "Ted Neward"
description: "Being a short history of how the book came to be."
---

With the publication of the book in February 2026, we finally brought to a close a process that had been going on for over two years, across two continents (bear with me), countless discussions, and needless to say a ton of hard work.

It's not common in the technical space, but readers sometimes want to know the "story behind the book"---questions like, "Why did you choose this topic? What was your motivation for writing it? How did you get started on the project? Did you have any other projects that were competing with this one? Why did you decide to write a book about this?" So, in the interests of those who are curious, I figured it'd be a good way to kick off a blog on the book by writing a blog about the book.

Once upon a time....

# 2019 - 2020
... a pandemic hit the world. We all locked down. Most of us remember that with some degree of distaste and frustration, so I won't linger on that memory except to say, "It was a time in which side projects suddenly got accelerated to the forefront of the brain", at least for me. For years, I'd been limping along with some scattered domains, and I wanted to take the time to look to coalesce everything into something coherent. Magical. Wonderful. Galaxy-shattering!

Yeah....

What ended up out of that, though, was a Git-backed, content-centric, statically-generated site so that I could just `git commit; git push` new updates and have things just "happen". The first property was [my research garden](https://research.tedneward.com), and once I had that more or less tuned to where I wanted it, I built out the [professional site](https://www.newardassociates.com) and [blog](https://blogs.newardassociates.com). Of course, along with the blog, came the deep-seeded feeling that "I need to go back and find topics to write about". Which meant going back through notes and notebooks of quite a few years. (Of which I have many.)

Buried in those notes was some notes around "developer relations" and a bunch more around "patterns", but nothing that combined the two. Yet. Things took a slight turn as we started to come out of lockdown, though....

# 2021
... in that I was laid off.

Although I didn't know it at the time, it would be [a three-year hiatus away from work](https://blogs.newardassociates.com/blog/2025/involuntary-sabbatical-reflections.html), but at the time, I saw it as a sort of "accidental sabbatical" (which I later came to term an "involuntary sabbatical") and an opportunity to dig into some side projects more deeply. Some of that was coding stuff, some was doing more research around various tech topics, but a lot of it was writing, often as a way for me to express what was jumbling around inside my own head. (Attention Deficit can be a hindrance, but man, if you ever want to feel like you're in the epicenter of a maelstrom of chaotic inspiration, an ADD brain is a wonderful place to be.)

DevRel has never been too far from my thoughts. I had spent a bunch of time at Rocket Mortgage talking with Woody about how we bring a degree of rigor and professionalism to Developer Relations as a profession in the years before. Even before that, when Scott and I worked at Smartsheet, I was looking for ways to better track and codify the things we do in DevRel. I wanted to think about each thing we do, the value it brings (measurable or not), how we execute it well, and so on. A few interviews at companies interested in building a DevRel team fell apart, but it got me thinking about how I would categorize and organize the activities of the team if and when I were to take that role again. When do we think about doing an **Article** as opposed to a **Blog Post**? How does a **Blog Post** differ from a **Guide** or a **Reference Doc**? And that's just the written stuff, there's a whole host of other kinds of activities we can do; how do we choose between them?

It struck me, as I was sitting in my office one sunny afternoon, that what I was trying to do inside my head was create an ontology--a pattern language, for those who followed that movement--of the various things we do in DevRel, and the idea was born. But it would take a while to come together...

# 2022 
... because the more I started doodling on the idea, the more I realized that this was not a small effort.

I'd undertaken some effort around patterns before, in that I had decided to take a stab at [revisiting the Gang-of-Four software patterns](https://blogs.newardassociates.com/patterns/) with an eye towards modernizing and updating with some common software design patterns that had emerged in the years since the GoF book's publication. So I had a sense of what I wanted, but man, the more I dove into the topic, the more I realized that this was not a tiny little side project. I started collecting thoughts and a rough structure on what I wanted each pattern to look like in a branch on the blog site, and then by about the middle of the year realized that this was not going to be just a few blog posts--this was going to need more room than a blog post. A LOT more room. 

Begin with the pattern structure: The GoF model was a good starting point, but I had long since (in my own head) slimmed a pattern down to "A Solution to a Problem within a certain Context that yields certain Consequences", and that was my starting point early on. However, it was clear that certain patterns were more closely grouped to others, and there were a few other vectors--time, money, that sort of thing--that weren't really captured in my simple four-part structure. Still, being the stubborn sort that I am, I stuck to it, with the exception of what I termed the "Building Blocks": what was necessary to make the execution of the pattern succeed, categorized into the ontology of "Code", "Presentation", "Social", and "Writing". (Readers of the book will notice the obvioous missing element here, "Budget".)

The beauty of doing all of this in Git and Markdown was that I could just tinker, edit, cut-and-paste, and so on, until I had something that felt half-formed. That meant it was time that....

# 2023
... I published the [first draft of the pattern language](https://blogs.newardassociates.com/devrel/activities/catalog.html) on my website in February.

> **NOTE:** Readers of the book will note that, as Martin Fowler has done with his books and Bliki, a fair amount of the book material remains on the website. I haven't changed any of it since we started the book project, though, so the material on the website serves as a historical marker for those who are interested in seeing the deltas, as well as a cost-effective way for people who can't or won't afford the cost of the book to still get access to some of the material.

After pushing the bits to the Web, my thought was, "Whoof. Job done. Glad *that's* over."

Things stagnated for a bit on that front, but a conversation with Woody led me to think that maybe there was a book to be had here. I knew I didn't want to do the book alone--[I've published a few in the past](https://www.newardassociates.com/books/), and I did not want to solo this one, because it was still going to be a ton of work to do, despite what I had already done. [Patterns](https://plopcon.org/) need to be [workshopped](https://www.industriallogic.com/design-patterns-workshop/) if you're going to get any decent kind of result, and you can't workshop them by yourself. You need a critical mass of people to do it effectively, and sitting by myself in my office, I didn't have that.

Ever had one of those moments when somebody says something, and it just makes you go "Hm. Hmmmm. *Hmmmmmmm.* **HMMMMMMMMMM**"?

Woody said, "Well, I'll do it with you, if you'll have me."

You know? That's not a half-bad idea.

But even two was a little on the light side, so Woody and I started brainstorming about who else we would want to join us on this little endeavor. I wanted at least one more core author, and the publisher (APress, whom we spoke to while Woody and I were at DevSum in Stockholm in May) was really interested in having some kind of illustrations. Woody suggested David, who is famous within the DevRel community for his illustrations (and the fact that he could workshop the patterns with us, being more than just an illustrator, was a huge benefit), and I wanted to get a hold of Scott, who was there with me at Smartsheet when we were first thinking around these ideas.

> **TIP:** As another side-note, if you're thinking of writing a book, write about a quarter or half of it up front, *then* go find a publisher. Technical book publishers get literally hundreds of proposals from would-be authors who are absolutely sure that writing a book "can't be all that hard", and never end up with an actual manuscript for the effort. When you go to a publisher with a book that already has a significant chunk of the material written, it signals that you already understand the work involved, and gives you, the author, a lot more egotiating power than you do when you have just an idea. Remember, ideas are easy, it's the execution that's the hard part.

I knew already that I wanted APress to be the publisher, since they'd already "broken ground" in the DevRel community with Mary's book. I had a few fallback plans, but the APress folks were just as excited to get in on this as we were, so after an hours' or so conversation with James Robinson-Pryor at APress, we had a tentative contract in hand and just needed to fill out whose names would go in the "author" field on it.

On 17 July 2023, I wrote this email to Woody and Scott:

```
Scott, Woody; Woody, Scott. (I can't remember if you guys have met formally 
before or not.)

We should set up a time for us to connect and talk book stuff, and maybe 
think about making it a weekly touchpoint or something.

Scott, just sent you an invite to the repo. Woody, do you have David Neal's 
email or his GitHub handle? I'll add him as well as soon as I know it. (We 
should see if David can join some of the touchpoints as well.)
```

... and the project was officially off and running.

# 2026
Notice that I'm neatly bypassing two years' worth of touchpoints, GitHub commits (we did all our work in Markdown files in a private GitHub repo), and numerous email, SMS, and PR messages, but the blog post is titled, "How It All Began", and that's how the project started.

And, of course, you know how it ended: Eventually. But the rest of the story, I'll leave to the others to give their impressions and history. For now, the important thing, to me anyway, is that the seven-year journey that was this idea of "applying patterns rigor to the world of DevRel" is now officially out in the world's hands. It's been an awesome ride, and I hope that you, dear reader, will enjoy the reading as much as I (we) did the writing.
