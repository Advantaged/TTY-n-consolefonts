# TTY-n-consolefonts

## Set bigger "TTY-Fonts", "consolefonts" 

* **Scope of Work:** Setup bigger fonts for TTY.
* **Merit to:** [Linux Mench](https://www.youtube.com/watch?v=75TzZj81yaQ&ab_channel=LinuxMench), [byte & thisoldman](https://bbs.archlinux.org/viewtopic.php?id=82240) ➕ [Archlinux-Wiki-console](https://wiki.archlinux.org/title/Linux_console).
* This work is tailored to Archlinux-like OS but apply to every other Linux too.
* Motivation: By switching to TTY or during boot you have to small fonts & hence cannot read it at all and/or to small for your display/monitor.


### Prerequisite

* Assure you can use `sudo` for installing programs and/or modify system-files
* Assure at least one of the following editors is installed: `nano`, `neovim`, `vim` or `kate`. 

### Step 1. install your preferred Font/Font-Family

1. Install font-s:

```
sudo pacman -Syy --needed --noconfirm terminus-font
```

* **Note:** This is my preferred font, is not installed by default & available on each distribution (Distro).

2. TTY- and/or `consolefonts`-location:

`cd /usr/share/kbd/consolefonts/`

### Step 2. Configure/Setup your preferred Font

1. Permanently Setup:

* Edit configuration file:

```
sudo nano /etc/vconsole.conf
```

* Add or modify your preferred font, add in case anew line:

```
FONT=ter-132b
```

* **Note-s:**
    * This is the largest & bold font of this "family".
    * Remember❗️ let an empty line at end of each Linux-configuration-file
    * If the configuration-file not yet exist… create one.
    * See my configuration below:

```
KEYMAP=us-acentos

FONT=ter-132b

```


✅  **Done** 👍 **and Enjoy** ❗️ 
