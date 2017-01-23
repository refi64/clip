clip
====

A simple shell script that wraps xclip and/or xsel in a portable way.

How to install
**************

::

  $ curl https://raw.githubusercontent.com/kirbyfan64/clip/master/clip | sudo bash /dev/stdin -i

Or::

  $ git clone https://github.com/kirbyfan64/clip.git
  $ cd clip
  $ sudo bash clip -i

Examples
********

Copy standard input::

  $ echo stuff | clip

Copy file contents::

  $ clip myfile

Paste to standard output::

  $ clip -o

Paste to file::

  $ clip myfile

Use xsel instead of xclip when possible:

  $ clip -s other_stuff_goes_here
