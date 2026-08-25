FROM quay.io/fedora/fedora-toolbox:46

COPY --from=common ./devcontainers  /tmp/common

# Symlinks for host access
RUN /tmp/common/symlinks.sh && \
	rm -rf /tmp/*

# hadolint ignore=DL3041
RUN dnf update && \
	dnf install -y clang gcc mold zsh file dnf-plugins-core \
	&& dnf clean all

