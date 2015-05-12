---
date: 2015-05-11
layout: post
title: "'Dancing Git' – How To Explain Git In Depth"
description: "Ever tried teaching the inner workings of Git to other developers? It can get pretty messy, if not confusing. We came up with a somewhat unorthodox approach that has learners dance Git.
Wait what? Did you say DANCE Git?
Yes. We did. Here's what such a workshop looks like and how you can host your own!"
category:
authors:
    - ben
tags: ["hackership", "Las Palmas", "Berlin", "batch-2", "Git", "workshop", "open education"]
image: /content/2015-05-06-dancing-git-repo.png
---

Becoming a great developer requires a deep understanding of the tools you use. Our learners know that and will often ask us to explain more. That's not always easy. Understanding something is one thing, explaining them effectively to another human being is another thing altogether.

Take Git for example. Most of us know how to use Git for day-to-day version control. But, **how well do you really understand Git?** What exactly goes on under the hood? And how would you explain that to someone else, without them getting utterly confused?

Hackership Coach [Carl Crowder](http://community.hackership.org/users/carlio) was tasked with untangling this complex system and creating a workshop that clearly explains the inner workings of Git to our learners. He came up with a highly interactive approach and one of the most successful workshops during Batch 14-07 in Berlin. Inspired by this workshop [Stefan Wille](http://community.hackership.org/users/stefanwille/activity) and I extended Carl's approach during our latest Batch of Hackership in Gran Canaria. The resulting workshop yielded better results than we could have ever imagined.

Now, we would like to share exactly what we did to effectively explain advanced Git to experienced programmers. What follows is essentially a how-to guide, helping you to host a similar workshop for your community. This guide is meant for people who already understand Git (at a deeper level), but are looking for a new way to teach it to others.

## Dancing Git

![From our version at Batch 15-01 in Gran Canaria](/content/2015-05-06-dancing-git-repo.png)

**Basics Idea**

Our basic idea was to recreate the life of a Git-repo and what goes on inside the `.git`-folder when various commands are executed. We used our learners as `git objects`. Some of them would play the role of a  `commit` holding a `tree` and pointing to their `predecessors`, others would be a `variable` pointing to another object. We gave pointers hats of different colors to represent the abstracted git pointers like `head`, _branches_ and _tags_.


**What you will need**

 * three types of hats (maybe even put a sign on the hat)

    - one hat  `head`
    - three hats for _branches_
    - one hats for a _tag_.

 * a print out of our [Git Trees](LINKS MISSING) for the _sandwhich recipe_ we are compiling
 * learners
 * (at least) one coach

**Here is how you do it**

Please take a look at this video recording to get an idea on how to assemble the git repo, step by step while explaining one concept after each other.


<iframe style="display:block; margin: 10px auto" width="560" height="315" src="https://www.youtube.com/embed/Az40xWwNvfk" frameborder="0" allowfullscreen>&nbsp;</iframe>


_Note_: As you probably observed, there's a lot of talking going on throughout the exercise. That's on purpose. Allowing people to interact is a good way for everyone to make sure thet understand what is going to. You should encourage learners to ask questions. Also, when newer things happen and new actions are introduced, ask participants to figure out where the new thing is supposed to go, rather then just telling them.


For the record (and for you to not forget anything), here is the _script_:

1. Simple Repo

 1. Empty repo
 2. Add `head` (with _hat_)
 3. Add `master` (with _hat_), `head` points to `master`
 4. **explain**: _object pointers_
 5. Add `first commit`
 6. `master` points to `first commit`
 7. Add `second commit` (pointing to its _predecessor_)
 8. **explain**: _branches_ are travelling references
 8. `master` now needs to point to `second commit`

2. Branching

 1. Add second branch (_low on calories_)
 2. Let learners figure out, where it is supposed to go, where things have to point
 3. Explain _checkout_ to have `head` point to new `branch`
 4. Add another commit
 5. Check out `master` again
 6. Add commit to master

3. Merging

 1. Add a `merge commit` (merging _low on calories_ into master)
 2. Resolve the conflict with the new change
 3. Explain that the merge-commits has to predecessors
 4. Delete `branch`

4. Tagging

 1. Add a Tag (other type of head)
 2. Add another commit on master – I forgot the bread
 3. Explain that master moved on, but tags do not

5. 'detached heads'

 1. checkout the commit (last one on low calories branch)
 2. Add another commit to this one
 3. explain what the problem is, when checking out `master` now
 4. Checkout the _tag_ and how this creates a detached head, too


Before everyone sits down again, make sure you answered any and all questions. There tend to be quite a few, so give everyone a chance to clear up any confusions they may have and to get familiar with all these new concepts. Once everyone understood it, make sure to take a break. The brain needs it!

We usually continue after the break by [recapping what we just did using the actual git wording and giving some tips on naming](https://www.youtube.com/watch?v=W0LT5Zet91s), followed by [explaining remotes and fetches](https://www.youtube.com/watch?v=2502nyT58io) using the great [explain-git-with-d3-tool](http://onlywei.github.io/explain-git-with-d3/).

Finally, if you have the time, we found that holding a [Git in Practice](https://www.youtube.com/watch?v=ESbqb-xx24o&feature=youtu.be) workshop a couple of days later is a great way to make sure everyone really understood what was going on and to improve retention.

That's it. Our Git workshop. Now it's your turn to host your own. Good luck! And please let us know if you have questions (check out the comments below). We're here to help!

---

You can find the [entire video series here](https://www.youtube.com/playlist?list=PLKWB6x05XySH9-093bQZwVEFkIDJW7eiZ).

This and all other learning material published by Hackership, is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>. Please go ahead and give this workshop. And if you have any feedback, please let us know.


