---
layout: postCommentit
title: 'Launching Comm(ent|it) (aka comments on Github Pages)'
---

*If you just want to try Comm(ent|it) without reading the all story, go, it is
there, on [commentit.io](https://commentit.io/) !*

I have been working on [Comm(ent|it)](https://commentit.io) since January 2015.
When I had created this blog one year before, I had told myself that third party
comment systems were only a temporary solution. Like many of us, my blog is
powered by the static website generator <a href="#">Jekyll</a> and is hosted on
<a href="https://pages.github.com">Github Pages</a>. Jekyll is by definition not
able to include such a feature as a comment system.

I had seen some bloggers who also did not want to store comments outside their
website. Some of them had just no comment system. Other had a "pull request"
button, for users directly to modify the post file, and add there comment at
the end of it. I found this very smart and even funny, as it gives you a lot of
freedom in the way you manage and display comments.

But it has several drawbacks. The first one is that any commenter needs to have
a Github account and know how pull requests work. This is a real problem, as many
of our readers are not experts in that field. This can cause merge conflicts,
website owner has to do some work so no one breaks the layout, and every comment
has to be pre-validated before appearing on the blog.

This gave me the idea to create Comm(ent|it), a service which automates the
process of storing comments in website repository through commits and pull
requests. Of course, I added several features. With Comm(ent|it), we have the
possibility to send comments directly to master or gh-pages branch. And there
are smarter ways to store comments than directly at the end of each post file.
It could be better and more beautiful (I am not a web developper), but I think
it does the job.

When we talk about static website generators, some people completely oppose them
to dynamic systems such as Wordpress or any PHP CMS (which often handle comments
natively). But what are really the features that make the difference between
them ? Both can have some kind of databases, PHP CMSs through MySQL and Jekyll
through database files. All have templates, rich text features. They can update
a homepage or a feed based on the last content. Dynamic websites generate HTML
files on the fly, whereas Jekyll generates them on content updates. But
dynamic websites sometimes have cache systems, which are warmed up on content
updates and serve entirely static HTML pages.

Not to say Wordpress and Jekyll are the same, of course not. The big difference
remains that Jekyll cannot handle any POST request, and cannot use sessions or
even cookies. But with Jekyll we can imagine a system where serving the content
and updating it are the role of two decoupled services. And both could be user
friendly. This can have advantages in term of security and portability.
