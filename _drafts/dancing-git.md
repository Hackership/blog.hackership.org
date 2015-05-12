---
date: 2015-05-11
layout: post
title: "'Dancing Git' – a better way explaining Git in depth"
description: "There is better ways to give people in-depth understanding how git works. Try to let them dance it!"
category:
authors:
    - ben
tags: ["hackership", "Las Palmas", "Berlin", "batch-2", "Git", "workshop", "open education"]
image: /content/2015-05-06-dancing-git-repo.png
---

At Hackership people don't only sit at their laptops and code away. Very often to master a task, you have to understand abstract concepts and complex systems. Heck, he world of IT is full of if. One of these rather abstract systems is the Git. Learning not only to use it but understand Git is one of the most asked for topics to have a workshop about at Hackership.

Trying to untangle this abstract system, Hackership Coach [Carl Crowder](http://community.hackership.org/users/carlio) experimented with a new, highly interactive approach at Batch 14-07 in Berlin. Inspired by its potential [Stefan Wille](http://community.hackership.org/users/stefanwille/activity) and I extended the approach during the latest Batch in Gran Canaria to run it again, yielding better results than we could have ever imagined. Today, I want to share with you this approach of explaining Git and its internal system to software programmers of all degrees. Presenting:

## Dancing Git

![From our version at Batch 15-01 in Gran Canaria](/content/2015-05-06-dancing-git-repo.png)

**Basics Idea**

Recreate the life of a Git-repo and what goes on inside the `.git`-folder when various commands are execute. Using the learners as `git objects` either a `commit` holding a `tree` and pointing to their `predecessors` or being a `variable` pointing to another object. Pointers have hats of different variate to represent the abstracted git pointers like _head_, _branches_ and _tags_.

**What you will need**

 * three types of hats (maybe even put a sign on the hat)

    - one hat  _head_
    - three hats for _branches_
    - one hats for a _tag_.

 * a print out of our [Git Trees](LINKS MISSING) for the _sandwhich recipe_ we are compiling
 * learners
 * (at least) one coach

**Here is how you do it**

Please take a look at this video recording to get an idea on how to assemble the git repo, step by step while explaining one concept after each other.


<iframe style="display:block; margin: 10px auto" width="560" height="315" src="https://www.youtube.com/embed/Az40xWwNvfk" frameborder="0" allowfullscreen>&nbsp;</iframe>


_Note_: The talking throughout the exercise might seem a little confusing in the video recording. But it is very useful to have everyone understand what is going to. You should encourage them to ask questions, make sure everyone understands what goes on, when newer things happen, ask them to figure out where it is supposed to go.


For the record (and for you to not forget anything), here is the _script_:

1. Simple Repo

 1. Empty repo
 2. Add _head_ (with _hat_)
 3. Add _master_ (with _hat_), _head_ points to _master_
 4. **explain**: _object pointers_
 5. Add _first commit_
 6. _master_ points to _first commit_
 7. Add _second commit_ (pointing to its _predecessor_)
 8. **explain**: _branches_ are travelling references
 8. _master_ now needs to point to _second commit_

2. Branching

 1. Add second branch (_low on calories_)
 2. Let learners figure out, where it is supposed to go, where things have to point
 3. Explain _checkout_ to have _head_ point to new _branch_
 4. Add another commit
 5. Check out _master_ again
 6. Add commit to master

3. Merging

 1. Add a _merge commit_ (merging _low on calories_ into master)
 2. Resolve the conflict with the new change
 3. Explain that the merge-commits has to predecessors
 4. Delete _branch_

4. Tagging

 1. Add a Tag (other type of head)
 2. Add another commit on master – I forgot the bread
 3. Explain that master moved on, but tags do not

5. 'detached heads'

 1. checkout the commit (last one on low calories branch)
 2. Add another commit to this one
 3. explain what the problem is, when checking out _master_ now
 4. Checkout the _tag_ and how this creates a detached head, too


Standing there now, make room for questions. Once everyone understood it, give it a break.

We usually continue after the break by [recapping what we just did using git slang and giving some tips on naming](https://www.youtube.com/watch?v=W0LT5Zet91s), [explaining remotes, fetches and the exact terms](https://www.youtube.com/watch?v=2502nyT58io) using the great [explain-git-with-d3-tool](http://onlywei.github.io/explain-git-with-d3/) and have a _Git in Practice_ workshop to follow up a few days later.


---

You can find the [entire video series here](https://www.youtube.com/playlist?list=PLKWB6x05XySH9-093bQZwVEFkIDJW7eiZ).

This, as all learning material published by Hackership, is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>. Please go ahead and give this workshop. And if you have any feedback, please let us know.


