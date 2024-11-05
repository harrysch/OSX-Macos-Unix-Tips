# OSX-Macos-Unix-Tips


## Homebrew
Give me real unix things, give all, give me more!

The Missing Package Manager for macOS (or Linux)
https://brew.sh/


## Tiling Windows
With the new macos 15 you will get "tiling windows" - or use "hammerspoon" https://github.com/Hammerspoon/hammerspoon and "hs.tiling" from https://github.com/dsanson/hs.tiling


---
## OSX, Macos Things:


## Mac-Shell-Script

Double click the script and it will be executed
add ".command" to shell-script
```.command```



### TextEdit, Pages Convert all RTF and RTFD files to Word DOCX via AppleScript

"We do this with Pages because it's the only thing that can correctly convert rtfd. textutil works on rtf files with no text in them but not on rtfd."

https://gist.github.com/dpinney

https://gist.github.com/dpinney/f5de675274c9f1ad16df6794d614dea8

```applescript
set my_paths to {"/path/to/first/file.rtfd", "/path/to/second/file.rtfd"}

repeat with my_path in my_paths
	tell application "Pages"
		set my_file to (my_path as POSIX file)
		set my_name to name of (info for my_file)
		set doc to open my_file
		export doc as Microsoft Word to alias (my_path & ".docx" as POSIX file)
		close doc
		tell application "Finder" to delete my_file
	end tell
end repeat
```

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


## Desktop Automation
Staggeringly powerful macOS desktop automation with Lua 
"hammerspoon" https://github.com/Hammerspoon/hammerspoon






