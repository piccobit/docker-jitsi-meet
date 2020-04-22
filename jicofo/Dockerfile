ARG JITSI_REPO=quay.io/piccobit
FROM ${JITSI_REPO}/jitsi-base-java:base-java-0.1.0

RUN \
	apt-dpkg-wrap apt-get update && \
	apt-dpkg-wrap apt-get install -y jicofo && \
	apt-cleanup

COPY rootfs/ /

VOLUME /config

