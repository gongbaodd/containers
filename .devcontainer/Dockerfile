FROM mcr.microsoft.com/devcontainers/typescript-node:0-18

RUN apt-get update
RUN apt-get install -y \
  curl \
  psmisc

# Install Tarpaulin
# RUN cargo install cargo-tarpaulin

# Install Tauri dependencies
# https://tauri.app/v1/guides/getting-started/prerequisites#setting-up-linux
RUN apt-get install -y \
  libwebkit2gtk-4.0-dev \
  build-essential \
  curl \
  wget \
  libssl-dev \
  libgtk-3-dev \
  libayatana-appindicator3-dev \
  librsvg2-dev

# Install tauri-driver dependencies
RUN apt-get install -y \
  webkit2gtk-4.0-dev \
  webkit2gtk-driver \
  xvfb

# Install tauri-driver
# https://tauri.app/v1/guides/testing/webdriver/introduction#system-dependencies
# RUN cargo install tauri-driver

CMD ["/bin/bash"]