For years I shipped boxed software. Quite literally, boxed. At Sun, we had a guy who's job title was "boxologist". He figured out what we could fit in to what kind of box and how to package it up. Not to do it, not to arrange the actual hard work of logistics. Just to figure out what could fit into a box. That's it, a full time guy, in 2006. (Not 1996. 2006!) (Possibly one of the reasons Sun didn't do so well, but I digress.)

Back in those funny days of boxed software, we'd ship things once every 2-3 years. It was a symbiotic fail: our customers couldn't test, QA and deploy new versions faster, and our product development couldn't develop, QA and release any faster. As the end of a release came up, it was a mad rush of work to get features in. The months before feature freeze were insane panic of forcing tons of things together in a dependency tree that makes a redwood look small.

Of course box or download: it's no different. When you have a long release cycle, regardless of the delivery method, you have a deadline. A deadline means you are either in or out. At some point, call it &lsquo;feature freeze', or &lsquo;the final iteration', you've got to package up what you have and actually get it to the customer. This process, the packaging, takes components from across your product, cutting across features and teams. Often the only common theme here is the deadline. Sure, there's probably an overall mission &ndash; introduce massive awesome feature X, clean up bugs Y, but the reality is vast swaths of code will have nothing to do with this mission. They will be the various cruft that builds up over time and NEEDS to get out to customers.

Deadlines are nasty things. Miss them, and you are in a world of hurt. Either you push the deadline for everyone else back to fit in, or you've got to wait till the next go around. Pushing back the deadline only leads to madness. Once you start pushing, it's almost impossible to stop that other team over there who can now add in their feature that **just** missed. Till that feature has as bug, and pushed the deadline even further back. And then someone else will have something to put in. Once you cross the line and push your deadline, you're in [slipping-for-years](http://en.wikipedia.org/wiki/Windows_Vista) mode.

## Iterations – because you want more deadlines?

The rational decision is to stick to the deadline, and push to the next release. With packaged software, maybe you'll wait a few years for that next release. That just ratchets up the pressure around hitting the deadlines 1000 times, making the bugs, the confusion, and the unnatural acts that much worse. The obvious solution is to shorten the release cycle. Release more often, say once every 6 months instead. Why stop there? With cloud delivery, we've removed the  pain of updating from the customer.  A well developed cloud app allows for transparent updates without an acceptance loop from the customer. This means there are no more constraints on how often you can release. Do it every month, or heck, every week.

However, if you're talking about releasing every X period, &ldquo;You're Doing It Wrong&rdquo; &trade;. By definition, you've still got deadlines. Sure, they're smaller, but they are there. All the same problems discussed above continue to exist, toned down, handled more frequently in smaller chunks, but fundamentally unchanged. You have still forced your company to make tradeoff decisions based on timelines.

## Developers have Flow &ndash; Products have Momentum

Individual creatives are aiming for [flow](http://en.wikipedia.org/wiki/Flow_(psychology)). Cranking out code, art, words. Just hammering away. In one session of good flow state I get more done than in weeks of fits and starts. Everyone has their own path to getting to flow. Some put on the headphones, wear a hoodie, and disappear into their computer. Others go to a coffee shop, let the white noise wash over them, and get into the zone. Sometimes though, the conditions are right, but the project isn't willing.</p>

Blog posts, software development, homework: we are all familiar with the experience of working incredibly &lsquo;hard', but just not getting anywhere. 20 hours in, and you just don't feel like you have a sense for how to even begin to tackle the project. Flow has it's own [conditions][]. Without clear understanding of goals, you aren't getting anywhere. Goals don't come from flow. They come from somewhere else. When you're creating, working on something innovative, they often seem to come from the subconscious. When you're stuck, and don't have a clear sense of the goal, if you're lucky, you walk away. You take a break. Maybe for 30 min. Maybe for a month or longer. And something happens. A shift. A new angle. A comment. Inspiration. You can pick the project back up again, and now you've got traction. You can push just as hard and make some real progress. You personally can get into flow. Your project can pick up momentum.

Momentum is fickle. It's not something you can predict, store, save and spend. Some projects are real bastards &ndash; they get stuck just when you think you're making the most progress. Sometimes you need to [put it down and pick it up 6 times over 13 months](http://devcenter.heroku.com/articles/cedar) before you finally cross the finish line. Some projects get momentum from the second you sit down, and one night later you've launched.

## Continuously avoid the death march.

Working against a project's momentum is about the most painful work experience I know of, and the standard name express it well: the [Death March][]. Deadlines mean death marches. Maybe small ones. Maybe huge ones. But if you've got a deadline, you've incorporated into your project &lsquo;death march by design.' The shorter the cycle, the smaller the potential, but even 1 week release cycles have a mini-death march built in.

Continuous deployment gives you the option to free yourself from the death march. As soon as you have a feature/bug fix/whatever, ship it. Don't wait for an artificial iteration to pass. If it works, if you are ready, if you've managed the lifecycle of the change, ship it. If you're not ready, don't. Releasing is hard work. You need to make sure it works. You need to test it with a segment of your customers. You need to think through all the permutations and impacts of your change. Slow down. Take the time to make sure you're doing it right.

Don't push things that don't have momentum. You've got 1000s of projects to work on, and 100s that are all amazingly valuable. Pick the one that's &lsquo;ready', work on it till you're not making progress, and then walk away. Take on something else. When it's ready, you'll know. The work you put in will deliver results. You'll be energized. It's obvious once you've experienced it. It's liberating.

## Slow in, fast out

Here's where the magic is. Your customers have no idea what your development process looks like. They have no idea what you're picking up and putting down. They see what you release. That's it. If you're following the momentum, you probably have a few projects in process at all times. Pick one up, put it down. Pick a different one up. Put it down. When and only when a feature is ready, push it out. This only works if you're deploying all the time. Not weekly, ideally not even daily. Deploy when it's ready. This lets you focus on just one thing. When feature Z is ready, ship it. No dependencies. Remove the complexity across projects. Once you've done that, you can walk away from projects at any time. There's no fear that if you miss the deploy next month, you'll have to wait 45 weeks till you can get it out again. You can get it out when it's ready. Tomorrow or next year.</p>

There's a word for this: you are [pipelining][] your development process. You will likely be releasing features significantly more frequently to your users, specifically because you're willing to walk away when they aren't ready.  This point bears repeating: by specifically trying to slow down, by not pushing things, by juggling a number of projects at once, you will actually ship to your customers more value, more often.


Thanks to [Adam Wiggins](http://adam.heroku.com/), [Rich Miller](www.telematica.com) and [Mark McGranaghan](http://mmcgrana.github.com/)for reviewing and providing feedback on this blog.

[pipelineing]: http://en.wikipedia.org/wiki/Pipeline_(computing)
[death march]: http://en.wikipedia.org/wiki/Death_march_(project_management)
[conditions]: http://en.wikipedia.org/wiki/Flow_(psychology)#Conditions_for_flow