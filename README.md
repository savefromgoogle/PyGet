# PyGet

![version 0.28](https://img.shields.io/badge/version-0.28-green.svg)
![python 2.7.2](https://img.shields.io/badge/python-2.7.2-yellow.svg)
![dependencies progressbar](https://img.shields.io/badge/dependencies-progressbar-green.svg)
![license GPLv2](https://img.shields.io/badge/license-GPLv2-green.svg)
![platform linux](https://img.shields.io/badge/platform-linux-green.svg)

Contents:

1. [About Pyget](#about-pyget)
2. [Installation](#installation)
3. [Basic Usage](#basic-usage)
4. [Advanced Usage](#advanced-usage)
5. [System Requirements](#system-requirements)
6. [FAQ](#faq)
7. [Authors](#authors)
8. [License](#license)

## About PyGet:

PyGet is a small program in the vein of wget and aria2.
I was unhappy with the usability of these two existing programs
and was faced with needing to write something for my final project
in my beginning programming class. Thus PyGet was born.

I don't expect a ton of people to want to use this, that's okay,
I'm writing it for me :)

PyGet is a fork of [piddle](https://github.com/ArchKaine/piddle)

## Installation:

PyGet requires a few dependencies that are slated to be provided in a 
future release.  You only need to install these dependencies manually if you
are using the current version of PyGet.

Dependencies:
    Python Modules: progressbar 

To install progressbar, use pip2 or your package manager's version into your 
PYTHONPATH.  All other imports are part of the standard Python installation for
most Linux distributions.

Main program installation:

To install PyGet, 'git clone git@github.com:darkredman/pyget.git' in your desired
installation directory (~/git/pyget is recommended).  Ensure that pyget.py is 
executable (as user, chmod +x pyget.py) and then symlink pyget.py to /usr/bin/pyget 
for convenience.  If the last step is not followed, you will have to cd into the folder
containing pyget.py and run './pyget.py' that way. 

## Basic usage:

Defaults:
Most users will find the default behavior of PyGet to be just fine for everyday
use.  Default behavior means prompting via the terminal.  This is the method that 
has seen the most extensive testing.  To run PyGet with the default settings, cd 
into the directory where you have installed PyGet (most likely ~/git/piddle), ensure
that the filename "pyget.py" is executable (as user, chmod +x pyget.py), and execute
./pyget.py.  Follow the prompts and enjoy painless downloading.

## Advanced Usage:

Advanced users and CLI junkies will appreciate PyGet's command line arguments.
They can be found by executing 'pyget.py --help'.  For more help, see pyget.py and scroll
down to the main() function.

## System Requirements:

A current Linux distribution with Python-2.7.2. Older Python versions are
untested and are therefore unsupported.  Python-3.x.x is unsupported at this time
but official support is planned for the near future.

What about Windows and Mac?

PyGet may in fact work on both of these platforms and future support is
intended, but they are untested.  Presumably, Mac systems could work with
PyGet's current code, though this is again, untested.  Windows support is almost
definitely a "no" at this time.


## FAQ

Q: Do you know what "PyGet" means in English!?!?!

A: I'm very well aware thank you.


Q: Knowing what "PyGet" means, why would you name a program like that?

A: Because it was just a "piddly little program" idea that I had.  That, and I 
have a sense of humor about it :)


Q: Download performance is insanely slow, I'm getting roughly 90B/s on a cable connection!

A: I'm very well aware of this and am looking into it.  So far it seems that 
urllib and urllib2 are to blame, but I have yet to find a fix.  This issue is
the highest priority and research into a fix is ongoing.


Q: You know the downloads would go faster if you just used 'X' module...

A: Yep, but then that doesn't solve the problem, does it?  I would rather use
urllib and urllib2 and simply contribute a fix to the community rather than skirt
the real problem and hope that someone else has the time and know-how to do it.
Besides, other methods to accomplish the same tasks as those two modules take a lot
more typing and are not really as elegant and simple to read.


Q: File looping doesn't work with my .csv file containing 'X#' of links! What gives?

A: Currently PyGet can can only take regular text files as arguments.  CSV support
is planned in future versions but is not yet implemented.


Q: Why would I use this instead of Wget or Aria2?

A: Good question! You like Python and want to laugh at a new programmer?


Q: Why doesn't PyGet work on 'X' OS?  You hate on anything that isn't Linux or something?

A: My distaste for Windows aside, I don't "hate" any OS in particular.  If your OS
isn't supported it's because I have yet to add the necessary compatible code.  
Support for Windows and Mac is incoming, but not before all features work perfectly
as intended on the development systems, which all happen to run Linux.


Q: When will that be?

A: "Soon"


Q: You're an idiot programmer because you didn't use 'X' programming language like
a real pro!

A: You're probably right.  However, I see it as me being a new programmer who is
learning and trying to progress.  If that bothers you, don't run the program.  You
probably have a neck-beard, live in your mothers basement, and have problems talking to women.
I on the other hand, have a hot wife, an EPIC BEARD, and have highly progressed social skills. :P


Q: No, seriously, why didn't you write this in C or C++?

A: Short answer, I don't know those programming languages, but they are on my 
"TODO" list.  Longer answer, Python is easy to read, has some powerful libraries
and provides a level of performance that is acceptable for this type of program.


Q: Something is broken! Where can I submit bug reports/feedback/patches/etc?

A: There is no official bug tracker or feedback form to fill out.  If you have feedback
or just want to know who to yell at, email Brian Tomlinson at darthlukan@gmail.com.
If you want to submit patches, please git pull the master branch of PyGet on GitHub
and send me a pull request with a detailed description of what your patch offers.
If it is as good as you say it is (after review) then I'll merge it into master
and credit you in the commit and code.


Q: I want to contribute to your project! What can I do?

A: Assuming that you are talking about code, feedback, testing, etc.  Email 
Brian Tomlinson at darthlukan@gmail.com and we'll go from there.  If in the off-chance 
you are talking about monetary contributions, thank you for your thoughts, but no thanks.
Firstly, while PyGet could very well turn into a larger project that would warrant 
a price tag to the enterprise world, it is still too small for that and honestly, doesn't cost
me any more than I would already be paying in electricity, computers, net, etc.  So save
your cash.  Secondly, because of the first answer, I haven't setup paypal or any other
donation service.  I enjoy coding enough that I'll do it for free for as long as I can.
If you really want to contribute monetarily, hire me to program for your company :)


Q: Where can I keep up to date on PyGet updates without having to check GitHub
everyday?

A: Good question! Right now, the only way to get updates outside of GitHub is
to check my profile on Google Plus: http://goo.gl/DkGtt.  Updates are not on any
kind of a schedule and as such are pretty sporadic.  I am also available via
Google Talk and Google Mail: darthlukan@gmail.com.    


Q: Will PyGet ever have a GUI?

A: Yes! Currently I am looking at a few options and researching which of those 
is easiest to implement cross-platform while maintaining the highest levels of 
stability (despite the OS in certain cases *cough* Windows *cough*).

## Authors

* [DarkRedman](http://www.darkredman.fr/)
    <contact@darkredman.fr>
* [Brian Tomlinson](https://plus.google.com/u/0/109039118030883131674/)
    <darthlukan@gmail.com>
* [Brian Turner](https://plus.google.com/u/0/107589895345000267917/)
    <archkaine@gmail.com>

## License

Check the LICENSE file for the full text version
