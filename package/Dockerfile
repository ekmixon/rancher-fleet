FROM registry.suse.com/bci/bci-base:15.4.27.11.21
ARG ARCH
ENV ARCH=$ARCH
COPY bin/fleetcontroller-linux-${ARCH} /usr/bin/fleetcontroller
RUN useradd -m -U fleet
USER fleet
CMD ["fleetcontroller"]
