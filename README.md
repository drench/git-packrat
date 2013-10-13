git packrat
===========

Do you like branches? Even the ones that went nowhere?

If you hate seeing your `git branch` output cluttered with dead
branches, yet can't bring yourself to just throwing that
never-to-be-merged code away, `git packrat` may be for you.

Usage
-----

To move a branch into the 'attic':

    % git packrat some-dead-branch

This creates an `attic` bare repo in a parallel directory,
`push`es the branch to it, and finally deletes the
local branch.

If you ever need to get it back (unlikely), just check it out
as you would any remote branch:

    % git checkout attic/some-dead-branch

Installation
------------

If you use homebrew:

    % brew tap drench/moregit
    % brew install git-packrat

Otherwise, just put `git-packrat` somewhere in your `$PATH`. May I suggest `~/bin/`?

License
-------

MIT-style
