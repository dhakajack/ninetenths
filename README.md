# ninetenths
Nine-Tenths of the Law (interactive fiction)

What is this?
-------------

This is the source code to "Ninetenths of the Law", an interactive fiction game
(or more commonly known as "text adventure".)  It was originally
written by Jack Welch in 2008 as an entry in that year's IntroComp.

The code is released under the "Creative Commons Attribution -
Noncommercial - Share Alike 3.0" license, which you can find in the
LICENSE file.

The game is written in the Inform 6 programming language, but has most
recently been compiled under the Inform7 IDE version 6M62, which still
supports Inform 6.

You can download the compiler and IDE as a single
package from http://www.inform7.com

When compiled, the source code produces a bytecode file which can be
executed on any implementation of the Z virtual machine:

https://en.wikipedia.org/wiki/Z-machine

The game's source code is in the main.inf file, but also includes
auxiliary code from the menus.h file. The uuid.txt is a unique 
identifier that allows this game to be indexed in interactive
fiction databases like ifdb 

http://ifdb.tads.org/viewgame?version=2&id=8ithpr6yhbhhb6fe


To build the game:
------------------

1. Create a working Inform project from your source tree:

  $ git clone URL NineTenths
  $ cd NineTenths
  $ mv Ninetenths.inform/ temp.inform/

  [...launch Inform, create new project in this dir called 'NineTenths'…]

  $ cp temp.inform/Source/story.ni Ninetenths.inform/Source/
  $ cp temp.inform/uuid.txt Ninetenths.inform/
  $ rm -rf temp.inform/

2. Launch the Inform IDE and load the Ninetenths.inform project.  The
source code should be visible, and it should compile fine.  [Make sure
that Inform's settings are are set to "Z5" as the target VM.]


WARNING!!
  ********************************************************************
  ** DO NOT do any version control operations (commit, push,
  ** and particularly, pull, update, and merge) while the Inform IDE 
  ** is still open.  When the IDE 'saves', it destroys and recreates 
  ** the whole pogoman-go.inform/ directory, thus possibly eradicating
  ** and changes you may have downloaded. 
  ********************************************************************
