FROM xbase

RUN sudo pacman -S --noconfirm base-devel gtk4 pipewire clang rust semver

RUN wget -O pkg.tar.gz https://aur.archlinux.org/cgit/aur.git/snapshot/helvum.tar.gz && tar -xvf pkg.tar.gz && cd helvum && export MAKEFLAGS="-j$(nproc)" && echo "" | makepkg -i

CMD ["/usr/bin/helvum"]
