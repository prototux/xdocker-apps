FROM xbase

RUN sudo pacman-key --init && \
    curl -O https://download.sublimetext.com/sublimehq-pub.gpg && sudo pacman-key --add sublimehq-pub.gpg && sudo pacman-key --lsign-key 8A8F901A && rm sublimehq-pub.gpg && \
    echo -e "\n[sublime-text]\nServer = https://download.sublimetext.com/arch/stable/x86_64" | sudo tee -a /etc/pacman.conf && sudo pacman -Sy --noconfirm sublime-text

COPY start.sh /usr/bin/sublime

CMD ["bash", "/usr/bin/sublime"]
