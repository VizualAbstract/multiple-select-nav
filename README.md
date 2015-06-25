modman "Multiple Select in Layered Navigation"
======
Based on Manadev's freely available Magento extension, "[Multiple Select In Layered Navigation](http://www.manadev.com/advanced-layered-navigation-ce/)". Made into a modman extension, simplyfing its installation and removal.


## Allow Symlinks

  * Web server must follow symlinks
  * For Magento, if using template files in a modman module, you must enable "Allow Symlinks" (found under System > Configuration > Advanced > Developer)
 
![Allow Symlinks](http://host.coreycapetillo.com/git/media/allow-symlinks.png)

## Installation

Make sure you have modman installed. See [https://github.com/colinmollenhour/modman/](https://github.com/colinmollenhour/modman/) for details

```
$ cd /var/www/html				# Wherever Magento is installed
$ modman init					# This is only done once in your application root
$ modman clone git@github.com:VizualAbstract/multiple-select-nav.gitinstalled
```
It's important that you re-index for the plugin to work properly (found under System > Index Management).

If [n98-magerun](https://github.com/netz98/n98-magerun) is installed, all you have to do is run: 

```
$ magerun index:reindex:all
```

## modman
For more information on working with modman modules, see their excellent tutorial at [https://github.com/colinmollenhour/modman/wiki/Tutorial](https://github.com/colinmollenhour/modman/wiki/Tutorial).
