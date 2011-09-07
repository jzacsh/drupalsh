## Drupalsh ##

###About###
------------
Tiny [bash](http://www.gnu.org/software/bash/manual/bashref.html) shell scripts and [functions](http://www.gnu.org/software/bash/manual/bashref.html#Shell-Functions) for working with drupal. Typically a function is something you can only run when sourced (eg.: in your login shell), while scripts can be run even without an interactive shell.

All utilities here are fairly simple in function. They're mostly wrappers around other popular
drupal utilities like [drush](http://drupal.org/project/drush) and [features](http://drupal.org/project/features).

Usage
------------
Usage statements for most scripts and functions can found by passing `-h` or
`--help`. Often times, especially for short functions, there's no point in
writing a usage print-out; its easier to just `type [function-name]` in your
shell.

Installation
------------
You basically only need bash and usually drupal.

These scripts just need to be in your [PATH](http://en.wikipedia.org/wiki/Path_(variable\)) [env. variable](http://en.wikipedia.org/wiki/Environment_variable). eg.: Download this repo and add it to your path:

    git clone git://github.com/jzacsh/drupalsh ~/drupalsh
    export PATH=~/drupalsh/:$PATH

Most scripts are just wrappers around drush, mysql, innotop, features, etc. I
generally have tried to write sanity-checks to fail my scripts when these
utilties aren't present.

The bash functions in ./drupalsh can be [source](http://www.gnu.org/software/bash/manual/bashref.html#Bourne-Shell-Builtins)d to make them available, eg. placing this in your ~/.bashrc:

    source drupalsh

TODO
----
- Make sure that bash4 feature-heavy scripts fail w/o bash4
- Make sure that utility-relying scripts fail w/o those utilities
- Place documentation/examples in here on power of PROJECT_BASE stuff.
- make PROJECT_BASE more powerful by porting it to dynamic scripts that sit in
  this repository ( eg.: commit 8164176 ) .
