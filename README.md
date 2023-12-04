# Pros and cons of MacOS (MacBook)

This is written by a Linux Mint user, biased but probably true.

### Pros:

* TouchID (**fingerprint to unlock** screen, limit max 3 fingerprints though).
* Having a **good built-in display**, high resolution and brightness,
  (but top screen have a notch and resolution value is weird,
  14 inch resolution is 3024x1964, 16 inch resolution is 3456x2234)
* Having a **good built-in speaker**.
* Remember opening apps after restart.
* Mouse size gets bigger if you are shaking it (help to find it on the display).
* The dock save recently open apps so user can choose to keep them in the dock.

### Cons:

* Macbook has **stupid ports**. It only has USB-C ports, no USB-A (force user to
  buy and bring adapter with the laptop). Macbook Pro 2023 model's ports are too
  close together, I have a problem when plug HDMI and USB on 1 side of the laptop.
  It is still better than some older models that only have 2 USB-C ports,
  no HDMI, what the fuck did they smoked.
* The file explorer **Finder is shit**. No button to create a new
  text file in the working directory. Need to click 2 tiny buttons to
  open Terminal from the working directory. Cannot copy directory path from
  somewhere else to Finder for opening the path. Hard to copy path of the
  working directory (need to hold `Alt` `RightClick`). Pressing `Enter` will
  Rename a file, `Enter` should be the main action, how often you want to Rename
  a file compare to Open it.
* **Top Menu Bar is shared between apps**, and always on the top edge of the
  screen. This makes the distance from app window to the menu is far.
  When you need to work with many apps at the same time, you can get
  confused what app is the Menu Bar pointing to. Another consequence is
  the Menu Bar will disappear if an app is running Full Screen mode,
  they don't think that you can have other apps on other display.
* The dock has **no option to Never Combine Taskbar** as Windows that show
  all opening windows of the same app with titles, this is unproductive when you
  edit many projects in IDE at the same time.
  (a decent workaround is using `Cmd Backtick` and `Cmd Tab` to switch
  among windows, minimized window will not be switched to with hotkey).
* MacOS has **no default package manager**, have to install [brew](https://brew.sh/)
  or something else. `brew` is so slow compare to Debian `apt`.
* Default Vietnamese input Simple Telex **cannot fast type "ươ"** by press `][`.
* Hard to **change default app** to open a file type. Example I did choose to
  open `.xlsx` file with LibreOffice and remove Microsoft Excel in Applications 
  dir, somehow Microsoft Excel is always reinstalled and set as default app to
  open `.xlsx`. This is a fucking virus behavior.
* Missing feature **copy on select, paste on middle mouse**.
* Different **hotkeys** that are **impossible or hard to be customized**:
  - No hotkey `Home` to go to the beginning of a text line, alternatives
    `Cmd Shift ←` does not work in Terminal, `Alt ←` is slow.
  - No hotkey to open Terminal.
  - No hotkey for maximize window (LinuxMint `Alt F10` or Windows `Alt Enter`)
  - No hotkey to move active window to other display(others have `Super Shift Arrow`).
  - Cannot `Ctrl MouseWheel` to zoom in many apps (`Cmd +` or `Cmd -` is not convenient).
  - Hotkey for Take Screenshot is `Shift Cmd 3`, should be `PrtSc`.
  - Hotkey `Cmd H` hides the active window, no built-in way to disable this shit.
  - Hotkey `Cmd Space` (Spotlight Search), `Ctrl Space` (Change Language Input)
    conflict with Code Completion hotkey in IDE (luckily you can disable)
  - Hotkey `F5` or `Cmd F5` opens voice things.
    (hotkey for Refresh is `Cmd R` or `Cmd Shift R`.)
  - Hotkey for Open File is `Cmd O`, should be `Enter`.
  - Hotkey for Rename is `Enter`, should be `F2`.
  - Hotkey for Cut File is unintuitive:`Cmd C` then `Cmd Alt V`
  - ...

### Cons not bother often:

* Macbook **memory or storage cannot be upgraded**. Apple charges $400 for an
  option to have more 16GB memory or 1TB storage in 2023, as expensive
  as 5 to 10 times normal price.
* **Default shell** is `zsh`, can switch back to `bash` (but very old
  Bash v3.2.57, because newer versions are licensed as GPL3).
* Default zip app (Archive Utility) will extract the file if you click open, so
  you have **no option to just preview zip** file without extracting it.
* Cannot create directory in root dir `/`, `sudo` does not help.
* Cannot turn off red notification in `System Settings` (when it wants to upgrade OS).
* `netstat -anv | grep LISTEN` to get process id that is listening on a
  port, but you still need another command to get process name.
* Window min max close buttons on the left and cannot be changed.
* Default mouse scroll direction is inverted (need to change
  `System Settings: Mouse: Natural Scrolling`)
