---
layout: post
title: 'Stoic Development Part 1'
tags: [stoic development, blog]
featured_image_thumbnail:
featured_image: 
featured: false
hidden: false
---

![](/images/posts/stoic_development_zeno.jpg)

What is Stoic Development? Stoic Development is the convergence of the philosophy of Stoicism and software development. I've written this post as I think it will make you a better developer if you practice it.

Before we get into what Stoic Development is, it's important to understand Stoicism.

Stoicism is a philosophy that was founded by Zeno and originated in Greece.
The main pillars of Stoicism include:
  - Seek the deep understanding of things.
  - Have self-control, resist distractions.
  - Be comfortable being poor.
  - Practice negative visualization.

For more info about Stoicism [read](https://dailystoic.com/what-is-stoicism-a-definition-3-stoic-exercises-to-get-you-started/).

**1.**
**Seek the deep understanding of things.** Don't just agree with what you read, be a consumer that critiques and also understands the pros and cons.
For example, when you learn a new principle in programming, always make sure to understand the positive and negative tradeoffs. There's no such thing as a free lunch. Everytime you choose a library, framework, methodology, or architecture consider the negative side effect or potential tech debt.
For example, about a year ago we started using dependency injection in our test suites. Now, dependency injection is a great technique. That said it does have its drawbacks. Injecting a dependency can give you a false positive if you don't fully understand how to properly mock the dependency for the given test.

**2.**
**Have self-control, resist distractions.** Marcus Aurelius once said: "_Concentrate every minute like a Roman - like a man - on doing what's in front of you with precise and genuine seriousness, tenderly, willingly, with justice. And on freeing yourself from all other distractions. Yes, you can - if you do everything as if it were the last thing you were doing in your life, and stop being aimless, stop letting your emotions override what your mind tells you, stop being hypocritical, self-centered , irritable. You see how few things you have to do to live a satisfying and reverent life? If you can manage this, that's all even the gods can ask of you._"
As developers we all know there are so many potential distractions: slack notifications that do not stop beeping, your product manager who asks a question about something that he needs help with, your phone buzzing with notifications, or coworkers asking questions. These are just a few examples, of some of the things that interrupt us with on a daily basis. In the midst of this chaos we're expected to do our job. So how can we "_Concentrate every minute like a Roman_" ? Try practicing the following techniques:
  - Put your phone away. Only check it once an hour or less.
  - Invest in noise cancelling headphones.
  - Encourage your team not to have music or noise where programmers are working.
  - Commit to the hours you're going to work with no interruption ahead of your day. I try to accomplish at least 4 – 5 hours of uninterrupted work a day. Some of you might say that's not enough, but these are the hours that I consider deep work, with no interruptions.
  - Make sure to have some sort of physical activity in the middle of the day. I think this may be one of the best hacks I ever found. Anytime, I have a hard day, or I'm stuck on a problem, this always does the trick for me.

**3.**
**Be comfortable being poor.** Nowadays, almost every developer uses some sort of third party library/component. Don't get me wrong, I think that there are many advantages to this, but it has a price. My general belief, is that the more third party components you use, the more reliant you become on "_magic_". My suggestion is to practice once a week, a day without the use of any third party libraries. I know this sounds radical and could result in more lines of code, but it will also enable you to understand things on a deeper level (see the first point). It will remove your fear. For example, what happens if that library stops being supported? With a third party library this can happen any day of the week.

**4. Practice negative visualization.**
Seneca once said "_He robs present ills of their power who has perceived their coming beforehand ._" Which means, it's good to be a bit paranoid (just a bit). We, as software developers, are guaranteed one thing, and one thing only. At some point something will break. If we know that, we can prepare. Here are some examples that I follow to mitigate risk:
  - Write good tests (Unit and BDD). I can't tell you how many times this practice has highlighted a bug when I thought I was done with a specific feature.
  -  Be proactive about bug fixing. Don't wait for somebody to report it. If you see a bug, open a ticket. Fix it yourself. I can't tell you how awesome it is when somebody comes to me and says I found this bug, here's a pr that fixes it.
  -  When manually testing your feature before final PR submission write out test cases for both you and the reviewer. For example, I recently wrote a notifications feature. In addition to testing the feature itself, I also tested that it had not regressed in relationship to other features in the same controller.
  -  Your feature is not in a vacuum. When you develop something, always think what effect it will have on other features.
  -  Introduce randomness to your process. When NASA writes tests it also includes randomness. Why shouldn't you? For example, say you are developing a mobile login screen. Try adding a test that will trigger random x and y coordinates on the screen to see if any issues occur.
  -  Introduce different networking conditions to your app and see how it responds.
  -  Introduce memory leaks. See if it causes any crashes.
  -  Crash your app on purpose. See what the experience is like for the user post crash.

Stoic Development may help you become a better software developer and write better code. It may take some adjusting, but from my experience the quality of your product will be higher. If you prefer quality over quantity, then this should be your mantra.
Now you might ask, where are all the code examples? For that you will have to stay tuned for part two.
