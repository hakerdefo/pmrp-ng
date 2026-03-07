# 📻 PMRP-NG

> The ultimate, lightweight, and resilient terminal internet radio player for Linux and macOS.

**PMRP-NG** is the next-generation successor to the classic `pmrp` script (featured in distros like antiX Linux). After 11 years, PMRP has been completely rewritten from the ground up to utilize modern tools, leaving behind hardcoded stations for a vast, dynamically updated global directory.

## ✨ Features

* **🌍 Infinite Stations:** Powered by the open Radio-Browser API, giving you instant access to over 40,000 global radio stations.
* **⚡ Blistering Fast Interface:** Uses `fzf` and `jq` for instant, fuzzy-searchable, and beautifully aligned columnar menus.
* **🛡️ Resilient Connections:** Automatically shuffles and pings multiple API directory servers on startup, locking onto the fastest available one to ensure the app never breaks if a server goes down.
* **⭐ Star Map (Favorites):** Bookmark stations directly after listening with a single keystroke. Access them instantly from the main menu.
* **🎵 MPV Powered:** Relies on the incredibly stable `mpv` engine for seamless background buffering and playback.

## 🛠️ Installation and Usage

### 1. Install Dependencies
PMRP-NG relies on a few standard, highly optimized terminal utilities. Install them via your package manager:

**Debian/Ubuntu/antiX:**
```bash
sudo apt-get install curl jq mpv fzf bsdmainutils
```
*(Note: `bsdmainutils` provides the `column` command on most Debian-based systems).*

**Arch Linux:**
```bash
sudo pacman -S curl jq mpv fzf util-linux
```

**macOS (Homebrew):**
```bash
brew install curl jq mpv fzf
```

### 2. Installation Methods

Download [pmrp-ng-master] zip, extract its contents and copy the file `pmrp-ng` to `/usr/local/bin` directory:
```sh
sudo cp pmrp-ng /usr/local/bin/
```

Next make it executable,
```sh
sudo chmod 755 /usr/local/bin/pmrp-ng
```

Or use the good ol' git directly:
```sh
git clone https://github.com/hakerdefo/pmrp-ng.git
cd pmrp-ng
sudo cp pmrp-ng /usr/local/bin/
sudo chmod 755 /usr/local/bin/pmrp-ng
```

### 3. Usage

Open terminal, run `pmrp-ng`, select a station according to your mood and don't forget to turn up the volume.

## 🕹️ Controls

Once a station is playing, `mpv` handles the stream. 
* **`q`** or **`Ctrl+C`** : Stop playback and return to the menu.
* **`9`** and **`0`** : Decrease / Increase volume.

## 📜 A Note on Legacy

The original `pmrp` was created over a decade ago, relying on `mpg123` and hardcoded station lists. It holds a proud legacy, serving thousands of users. If you are looking for that classic, ultra-minimal version, [you can find the legacy repository here](https://github.com/hakerdefo/pmrp). This Next-Gen version brings dynamic search and modern API integration while maintaining the lightweight spirit of the original.

## 🙏 Support

If you like **pmrp-ng**, please consider supporting it, even the smallest contribution goes a long way. It is quick & easy via PayPal, Buy Me a Coffee or Liberapay:  

[![Support via PayPal](https://cdn.jsdelivr.net/gh/twolfson/paypal-github-button@1.0.0/dist/button.svg)](https://paypal.me/hakerdefo)  
[!["Buy Me A Coffee"](https://user-images.githubusercontent.com/1376749/120938564-50c59780-c6e1-11eb-814f-22a0399623c5.png)](https://www.buymeacoffee.com/hakerdefo)  
[![Support via Liberapay](https://liberapay.com/assets/widgets/donate.svg)](https://liberapay.com/hakerdefo/donate)  

## 🪪 License

[![Public Domain Mark](http://i.creativecommons.org/p/mark/1.0/88x31.png)](http://creativecommons.org/publicdomain/mark/1.0/)  
This work (<span property="dct:title">pmrp</span>, by [<span property="dct:title">hakerdefo</span>](https://github.com/hakerdefo/pmrp-ng)), identified by [<span property="dct:title">hakerdefo</span>](https://hakerdefo.github.io), is free of known copyright restrictions.

---

*Created with ❤️ and 🎼 by hakerdefo.*

[pmrp--ng-master]:https://github.com/hakerdefo/pmrp-ng/archive/master.zip
