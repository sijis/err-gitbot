err-gitbot a bot that watchs your git repositories (plugin for the XMPP bot err) 
================================================================================

For more information about err you can find it here: https://github.com/gbin/err

**Installation**

This plugin is only Python 2 compatible, pending the port of gitpython.

*dependencies*

    pip install gitpython

If you have the admin rights on an err chatbot simply use
::

    !install err-gitbot

in order to install the plugin.
Then !help to see the available commands and their explanation.

Some tips here :

To track all the branches of a repo just say with the repo url i.e.:
!follow git://github.com/opdenkamp/xbmc.git

Err will extract smartly the name "xbmc" from it.

if you want to follow a specific branches instead of everything just :
!follow git://github.com/opdenkamp/xbmc.git Eden-pvr Dharma

If you redo a follow this time simply with the symbolic name you can add new branches to track :
!git follow xbmc staging

Or you can remove a specific branch with !unfollow :
!git unfollow xbmc staging

Or the repo alltogether
!git unfollow xbmc 

If at any point you are lost, you can ask the list of currently followed repos / branches with :
!git following

Note : If you have several chatrooms defined in your err config, it will only "spam" the first one.

