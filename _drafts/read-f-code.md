---
date: 2015-06-01
layout: post
title: "Read f* code – resource list"
description: "To become a good writer, one must read a lot – the saying goes. This is as true for writing code as for books. Whether you consider it a craft or an art, to become better at writing code you need to excercise (write code) and you need to study. And there is no better way to study how to programm, how to design and structure programs, how to build architectures and name things, than reading others peoples code. Unfortunately there is a lot of bad code out there. Here is our list of a few great code resources to read and learn from."
category:
authors:
    - ben
tags: ["hackership", "material", "read code", "code", "open education"]

---

To become a good writer, one must read a lot – the saying goes. This is as true for writing code as for books. Whether you consider it a craft or an art, to become better at writing code you need to excercise (write code) and you need to study. And there is no better way to study how to programm, how to design and structure programs, how to build architectures and name things, than reading others peoples code. Unfortunately there is a lot of bad code out there. Here is our list of a few great code resources to read and learn from.

- **Real World Implementation of Text book Algorithms**

  Yes, they do really get implemented from time to time. And it is actually quite interesting to see, how this works (and changes) in practice. There has [been a great StackExchange Thread on this a while back](http://cstheory.stackexchange.com/a/19773), covering all types of Lists, Hashes, Searches, Sorting and so on. Highly recommended!

- **[BackboneJS][1]**

  is a one-1500lines-files implementing a whole frontend-side MVC and uses advanced JS features to do that. Highly recommended comes their [Annotated Source Code][2] (yes, they have annotated the whole source file for your consumption)

- **[UnderscoreJS][3]**

  along with that comes UnderscoreJS, which also has a [fully annotated source code][4] and that backbone uses exensively to its job done.

- **Linux Kernel**

  As you might have noticed on the top about *core-algorithm*, of course the **Linux Kernel** is a great project not only having an amazing infrastructure but also just very elegant code. And we aren't the first to realise it, actually there are [full][6] [fletched][7] [tours][8] on the Linux Source code and [helpful pointer on where][9] to get started.

- **Python's NDB**

  If you know yourself some Python and Metaclasses and have some knowledge on Key-Value-Store-Database-Theory, Guido van Rossum, inventor of Python, totally rewrote the  Database layer of Google AppEngine (on BigTable) and it is incredible. You can find the full source code of [**NDB** here][10].

- **HTTP Stack**

  If you are interested to learn more about the HTTP-Protocol and Web-Stacks, there are two really elegantly build projects I'd recommend reading: the ruby-framework **[Sinatra][12]** ([start at base.rb][13]) and the Python framework **[flask][14]** ([start at app.py][15])

---

<img src="/uploads/default/49/a4d7106692a15c14.jpg" width="640" height="360"> 


  [1]: http://backbonejs.org/
  [2]: http://backbonejs.org/docs/backbone.html
  [3]: http://underscorejs.org/
  [4]: http://underscorejs.org/docs/underscore.html
  [6]: http://en.wikiversity.org/wiki/Reading_the_Linux_Kernel_Sources
  [7]: http://www.tamacom.com/tour.html
  [8]: http://www.youtube.com/watch?v=y7SWXTyXF0E
  [9]: http://stackoverflow.com/a/1016109
  [10]: http://code.google.com/p/appengine-ndb-experiment/source/browse/
  [12]: http://www.sinatrarb.com/
  [13]: https://github.com/sinatra/sinatra/blob/master/lib/sinatra/base.rb
  [14]: http://flask.pocoo.org/
  [15]: https://github.com/mitsuhiko/flask/blob/master/flask/app.py