FROM xbase

RUN sudo pacman --noconfirm -S intel-media-driver libvdpau-va-gl libxcb xcb-util libxkbcommon-x11 xcb-util-cursor xcb-util-keysyms xcb-util-renderutil xcb-util-wm xcb-util-errors xcb-util-xrm

ADD https://repository.drovio.com/stable/drovio/linux/latest_version/drovio.pkg.tar.xz /tmp/drovio.pkg.tar.xz
RUN sudo pacman --noconfirm -U /tmp/drovio.pkg.tar.xz

CMD ["/opt/drovio/drovio-core"]
