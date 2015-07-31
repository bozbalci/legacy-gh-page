---
layout: page
title: L'oiseau
permalink: /oiseau/
---

A [Last.fm][lastfm] scrobbler for [Music Player Daemon][mpd], written in Python.

Quoting [scmpc][scmpc]:

>”Another one?”, I hear you cry? Yes, I know about mpdscribble, but when I started this project it didn’t do entirely what I wanted it to. It didn’t run as a daemon, for example, and it didn’t work if you enable crossfading in MPD. I didn’t add the support for these in mpdscribble, partly because GNU coding style scares me, and I got slightly lost in the source code, but also because I created this as a way of teaching myself C programming.

I wrote oiseau because scmpc submitted multiple instances of a song to Last.fm. The "keeping unsubmitted songs in a queue saved to a file" feature didn't really work in scmpc. Originally, I wanted to write oiseau in C, but I didn't want to use glib, and I realized that it would make the experience extremely difficult (seeing as there isn't too much examples of programs which use libmpdclient and not glib)

Features
--------

* Scrobbling (obviously)
* Updates "Now Playing" on Last.fm when it can
* No duplicate scrobbles (almost guaranteed)
* Waits for a portion of the song to be finished before scrobbling
* Can set "scrobble after N tracks"
* Can cache tracks for later scrobbling
* Configuration file
* Run as a daemon

Installation
------------

Installation is relatively easy. Get the source from any of the links below, and run `python setup.py install` with the sufficent privileges. Then create a configuration file and you are ready to use oiseau.

For further information, see **README.rst**.

Source
------

* The latest source tarball is available here: [/oiseau-0.1.0.tar.gz][tarball]
* Git repository: [GitHub][github]

Development
-----------

If you'd like to get involved, if you have found any bugs, or if you have any feature requests, please open a [new issue][issue] in GitHub.

[lastfm]: http://www.last.fm/
[mpd]: http://www.musicpd.org/
[scmpc]: http://cmende.github.io/scmpc/
[tarball]: https://github.com/bozbalci/oiseau/archive/oiseau-v0.1.0.tar.gz
[github]: https://github.com/bozbalci/oiseau/
[issue]: https://github.com/bozbalci/oiseau/issues
