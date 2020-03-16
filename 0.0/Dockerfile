FROM zenten/archlinux-aur:latest
RUN pacman -Syu --noconfirm --needed idris clang libx11
RUN su docker -c 'yay -S --noprogressbar --needed --noconfirm chez-scheme'
