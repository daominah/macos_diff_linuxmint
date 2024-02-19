# Pros and cons of MacOS (MacBook)

This is written by a Linux Mint user, biased but probably true.

### Pros:

* TouchID (__fingerprint to unlock__ screen, limit max 3 fingerprints though).
* __Good built-in display__, high resolution and brightness,
  (but top screen have a notch and resolution value is weird,
  14 inch resolution is 3024x1964, 16 inch resolution is 3456x2234)
* __Good built-in speaker__.
* __Good CPU__. Rarely hear the fan noise from M2 Pro (10 cores: 6×P+ 4×E).
* __Good battery__.
* Remember opening apps after restart.
* Mouse size gets bigger if you are shaking it (help to find it on the display).
* The dock save recently open apps so user can choose to keep them in the dock.

### Cons:

* Macbook has __stupid ports__. It only has USB-C ports, no USB-A (force user to
  buy and bring adapter with the laptop). Macbook Pro 2023 model's ports are too
  close together, I have a problem when plug HDMI and USB on 1 side of the laptop.
  It is still better than some older models that only have 2 USB-C ports, no HDMI,
  what the fuck did they smoked.
* The file explorer __Finder is shit__:
  - No button to create a new file in a directory.
    To create a new file on the Desktop, I have to: open `Finder`: click `Desktop`:
    right click Desktop on `Path Bar`: `Open in Terminal`: `touch new.txt`,
    very easy and intuitive.
  - Need to click 2 tiny buttons to open Terminal from the working directory.
    No hotkey to open Terminal, don't tell me `Cmd Space` to open it with Spotlight.
  - Cannot copy directory path from somewhere else to Finder for opening the path.
    Hard to copy path of the working directory (need to hold `Alt` `RightClick`).
  - Pressing `Enter` will Rename a file, `Enter` should be the main action,
    how often do you want to Rename a file compare to Open it. `Cmd O` is hard to press.
  - Unintuitive way to change default app to open a file type.
    If you set `Always Open With` for a file, it only works for that specific file,
    not for all files with the same extension.
    You have to `RightClick`: `Get Info`: `Open With`: `Change All` (about 10 clicks). 
* __Top Menu Bar is shared between apps__, and always on the top edge of the screen.
  This makes the distance from app window to the menu is far
  (try to use MS Excel without full screen, the menu bar is literally unreachable).
  When you need to work with many apps at the same time, you can get confused
  what app is the Menu Bar pointing to. Another consequence is
  the Menu Bar will disappear if an app is running Full Screen mode,
  they don't think that you can have other apps on other display.
* The dock has __no option to Never Combine Taskbar__ as Windows that show
  all opening windows of the same app with titles, this is unproductive when you
  edit many projects in IDE at the same time.
  (a decent workaround is using `Cmd Backtick` and `Cmd Tab` to switch
  among windows, minimized window will not be switched to with hotkey).
* MacOS has __no default package manager__, have to install [brew](https://brew.sh/)
  or something else. `brew` is so slow compare to Debian `apt`.
* Docker cannot be run in host network mode.
* Missing feature __copy on select, paste on middle mouse__.
* Cannot use **MouseWheel to zoom** in apps
  (default hot key `Cmd +` `Cmd -` is not convenient,
  and installing 3rd party software feels uncomfortable).
* Different __hotkeys__ that are __impossible or hard to be customized__:
  - No hotkey to move active window to other display (others have `Super Shift Arrow`).
    You can set `System settings`: `Keyboard Shortcuts`: `App Shortcuts`: `All Applications`,
    but the hotkeys in many apps do not work.
  - Hotkey `Cmd H` hides the active window, no built-in way to disable this shit.
  - No hotkey for maximize window (LinuxMint `Alt F10` or Windows `Alt Enter`).
  - No hotkey `Home` to go to the beginning of a text line,
    alternatives `Cmd Shift ←` does not work in Terminal, `Alt ←` is slow.
  - Hotkey for Take Screenshot is `Shift Cmd 3`, should be `PrtSc`.
  - Hotkey `Cmd Space` (Spotlight Search), `Ctrl Space` (Change Language Input)
    conflict with Code Completion hotkey in IDE (luckily you can disable).
  - Hotkey for Cut File is unintuitive:`Cmd C` then `Cmd Alt V`.
  - ...

### Cons not bother often:

* Macbook __memory or storage cannot be upgraded__.
  Apple charges $400 for an option to have more 16GB memory or 1TB storage in 2023,
  as expensive as 5 to 10 times normal price.
* __Cannot make password visible__ on the login screen.
  Security your ass, input sources can mess up the tying,
  good luck with finding what wrong in your password.
* No built-in way to keep a window always on top of other windows.
* __Default shell__ is `zsh`, can switch back to `bash` (but very old
  Bash v3.2.57, because newer versions are licensed as GPL3).
* Default zip app (Archive Utility) will extract the file if you click open, so
  you have __no option to just preview zip__ file without extracting it.
* Cannot create directory in root dir `/`, `sudo` does not help.
* Cannot turn off red notification in `System Settings` (e.g. when it wants to upgrade OS).
* `netstat -anv | grep LISTEN` to get process id that is listening on a port,
  but you still need another command to get process name.
* Window min max close buttons on the left and cannot be changed.
* Default mouse scroll direction is inverted
  (need to change `System Settings: Mouse: Natural Scrolling`).

### Tips

* You can swap `Cmd` and `control` key,
  so example press `Cmd C` has the same position as `Ctrl C` on a normal keyboard,
  by changing the setting in `System Settings`: `Customise modifier keys`.
* If you sometimes produce weird symbols while typing (å∫ç ...),
  the reason is you press `option` combine with a character, you can disable this
  by [change setting](https://stackoverflow.com/questions/11876485/how-to-disable-generating-special-characters-when-pressing-the-alta-optiona#comment131744363_41219023)
  Keyboard Input Sources, remove ABC and add Unicode Hex Input.
* If you are Vietnamese, Input Sources Telex is better than Simple Telex.
* If you don't hear your notification sound, e.g. from Slack, check the following:
  - System Settings: Notifications: Application Notifications
  - Focus (Do Not Disturb): can be accidentally turn on by hold `option` key and
    click on the Calendar at the top right of the screen.
