    pacman -S artwiz-fonts awesome ctags git gtk-engine-murrine jshon         \
              keychain lua luajit luakit mpc mpd mpv mutt msmtp notmuch pass  \
              ruby rxvt-unicode slock sxiv tmux xautolock xorg-server         \
              xorg-xmodmap xsel zsh
    packer -S compton dmenu-xft-fuzzy isync-git powerpill xcape-git
    gem install gem-ctags bundler

    git clone https://github.com/cyanideoverdose/dotfiles ~/.dotfiles
    cd ~/.dotfiles
    rake


