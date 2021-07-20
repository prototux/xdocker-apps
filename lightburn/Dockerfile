FROM xbase

RUN sudo pacman --noconfirm -S nss gtk2

ARG LB_VERSION=0.9.24

RUN wget https://github.com/LightBurnSoftware/deployment/releases/download/$LB_VERSION/LightBurn-Linux64-v$LB_VERSION.run && chmod +x LightBurn-Linux64-v$LB_VERSION.run && ./LightBurn-Linux64-v$LB_VERSION.run && rm LightBurn-Linux64-v$LB_VERSION.run

CMD ["/home/jason/.local/share/LightBurn/LightBurn"]
