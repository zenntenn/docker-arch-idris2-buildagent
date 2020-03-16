FROM archlinux:latest

RUN pacman -Syu --noconfirm --needed base-devel idris clang

RUN mkdir /home/build && chgrp nobody /home/build && chmod g+ws /home/build && setfacl -m u::rwx,g::rwx /home/build && setfacl -d --set u::rwx,g::rwx,o::- /home/build

RUN cd /home/build && sudo -u nobody git clone https://aur.archlinux.org/chez-scheme.git && cd chez-scheme && sudo -u nobody -si --noconfirm --needed
