FROM xbase

RUN sudo pacman -S --noconfirm qt5-base qt5-serialbus qt5-declarative qt5-tools git make gcc

RUN git clone https://github.com/collin80/SavvyCAN.git && cd SavvyCAN && qmake && make -j8

CMD ["./SavvyCAN/SavvyCAN"]
