FROM xbase

RUN sudo pacman -S --noconfirm base-devel qt5-base qt5-svg qt5-quickcontrols2 sdl2_ttf ffmpeg intel-media-driver git libva

RUN wget -O pkg.tar.gz https://aur.archlinux.org/cgit/aur.git/snapshot/moonlight-qt.tar.gz && tar -xvf pkg.tar.gz && cd moonlight-qt && export MAKEFLAGS="-j8" && echo "" | makepkg -i

CMD ["/usr/bin/moonlight"]
