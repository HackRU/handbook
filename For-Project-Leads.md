# UWU, what this?

This is documentation for how to project-lead for HackRU R&D.

Below we have how your role works. Being in the middle can suck:
your team gets to blame you for fires and the directors point at you
when their execs complain. But rest assured, you too can not only point around,
but also read this document to understand how your roles works!

We have sections organized by priority:
1. How to deal with your team.
1. How to deal with the directors. [It's a bit of a scroll...](#dealing-with-directors)
1. A few dev-related ideas. [Right at the bottom...](#feature-branches-and-the-r&d-dev-flow)

## Getting a Team

Just because you're leading a project, doesn't mean you'll be doing the most work on it.

You should have a team and you get to assign them work. Be fair. We can summarize the rules
as "don't be evil," but then we would be Google. Really, we let anybody work on anything
and you should strive to that - as long as people aren't over-committed.

We can go over managing teams in terms of the hurdles:
1. How not to intimidate people and have them know what to do: maintain [a good git community](#a-good-git-community).
1. How to make sure people are doing their work: [politely pressure them](#polite=pressuring) and [have regular meetings](#team-meetings).

### A Good Git Community

A good way to make your project accessible is to make it a decent part of the open source
world. Luckily, there's a big open source world out there with [its own guides](https://opensource.guide/best-practices/).

A few of these are dev tips that we also mention below, but all the tips are very nice to keep in mind!
If this is well organized and the vision is stated, not only will it be easier for people to find information,
but you'll have an easier time staying on top of the project's goals.

But how does this help newbies? Newbies will also find it easier since you'll generally be more articulate
about what they can do for you. This helps a lot! You'll find yourself frequently wishing that
there was a glossary for your project and that people could implant it into their brains so that
your nicknames, metaphors, metonymies, ideas, and code all make sense. A good open source community
can be just that! Then newbies don't always have to ask you - they can consult the community.

### Polite Pressuring

The sad part about being a student-run organization is that students are students, first and foremost.
This applies to you too - we'll talk about that in the next section - but it applies to your team.
This will make scheduling hard (there's always an 8 pm class and a commuter who can't stay past 7).
But that can be managed with the power of tech: video-calls, GitHub, and the discord will all help.
But nothing is worse than when a team has midterms - all at the same time.

This is why, while you have important things that your team needs to do and your goals and aspirations,
Rutgers and the fact that people are students have other plans.

Just be polite and open to people coming back if they're committed. Because people make mistakes and
should be given more than one chance.

However, don't be afraid to say "no" either. If a team member hasn't been participating and suddenly
demands a large, important task, you can say no. In fact, odds are, you should say no. Give them a smaller
task.

Give your team members a clear path and be open to slight delays, but don't forget your right to reset
them on their path if you have to.

### Team Meetings

You should meet with your team. This does not have to be very formal, but should be regular.
We recommend weekly meetings since you can use the R&D meetings as this time anyway.

Make sure that you know what your team members are generally doing: are they in difficult classes,
do they have a tall stack of extracurriculars? This will help you and the team be a team.
The team meetings are where the less personal elements of this can arise. (Or if your team is a
glorified friend-group, as teams are wont to become, discuss whatever you feel is necessary.)

Remember, too, that your meetings should update you on your code-base and project status.
They are your team member's chance to know more about the project and the bigger picture framing their
task, so take these meetings somewhat seriously - let members actively contribute, just as they should
be in the code-base. Acknowledge achievements and rectify failures.

## Dealing With Directors

The directors are there to help you and are your interface to the rest of HackRU.
Hence, if you have any problems, they should be your first point of contact.

There are a few specific things your should know...

### The R&D Meetings

The directors will run meetings to catch up with the whole team.
Here, you will be expected to update all of R&D on your project.
This is very informal. Banter is looked forward to. But this is your responsibility:
you have to allow other teams to understand your project's status.

### The Rest of HackRU

The greatest thing about R&D is that your code is not in a vacuum: people use it.
But that also means that you have to deal with end-users in a way.
There are two types of end-users: the hackers and your fellow organizers.

The R&D directors will help with the below facets, but knowing these general things is helpful.

#### Hackers

Whatever subset of your team shows up on the day of HackRU will be expected to help people use
your project. This means that you and your team must know the bugs, errors, and design of the code.

This also means that you have to deal "customers" and so you have to be polite and understanding.
Make sure that whoever is dealing with hackers is relaxed and semi-rested. (This could include the directors.)

#### Other Organizers and Directors

In many cases, other organizers might as well be hackers: they too have no clue how your amazing tool
has been built.

The key difference is that organizers have the power, before the even, to change your project's specs.
You should be receptive to their feedback, but also reasonable about you and your team's capabilities.

### Director Meetings

If your project needs a lot of feedback from another team, the directors will invite you to meet with
that team. On the same note, you can be invited to meet all the directors and get a lot of feedback.

Unfortunately, these are also usually time-consuming. They're not worthy of any stress: there's simply a
lot of information passed around.

## Feature Branches and the R&D Dev Flow

So we hope to use feature branches and integration tests
to promote test-driven-development and accountability.

A lot of this structure is based on past lessons and the
development flow seen in some companies.

Currently, the LCS and frontend repositories have this fully
enforced.

### What Feature Branches Are

So in order to know a feature branch, you must know what a
feature is and what a branch is.

A feature is... a feature - an improvement, fix, or change
that you want to add on the GitHub. We may have features we
want to see written about in issues, but any feature is a feature.

A branch is a version of the code's history. Literally just another
version of the repository. This allows for parallel development without
some features affecting others.

So feature branches are branches made to implement, debug, and test a
feature.

### Why Feature Branches

We use feature branches for accountability. This means that the feature
is written about somewhere, and its implementation is also discussed.

### How to Use

This assumes you're comfy with the committing,
pulling, cloning, and pushing bits of git.

So you always branch off master. `master` is the main branch that has the
version of code that R&D will ship. Let's say you're implementing `cool-feature`
(please actually name your branches in a more self-documenting way - it helps
with the sanity). Firstly, you make the branch:
```
git checkout -b cool-feature
```
Now all your commits will go there.
```
git push --set-upstream origin/cool-feature
```
makes it so that GitHub knows where you're pushing to. You'll have to do this the
first time you push. (If you forget, the error message will remind you.)

When you think it's ready, you can open a pull request. We'll bother with the merging,
telling you to fix stuff, etc. Once it's merged, we'll delete the branch remotely and
locally, you ought to:
```
git branch -d cool-feature
```
(if it yells and you and you're 100% sure everything's merged, just use `-D` instead).

### All Hail the Robot Over-lords

So the hope is that we'll add automatic testing, linting, and deployment on our super-secured
master branches with this workflow. This will just make life nicer. Like who even wants to
deploy my bullshit at 2am? Only the robot.

### Kafka won't Complain (We hope not to be a Bureaucracy)

So we're humans (undergrads) too. So we don't enjoy berating your code and ideas.
We're doing this since we've shot ourselves in the foot. Repeatedly.

But, as fellow undergrads, we're here for you to talk to. So ask us. We're not
gig brother, there are no Catch-22s, and our workflow is open to a metamorphosis.
