FROM ubuntu:latest

# Update base packages
RUN export DEBIAN_FRONTEND=noninteractive \
 && apt-get update \
 && apt-get upgrade -y \
 && apt-get install software-properties-common -y \
 && apt-add-repository ppa:git-core/ppa \
 && apt-get update \
 && apt-get install -y \
    git \
    cmake \
    file \
    rpm \
    build-essential \
    libavahi-compat-libdnssd-dev \
    libcurl4-openssl-dev \
    libice-dev \
    libsm-dev \
    libssl-dev \
    libxinerama-dev \
    libxrandr-dev \
    libxtst-dev \
    libxkbcommon-dev \
    libglib2.0-dev \
    ninja-build \
    qtbase5-dev \
    qttools5-dev \
    qttools5-dev-tools \
 && rm -rf /var/lib/apt/lists \
 && git config --system --add safe.directory '*'
