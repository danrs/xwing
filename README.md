(Yet Another) X-Wing Miniatures Squad Builder
=============================================

[![Build Status](https://travis-ci.org/geordanr/xwing.png)](https://travis-ci.org/geordanr/xwing)

What?
-----
This is a squad builder for Fantasy Flight Games' X-Wing Miniatures game, completely in HTML and JavaScript.  No backend is necessary.
It can theoretically be dropped into any existing site, but since it uses a lot of styling from [Twitter Bootstrap](http://twitter.github.com/bootstrap/) it may require some CSS trickery if you're using some other incompatible framework (e.g. [Foundation](http://foundation.zurb.com)).

Can I save squads or share them on `$SOCIAL_NETWORK`?
-----------------------------------------------------
Saving: yes, if you provide a backend that adheres to the API.  See my [X-Wing Backend](https://github.com/geordanr/xwing-backend) project for an example.  Sharing, no.

Aren't there other squad builders out there already?
----------------------------------------------------
Yes.

So...?
------
MAGIC

What happened to Geordanr?
-----------------------
He 'retired'. I took over.

When will this be done?
-----------------------
Whenever FFG stops releasing content for the game.

Building
========

1. Install [Node.js](http://nodejs.org/) to get `npm`.
2. `sudo npm install -g grunt-cli` to install the global Grunt CLI.
3. `npm install` to install the dependencies listed in `package.json`.
4. `grunt` to build everything into the `app` directory.  The builder is at `app/index.html`.

Deployment
==========

1. Check out the `deploy` branch and rebase on top of master for any changes
2. Build as per instructions above
3. `mv app docs # move the build to a directory that the pages builder can see`
4. `git push origin deploy`


Translation
===========

Wanna help translating YASB into your language? See instructions in the
`translation_helper/README.md` file.

Exporting Squads
===========

[Squad2xws](https://github.com/zacharyp/squad2xws) allows you to export squads you have created to xws format for use in other places. Take the url of the squad you have built, replace the "https://raithos.github.io/" part of the url with "https://squad2xws.herokuapp.com/yasb/xws" and it will output your squad in the xws format to be used for whatever.

Credits
-------
[X-Wing Miniatures](http://www.fantasyflightgames.com/edge_minisite.asp?eidm=174&enmi=X-Wing) is by [Fantasy Flight Games](http://www.fantasyflightgames.com/index.asp).
Icons and fonts originally from GeckoTH's excellent PSD, available [here](http://www.afewmaneuvers.com/topic/122-hi-res-photoshop-templates/).
X-Wing symbols and ships fonts courtesy [Hinny](https://github.com/Hinny) and [Josh Derksen](https://github.com/armoredgear7) and are available as a [Bower package](https://github.com/geordanr/xwing-miniatures-font).
Maneuver dial support by @hpanderson.
Fancy printout design inspired by TheKestrel on the FFG forums.
Upgrade card text integrated into printouts by [wffurr](https://github.com/wffurr).
Squad name in the permalink and obstacles choice modal by [zacharyp](https://github.com/zacharyp).

I'm bad at keeping this up to date; see the About section of the builder.

CHANGELOG
=========

01 Aug 2018
-----------
Initial Relase of 2.0
