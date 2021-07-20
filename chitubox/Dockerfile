FROM xbase

RUN sudo pacman -S --noconfirm xcb-util xcb-util-cursor xcb-util-keysyms xcb-util-renderutil xcb-util-wm

ENV LD_LIBRARY_PATH="/app/chitubox/lib:${PATH}"
ENV QT_QPA_PLATFORM_PLUGIN_PATH="/app/chitubox/plugins"

ARG VERSION="1.8.1"

COPY chitubox_v1.8.1.tar.gz /app/
RUN cd /app/ && sudo tar -xvf chitubox_v${VERSION}.tar.gz && sudo mv "CHITUBOX V${VERSION}" chitubox

WORKDIR /app/chitubox/
CMD ["/app/chitubox/CHITUBOX"]
