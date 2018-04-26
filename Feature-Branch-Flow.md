#Feature Branches and the R&D Dev Flow

So we hope to use feature branches and integration tests
to promote test-driven-development and accountability.

A lot of this structure is based on past lessons and the
development flow seen in some companies.

Currently, the LCS and frontend repositories have this fully
enforced.

## What Feature Branches Are

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

## Why Feature Branches

We use feature branches for accountability. This means that the feature
is written about somewhere, and its implementation is also discussed.

## How to Use

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

## All Hail the Robot Over-lords

So the hope is that we'll add automatic testing, linting, and deployment on our super-secured
master branches with this workflow. This will just make life nicer. Like who even wants to
deploy my bullshit at 2am? Only the robot.

## Kafka won't Complain (We hope not to be a Bureaucracy)

So we're humans (undergrads) too. So we don't enjoy berating your code and ideas.
We're doing this since we've shot ourselves in the foot. Repeatedly.

But, as fellow undergrads, we're here for you to talk to. So ask us. We're not
big brother, there are no Catch-22s, and our workflow is open to a metamorphosis.
