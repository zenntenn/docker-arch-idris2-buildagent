FROM archlinux:latest

RUN pacman -Syu --noconfirm --needed base-devel idris clang git libx11

RUN mkdir /home/build
RUN chgrp nobody /home/build
RUN chmod g+ws /home/build
RUN setfacl -m u::rwx,g::rwx /home/build
RUN setfacl -d --set u::rwx,g::rwx,o::- /home/build

RUN cd /home/build && sudo -u nobody git clone https://aur.archlinux.org/chez-scheme.git && cd chez-scheme && sudo -u nobody makepkg -si --noconfirm --needed
