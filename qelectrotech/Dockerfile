FROM xbase

RUN sudo pacman -S --noconfirm base-devel qt5-svg desktop-file-utils hicolor-icon-theme kcoreaddons kwidgetsaddons tk git

RUN git clone https://aur.archlinux.org/qelectrotech.git && cd qelectrotech && makepkg --noconfirm -i

CMD ["/usr/bin/qelectrotech"]
