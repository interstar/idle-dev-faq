IDLE-dev FAQ
============

This document came about from a [Feb 2014 idle-dev mailing list thread](https://mail.python.org/pipermail/idle-dev/2014-February/003377.html) about the need for a dev guide specifically for IDLE development.

###Getting Started

1. Read the general [Python Developer Guide](http://docs.python.org/devguide/).
1. Fill out the PSF's [Contributor Agreement](https://www.python.org/psf/contrib/contrib-form/)
1. Read [PEP 434](https://www.python.org/dev/peps/pep-0434/), which explains how IDLE development differs from Python development (re: backporting).
1. Familiarize yourself with the [idle-dev mailing list archive](https://mail.python.org/pipermail/idle-dev/) and read the last few years of discussion. (Don't worry, this is a relatively low volume list.)
1. Check out the [open issues on the Python bug tracker](https://bugs.python.org/issue?%40search_text=&ignore=file%3Acontent&title=&%40columns=title&id=&%40columns=id&stage=&creation=&creator=&activity=&%40columns=activity&%40sort=activity&actor=&nosy=&type=&components=6&versions=&dependencies=&assignee=&keywords=&priority=&status=1&%40columns=status&resolution=&nosy_count=&message_count=&%40group=&%40pagesize=50&%40startwith=0&%40sortdir=on&%40queryname=&%40old-queryname=&%40action=search), as well as the [closed issues](https://bugs.python.org/issue?@template=search&status=1) for a sense of history.
1. IDLE uses the Tkinter GUI toolkit in Python's standard library. Check out the following Tkinter tutorial resources:
    1. [YouTube tutorials by TheReimber](https://www.youtube.com/watch?v=rcACl0sUJeQ)
    1. Book: [Modern Tkinter for Busy Python Developers](http://www.amazon.com/Modern-Tkinter-Busy-Python-Developers-ebook/dp/B0071QDNLO)
    1. Demo code of Tkinter widgets: [A_tour_of_Tkinter_widgets](http://tkinter.unpythonic.net/wiki/A_tour_of_Tkinter_widgets)
1. Check out the [IDLE source code guide](source_code_guide.md)


A quick cheat-sheet / FAQ for people interested in contributing to Python IDLE development.


###Q: How do I get the source code of IDLE?

Use [Mercurial](http://mercurial.selenic.com/) and clone the repo at [https://hg.python.org/cpython](https://hg.python.org/cpython).

    $ hg clone https://hg.python.org/cpython


###Q: How do I get started contributing to IDLE?

 * Look at the [current bugs](http://bugs.python.org/issue?components=6&keywords=2&status=1&%40columns=id&%40columns=activity&%40columns=title&%40group=priority&%40sort=activity&%40action=search) in the issue tracker.
 * Fix one
 * Submit a patch. Note patches are always tied to issues in the tracker.

###Q: Where can I check-out the current state of IDLE development?

TODO (currently the mailing list)

###Q: Where can I see current issues?

On the issue tracker. [Here is a search for IDLE bugs](http://bugs.python.org/issue?components=6&keywords=2&status=1&%40columns=id&%40columns=activity&%40columns=title&%40group=priority&%40sort=activity&%40action=search)


###Q: Who do I submit patches to?

Submit patches on the [https://bugs.python.org/](https://bugs.python.org/) bug/issue tracker. Terry Reedy is currently responsible for IDLE issues, but anyone who is on the [nosy list](http://docs.python.org/devguide/triaging.html#nosy-list) of followers for the issue will get a notification if a patch is submitted.

###Q: How can I signal that I have a patch for someone to look at?

> Upload the patch to the related issue on the issue tracker. All people on the nosy list will get notified.

> Mark keyword 'patch' so the issue appears on [this search](http://bugs.python.org/issue?%40search_text=&ignore=file%3Acontent&title=&%40columns=title&id=&%40columns=id&stage=&creation=&creator=&activity=&%40columns=activity&%40sort=activity&actor=&nosy=&type=&components=6&versions=&dependencies=&assignee=&keywords=2&priority=&%40group=priority&status=1&%40columns=status&resolution=&nosy_count=&message_count=&%40pagesize=50&%40startwith=0&%40queryname=&%40old-queryname=&%40action=search)

> Trimmed and possibly not correct (I do not understand the %40s, nor how much
> the order matters):
> http://bugs.python.org/issue?components=6&keywords=2&status=1&%40columns=id&%40columns=activity&%40columns=title&%40group=priority&%40sort=activity&%40action=search
>


###Q: Where can I discuss IDLE development?

The [idle-dev mailing list](https://mail.python.org/mailman/listinfo/idle-dev). Discussions on the mailing list are friendly and civil, and users are expected to abide by the [PSF Code of Conduct](http://www.python.org/psf/codeofconduct/).

###Q: Are there other projects based off of IDLE?

[IdleX](http://idlex.sourceforge.net/) extends the functionality of IDLE with new features. [VIDLE for VPython](http://www.vpython.org/index.html) is also derived from the IDLE codebase.