# Builder container to get debian package and extract it
FROM xbase as builder

ARG version=3.4.0

ADD https://mango-lychee.nyc3.cdn.digitaloceanspaces.com/LycheeSlicer-${version}.deb /tmp

RUN cd /tmp && sudo pacman -S --noconfirm binutils && \
	sudo chmod 777 LycheeSlicer-${version}.deb && \
	ar x LycheeSlicer-${version}.deb && \
	sudo tar -xf data.tar.xz && \
	sudo chmod 4755 ./opt/LycheeSlicer/chrome-sandbox

# Final image
FROM xbase

RUN sudo pacman -S --noconfirm nss atk at-spi2-atk gdk-pixbuf2 gtk3

COPY --from=builder /tmp/opt/LycheeSlicer /opt/LycheeSlicer

CMD ["/opt/LycheeSlicer/lycheeslicer", "--no-sandbox"]
