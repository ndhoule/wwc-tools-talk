# Setting Up JSHint and Sublime Text 2

*Note: These instructions only work for Mac OS X (and maybe Linux).*

1. If you haven't already, download and install [Sublime Text 2](http://www.sublimetext.com/2).
2. Install [Package Control](http://wbond.net/sublime_packages/package_control/installation)
   for Sublime Text 2, which will let you install extensions for Sublime Text.
3. Restart Sublime Text and press `Command + Shift + P`. Type `Install Package`,
   then type `SublimeLinter` and hit `Enter`.
3. Download and install [Node.js](http://nodejs.org/download/) from the official
   website.
4. Open your terminal, paste these commands, and hit enter:

```
sudo npm -g install jshint
export PATH="/usr/local/share/npm/bin:$PATH" >> $HOME/.bash_profile
source $HOME/.bash_profile
```

Restart Sublime Text 2 and you should be set. Enjoy!

## Extra Credit
Open Sublime Text and navigate to the following menu:

```
Sublime Text 2 > Preferences > Package Settings > SublimeLinter > Settings - User`
```

Replace the contents of the opened file with the contents of the
`sublimeLinterSettings.json` file, included in this repository. This will make
your error highlighting a little bit more strict--which is a good thing!
