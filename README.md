devlin zed's dotfiles
=====================

This is my dotfiles repository that lets me quickly bootstrap a new Arch Linux
system.  It's expansive and essentially its own Linux distribution, so you're
probably only looking for configuration for a program or two.

![screenshot](https://raw.github.com/devlinzed/dotfiles/master/screenshot.png)

install
=======

Before installing, you should install the relevant packages with `pacman` and
`gem`.  A list of packages and their purpose is below.

    pacman -S artwiz-fonts awesome ctags git gtk-engine-murrine jshon         \
              keychain lua luajit luakit mpc mpd mpv mutt msmtp notmuch pass  \
              ruby rxvt-unicode slock sxiv tmux xautolock xorg-server         \
              xorg-xmodmap xsel zsh
    packer -S compton dmenu-xft-fuzzy isync-git powerpill xcape-git
    gem install gem-ctags bundler

Afterward, check out the repository and run the installation script:

    git clone https://github.com/devlinzed/dotfiles ~/.dotfiles
    cd ~/.dotfiles
    rake

When you're done, `git grep` for `devlin` and change it as necessary.  If you
installed to a different directory, look for `.dotfiles`, too.

what i use
==========

The focal bits are the following.  This repository mainly consists of
configuration and scripts for these programs.

* **email**: [mutt](http://mutt.org/)
* **image viewer**: [sxiv](https://bbs.archlinux.org/viewtopic.php?id=112643)
* **music player**: [mpd](http://mpd.wikia.com/wiki/Music_Player_Daemon_Wiki) and [mpc](http://mpd.wikia.com/wiki/Client:Mpc)
* **shell**: [zsh](http://zsh.org)
* **terminal emulator**: [rxvt-unicode](https://en.wikipedia.org/wiki/Rxvt)
* **terminal multiplexer**: [tmux](http://tmux.sourceforge.net/)
* **text editor**: [vim](http://vim.org)
* **version control**: [git](http://git-scm.org)
* **video player**: [mpv](http://mpv.io/index.html)
* **web browser**: [luakit](http://luakit.org)
* **window manager**: [awesome](http://awesome.naquadah.org/) with
  [compton](https://github.com/chjj/compton)

Some programs or scripts rely on secondary programs.  To properly use
everything in this repository, you'll need to install these as well.

* [dmenu](http://tools.suckless.org/dmenu/) for a top-of-the-screen menu
* [exuberant ctags](http://ctags.sourceforge.net/) for indexing code
* [isync](http://isync.sourceforge.net/) for syncing email
* [keychain](http://www.funtoo.org/wiki/Keychain) for managing agents & passwords
* [msmpt](http://msmtp.sourceforge.net) for sending email
* [notmuch](http://notmuchmail.org/) for indexing and searching email
* [pass](http://zx2c4.com/projects/password-store/) for managing passwords
* [xautolock](http://freecode.com/projects/xautolock) and
  [slock](http://tools.suckless.org/slock) to lock the screen

license
=======

Where I have the right to, I release everything in this repository into the
public domain.  See `UNLICENSE.md` for the full license.
