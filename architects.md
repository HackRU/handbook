# Wilkommen

Hallo und wilkommen am der dokument für architekten.

Because I don't speak German and you probably don't, I'll start again:

# Welcome

Hello and welcome to the document for architects.

Jokes and immaturity aside, this is an explanation of what it means to be an architect.
Because we love the notion and the job and all of running R&D, there'll be a lot of stuff
written here. But we're R&D, so there is a table of contents, because ain't nobody got time
for reading the whole manual.

**Sections**:
 - [What is an architect](#what-is-an-architect)
 - [The work - the projects](#projects)
 - [The people](#people)
 - [The meetings](#meetings)
 - [Coping and life tips](#coping)

# What is an architect?

We actually spent a few hours deciding on this name. The other organizers in other HackRU
teams are just called "organizers." But there were ideas and most of them sucked:
1. builders - but you don't just build.
1. creators - but creation isn't the sole purpose.
1. designer - but MnD has designers and design is not all that makes great applications.
1. organizer - but you're special.

Therefore, we suck to **architect**. This is to emphasize that you do not only create or build or
code your application. You architect it - you chose a lot of the structure and look and feel of the
application you're making. You chose the libraries and all the small decisions that power it.
Hence, you chose the architecture. You're also not just a designer - the considerations are not
merely aesthetic and you stay with the application as it is built, tweaking your design.

So we expect a few things from you, giving you the title of architect:
 - we expect you to be able to design and problem solve.
 - we expect you to stay with your application for as long as possible.

## Why be an architect?

There is nowhere else in your undergraduate career where you're guaranteed to have 600 users
of an app that you design and code.

_(OK, there's OSS and your internships, but both don't give you this much flexibility.)_

So, if anything, this is a huge resume boost. And you get to have fun, ownership, pride, and if you
stay for long enough, leadership.

# Projects

You're expected to work on a project as an architect. The project can come from you or the rest of
HackRU.

The projects can be in any phase: it could have never existed before, it could be an unmaintained
thing we dug up, or - most likely - it could be a project that served the last HackRU but needs
tweaks and maintenance.

## The Usual Suspects

The projects are usually as follows:
 - LCS: the backend
 - The one app (android): the mobile app for android.
 - The one app (iOS): the mobile app for iOS.
 - SlackRU: the mentorship slackbot.
 - Sledge: the judging app.
 - The web front-end.
 - team-builder: A team-building application.

## Some Common Ideas

Here are some ideas and why they have yet to be implemented.
 - A snack tracking thing: we wanted to track the snacks consumed by the hackers. This is just hard to implement and nobody in the food team wants it anymore.
 - A self-driving snack cart: too much liability...
 - A scheduler for volunteers and mentors: VHX need to be talked to. A lack of time and communication is the only cause.

# People

This is about how R&D is organized and the people you may have to deal with as an architect.

## Your Project Lead

Your project will be lead by a fellow architect. They're your boss (senpai, if you care for it) and
so have a bit more power. Hence, though you get to make decisions, you do not get to override theirs.
Additionally, you will be given tasks from this leader. You should do them.

If you think your lead is unfair for whatever reason, you can bring it up to the directors and they'll
handle the case.

## The R&D Directors

The R&D directors are the project leads' project leads. They interface with the rest of HackRU and
lead the project leads on the overarching goals for each project.

We are there for you. We can meet with you if you have any problems. Also, on a technical note,
we take care of the interviews.

## The Rest of HackRU

The HackRU organizing team is one of the largest. As a result, you'll have a lot of fellow organizers
across the teams.

They will not know about your project, most of the time. So in terms of explaining it, you might as
well treat them like regular users - just with more powers and more knowledge about their team in
HackRU.

You may have to meet these people, depending on your project and project lead. Remember that they
care about HackRU as much as you do!

## Hackers

You will, in a mix of fortune and misfortune, have to deal with the end-users of your applications as
well. These people are the people you were serving. And they do not understand your struggles.
You should not help them understand your struggles either - they should live with the illusion that
the application is running smoothly as it always was.

You will know just how much you'll have to talk to hackers after talking to your project leads.

# Meetings

There are a few types of meetings you'll have to care about.

## R&D Meetings

We meet as a whole R&D team to discuss the team's goals and how all the teams are doing.

While this is the directors' key tool to understand the team's progress and blockers, it is also
a chance for you to know how R&D is working. If it is healthy, you would be able to follow the updates
that every project lead is giving and feel a sense of progress in general.

The meetings will start with project leads describing the work done in the past week and the goals for the next.
Then your project will be grouped and allowed to work for upwards of an hour.

## Project Meetings

If your project is also in a critical phase or moving along quickly, or simply so chooses, you may
meet your project leads and people on your project to work on the project.

These will vary sharply but should be rather informal.

## Other HackRU Meetings

You might, depending on your project leader, go to other HackRU meetings - like director meetings
and the meetings of other teams. You will have to respect the other teams and be polite. Your
project lead and perhaps the directors will give you relevant tips at R&D meetings as they come up.

# Coping

Being an architect is not easy. There are various dimensions of hurt that can happen. A few hours
ago, in conversation with project leads, I found myself saying that 0.03 of my GPA can be attributed
as lost due to R&D. This is as a junior, so 0.03 is not _that_ small. I owe a B+ at least to R&D.
In fact, we ask you how much of your soul you'll sell to HackRU. The organizers who take this question
as a joke do not last: they're quickly outpaced by the all-nighter pulling maniacs around them.

OK, but this is about coping... so why do I talk about all the hard work it is? So that you feel
vindicated of course. HackRU is one of the few places in the world where hard work is directly
rewarded.

But you need to cope with a lot of things. So here are some tips:

Ez wrote up some nice ones on [the frontend repo's README](https://github.com/HackRU/frontend/tree/bastard).

## How not to panic

Every README in this organization should be prefixed with a "do not panic." Remember that at some point,
everybody around you was just as clueless as you may be. The code did not write itself - somebody
thought about it for a long. long time. As a believer that P < NP, I'll be the first to say: they
probably had a harder time writing the code than you will reading it. It's just that you can
see your efforts in reading more clearly than theirs in writing.

Just ask about how to test the code, make sure you can install it, and break it. Seriously. We use
version control, so you can nuke your copies as many times as you want to.

If you have questions ask them. If not to a fellow architect, the project lead. If not the project lead,
a director. If not a director, the alumni mentor. If not them, may be google. But be open about
how daunting the code base is. With experience, steep learning curves are easy to forget, so the
leads and directors and alumni may not understand exactly how high up the code base seems for you.
Just tell them. It's their job to help you feel that you understand your work.

## Impostor Syndrome

This is the feeling that, despite you deserving an accolade, you do not feel that you are worthy.

I'm tempted to explain some I occasionally have. (I'm Heman, one of the first R&D co-directors.)
I feel that I don't deserve to be a director for R&D quite often: I was at the right place
at the right time - when Carlin wanted an R&D team, directing a useless one. And I was only ever
there and remotely decent in CS because of my dad's career choices.

So yeah... that's the syndrome. I don't know how to deal with it. I ignore it. So that we're
both healthier, [I found some tips.](https://lifehacker.com/overcoming-impostor-syndrome-what-to-do-when-you-feel-1651827849)

## Stress

Again, I don't think I have great coping mechanisms. I just pull all-nighters and am a caffeine addict.
But you should try to have lists and priorities. Do small tasks.

Most of all, tell people if you have other commitments or too much work. It's alright to do so. And
it's even more alright to leave R&D for some time. Just let us know that you will.

## Fire on Prod

Yes, you can set prod on fire. And users will see it and know of your failures. Hooray.

This is not something that should put you off R&D. Know that the directors have put their own
fires on prod. The team is there for you. We will do whatever we can to help you fix your bug.
Just talk to us and help us understand the crashing.

Internally, you should accept the fire too - you did it, it sucks, but you grew. The team grew.
If everything went well, everybody learned.
