---
published: true
layout: post
author: Andrew Hoppin
title: Creating better DKAN documentation, as a community
---
With the release of DKAN 1.13, the core DKAN team is shifting to a new focus on our fantastic community of adopters and contributors (as well as, of course, supporting a ton of great [new features](http://docs.getdkan.com/en/latest/releases/notes/1.13.html)). While the community has always been a big part of DKAN’s development, the reality is that we haven’t always prioritized getting contributions directly from the global DKAN user community into DKAN itself. 

We want that to change, and after hearing a lot of feedback, we know our community does as well. For that reason, we’re truly prioritizing collaboration and engagement with users and developers from now on. With version 1.13, both the software and its community of adopters have reached a maturity that makes a more open and collaborative approach to development not only possible, but crucial to DKAN’s future.  

This community engagement initiative has basically taken the form of:

- A new set of documentation hosted on ReadTheDocs, focused on empowering adopters to use DKAN to its fullest potential, and
- Prioritizing bug reports and pull requests in our public GitHub repo.

These two are closely related because, after spending its first years of life as a separate Drupal site that developers outside our core team had no way to contribute to, the documentation now lives in the main DKAN repo itself. Users and developers can engage with the docs in the same way that they would engage with the code, via issues and pull requests in GitHub.

In a future post we’ll talk about how to actually work on and contribute to DKAN’s codebase, but today we want to start this conversation by focusing specifically on the docs. 

First, I’d invite you to review the [DKAN Technical Documentation](http://docs.getdkan.com/en/latest/) if you haven’t already. 

If you find a page in the docs that you’d like to improve, click “Edit on Github” in the top right corner of that page. You can also just look around the [/docs folder](https://github.com/NuCivic/dkan/tree/7.x-1.x/docs) in the Github repo, where all the files used to build the DKAN documentation site now live. Note that, while our original documentation was written in [MarkDown](https://daringfireball.net/projects/markdown/syntax), much of it has now been converted to [ReStructuredText](http://www.sphinx-doc.org/en/stable/rest.html), a more powerful human-readable format for writing technical documentation. You may need to take a little time to get used to the format, but it is fairly intuitive if you just follow the lead of the existing documentation.

Make your edits, then submit your suggested improvement as a “pull request” to that section of the DKAN Github repository.  If you’re not familiar with how to do this, here’s a [handy guide](https://www.thinkful.com/learn/github-pull-request-tutorial/#Opening-Your-Pull-Request).

Alternatively, if you can’t figure out the pull request process, or you have found something that you’re not sure how to address, simply note the issue for us as a [new Issue](https://github.com/NuCivic/dkan/issues/new) in the DKAN Github repository. Potential improvements could be as small as fixing a typo, or as large as writing an entire new section about a feature or process that you think isn’t sufficiently well-documented.  

Soliciting, triaging, and accepting community contribution to DKAN are a high priority for us going forward. I’d like to thank users like [bllkng](https://github.com/NuCivic/dkan/pull/1789) and [oriole9g](https://github.com/NuCivic/dkan/issues/1721) for the contributions they’ve already made to improving the docs with recent pull requests!


