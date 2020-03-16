FROM greyltc/archlinux-aur:latest
RUN pacman -Syu pacman --noconfirm
RUN pacman -Syu --noconfirm --needed base-devel idris clang git libx11
RUN su docker -c 'yay -S --noprogressbar --needed --noconfirm chez-scheme'
