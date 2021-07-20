FROM xbase

RUN sudo pacman -S --noconfirm unzip qt5-base

RUN wget https://sourceforge.net/projects/veroroute/files/VeroRoute_V212_LinuxMint183_64bit.zip/download && unzip ./download && cd ./VeroRoute && sudo ./veroroute-install.sh

CMD ["/usr/bin/veroroute"]
