# OSX-Macos-Unix-Tips


## Homebrew
Give me real unix things, give all, give me more!

The Missing Package Manager for macOS (or Linux)
https://brew.sh/


## Tiling Windows
With the new macos 15 you will get "tiling windows" - or use "hammerspoon" https://github.com/Hammerspoon/hammerspoon and "hs.tiling" from https://github.com/dsanson/hs.tiling


---
## OSX, Macos Things:


### Hidden Files
To show always hidden files in finder.
Terminal:
```defaults write com.apple.finder AppleShowAllFiles true;```

or use the 

#### Bar toggle für hidden files

Press ```Command+Shift+Dot```

### FUSE
macFUSE is a software package for macOS that lets non-privileged users create their own file systems without having to write a single line of kernel code. 
https://github.com/macfuse/macfuse

### Shell-Script

Double click the script and it will be executed
add ".command" to shell-script
```.command```


### Spotlight, mdfind
find files without finder: fff

```
mdfind -name

mdls Datei.txt -name kMDItemFinderComment

mdfind -onlyin /Users/fred/tmp/ -onlyin /Users/fred/tmp2/ searchword

mdfind "searchword searchword2"

# oder ohne
mdfind "berry_tea OR peppermint_tea -chamomile_tea"


# restart
sudo mdutil -E -i on


mdimport -i /Volumes/music/
```


### TextEdit, Pages Convert all RTF and RTFD files to Word DOCX via AppleScript

"We do this with Pages because it's the only thing that can correctly convert rtfd. textutil works on rtf files with no text in them but not on rtfd."

https://gist.github.com/dpinney

https://gist.github.com/dpinney/f5de675274c9f1ad16df6794d614dea8


---

## Apps


Quality crafted apps
https://sindresorhus.com/apps

### Menu Bar Calendar
A monthly calendar, one click away
https://sindresorhus.com/menu-bar-calendar

### Week Number
The current week number in your menu bar 
https://sindresorhus.com/week-number

### Switch default browser easy
I like to have different browsers for different things: one for apple, one for google-things, ... , one for sunday


### Velja
Powerful browser picker
Open links in a specific browser or a matching native app. Easily switch between browsers.
https://sindresorhus.com/velja

or with terminal:

```http://apple.stackexchange.com öffnen -a Firefox.app```

## Desktop Automation
Staggeringly powerful macOS desktop automation with Lua 
"hammerspoon" https://github.com/Hammerspoon/hammerspoon






