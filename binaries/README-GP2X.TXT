Simon Tatham's Portable Puzzle Collection - Port to GP2X/SDL
============================================================
                         by Ledow

This is an unofficial port of the puzzles from Simon 
Tatham's Portable Puzzle Collection to the GP2X.  Please 
don't bother Simon Tatham himself with issues about this 
port.

The Puzzle Collection is a set of (currently) 27 puzzle
and logic games.  They are based on a portable framework
which means that new games instantly run on all platforms.

This port was not a simple task as the original collection
only had support for GTK, MacOS, Palm and Windows.  It
had to be laboriously converted to SDL before it was able 
to run on the GP2X.

The port author is ledow, whose website is available at:

 http://www.ledow.org.uk/
 http://www.ledow.org.uk/gp2x

Parts of the software were made by other people (e.g. 
the games were made by Simon Tatham, the menu by juanvvc).
See the various LICENCE files for details.

Installation
============

Make sure you extract the zip file with full directories.
You should get a folder "STPPC2x" with a subdirectory
"games" (you may also get a "source" directory if you have
downloaded the source-code too).

Copy the entire STPPC2x folder (you may omit the "source"
folder if you want) to your GP2X.  On the GP2X, navigate
to the folder STPPC2x and either run the menu or go into
"games" and run the individual game of your choice.

If you are using GMenu2x, I suggest you use the games 
inside the "games" folder (the ones without the .gpe 
extension) as these do not try to return to the GP2X's
default menu.  The .gpe's in there are just wrapper 
scripts.

Controls
========

The joystick controls the mouse cursor.  

[F-200 users may be lucky enough to have touchscreen 
controlling the mouse too but I have no way to test that.  
Chances are that you can only left-click, though.]

In-game:

- A, Y and B work as left, middle and right mouse buttons.
- L & R are used for selecting numbers.
- X inserts the currently selected number.
- Vol+ and Vol- at the same time solves the puzzle.
- Start brings up the menu to let you pause, restart, 
  quit, configure and start new games.
- Select restarts the current game.
- L and R at the same time quits the game.

In-game menu:

- X saves the current configuration as default
- L & R are used for selected save slots
- Select saves the current game to a save slot
- Vol+ and Vol- at the same time loads the game from a slot

For gameplay information or the use of the mouse buttons in 
the individual puzzles see PUZZLES_QUICKSTART.TXT.  There is
also PUZZLES.TXT which goes into more detail but this file is
written with desktop use in mind and includes references to 
lots of irrelevant features).

Development information
=======================

The original license and copyright for the puzzles and 
sourcecode can be found in LICENCE.SimonTatham. My 
contributions are under the GPLv2, found in 
LICENCE.GPL.  

This port also uses the following software:

Deja Vu Fonts - LICENCE.DejaVuFonts
SDL_gfx - LICENCE.SDL_gfx
SDL_ttf - LICENCE.SDL_ttf
SDL - LICENCE.SDL
Freetype - LICENCE.Freetype
INIParser - LICENCE.INIParser
Paeryn's accelerated SDL Library (although it runs just
as well under Open2x SDL libraries)
juanvvc's menu - LICENCE.GUI
FastEvents - LICENCE.FastEvents

The original GTK/Windows/MacOS/Palm puzzle collection is 
available (with source code) here:

 http://www.chiark.greenend.org.uk/~sgtatham/puzzles/

This GP2X port is primarily based on SVN version r7977 from:

 http://svn.tartarus.org/puzzles/
 svn://svn.tartarus.org/puzzles/

Complete source code for this modified version can be found
in the /source directory.  This file can be obtained from 
the website if you haven't already got it:

 http://www.ledow.org.uk/gp2x/

This port is in two parts - first it had to have an SDL 
frontend added to the GTK/MacOS/Windows frontends.  Then
it had to be edited, customised and cross-compiled for the 
GP2X, including screen drawing routines, mapping the 
joystick to a mouse and providing numerical input.

There should be no dependancies other than libraries already
present in firmware 3.0 or above (in fact, probably not even
that because the games are statically linked with the 
libraries that they need).  For more technical information, 
see the source code.

The collection was ported with the aid of:

The Open2x toolchain
The Open2x libraries
The Deja Vu fonts
The "pico" text editor (I kid you not)
A brain that hadn't programmed in C for years.

Primary testers were:

Me.
My wife.
(she won the bug-finding contest between the two of us)

I hope you enjoy the puzzles.  If you get stuck on them,
I'll be absolutely no use to you.

- Ledow
http://www.ledow.org.uk/gp2x/
