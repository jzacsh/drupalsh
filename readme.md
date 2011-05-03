## Drupalsh ##

###About###
------------
Shell scripts I use everyday, working with drupal.

All scripts here are fairly simple in function. They mostly wrap popular
drupal scripts/modules (like drush or features).

Usage
------------
Rmff.. I'll write something here soon.

Installation
------------
You basically only need bash and drupal.

These scripts just need to be in your path. eg.: Download these, add them to your path:

    git clone git://github.com/jzacsh/drupalsh ~/drupalsh
    export PATH=~/drupalsh/:$PATH

Most scripts are just wrappers around drush, mysql, innotop, features, etc. I
generally have tried to write sanity-checks to fail my scripts when these
utilties aren't present.

TODO
----
- Make sure that bash4 feature-heavy scripts fail w/o bash4
- Make sure that utility-relying scripts fail w/o those utilities
- sub-shell hell prevents dproj from being a script; see its comments
- Place documentation/examples in here on power of PROJECT_BASE stuff.
- make PROJECT_BASE more powerful by porting it to dynamic scripts that sit in
  this repository ( eg.: commit 8164176 ) .

