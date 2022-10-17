FROM xbase

RUN printf "[multilib]\nInclude = /etc/pacman.d/mirrorlist" | sudo tee -a /etc/pacman.conf && \
	cat /etc/pacman.conf && \
	sudo pacman -Sy && sudo pacman -S --noconfirm steam

CMD ["/usr/bin/steam"]
