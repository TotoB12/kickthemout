# KickThemOut

> [KickThemOut](https://github.com/totob12/kickthemout/) - **Kick Devices Off Your Network**

A tool to kick devices out of your network and enjoy all the bandwidth for yourself.
It allows you to select specific or all devices and ARP spoofs them off your local area network.

- Compatible with Python **3+** 🎉.

- *Not* compatible with Windows.

Author: [TotoB12](mailto:totob12github@gmail.com).
    
-------------

# Installation

## Debian Installation

You can download KickThemOut by cloning the [Git Repo](https://nikolaskama.me/kickthemoutproject) and simply installing its requirements:

```
~ ❯❯❯ sudo apt-get update && sudo apt-get install nmap

~ ❯❯❯ git clone https://github.com/totob12/kickthemout.git

~ ❯❯❯ cd kickthemout/

~/kickthemout ❯❯❯ sudo -H pip3 install -r requirements.txt

~/kickthemout ❯❯❯ sudo python3 kickthemout.py
```


## MacOS Installation

If you would like to install KickThemOut on a Mac, please run the following:

```
~ ❯❯❯ brew install libdnet nmap

~ ❯❯❯ git clone https://github.com/totob12/kickthemout.git

~ ❯❯❯ cd kickthemout/

~/kickthemout ❯❯❯ sudo -H pip3 install -r requirements.txt

~/kickthemout ❯❯❯ sudo python3 kickthemout.py
```

**NOTE**: You need to have [Homebrew](http://brew.sh/) installed before running the Mac OS installation. 

Also, **keep in mind** that you might be asked to run some extra commands after executing the pip requirement installation.


## ArchLinux Installation

You can download KickThemOut on an Arch based system by executing the following:

```
~ ❯❯❯ git clone https://github.com/totob12/kickthemout.git

~ ❯❯❯ cd kickthemout/

~/kickthemout ❯❯❯ sudo -H pip3 install -r requirements.txt

~/kickthemout ❯❯❯ sudo python3 kickthemout.py
```

<br/>

# Usage

```
Usage: sudo python3 kickthemout.py [options]

Options:
  --version             show program's version number and exit
  -h, --help            show this help message and exit
  -p PACKETS, --packets=PACKETS
                        number of packets broadcasted per minute (default: 6)
  -s, --scan            perform a quick network scan and exit
  -t TARGETS, --target=TARGETS
                        specify target IP address(es) and perform attack

Examples:
  sudo python3 kickthemout.py --target 192.168.1.10 
  sudo python3 kickthemout.py -t 192.168.1.5,192.168.1.10 -p 30
  sudo python3 kickthemout.py (interactive mode)
```

To view all available options run:

```
~/kickthemout ❯❯❯ sudo python3 kickthemout.py -h
```
