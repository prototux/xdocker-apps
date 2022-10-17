FROM xbase

RUN sudo pacman -S --noconfirm gimp

# XP-Pen driver install
#RUN wget -O driver.tar.gz https://www.xp-pen.com/download/file/id/1936/pid/749/ext/gz.html && tar -xvf driver.tar.gz && cd xp-pen-* && sudo bash ./install.sh && cd .. && sudo rm -rf driver.tar.gz xp-pen*

CMD ["/usr/bin/gimp"]
