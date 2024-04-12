FROM debian
ENV FLUTTER_VERSION 3.19.5
RUN apt-get update -y 
RUN apt-get upgrade -y
RUN apt-get install -y curl git unzip xz-utils zip which libglu1-mesa wget
# install android dependency
RUN apt-get install -y clang cmake ninja-build pkg-config libgtk-3-dev liblzma-dev
# install flutter sdk
RUN mkdir /tmp/flutter && wget https://storage.googleapis.com/flutter_infra_release/releases/stable/linux/flutter_linux_${FLUTTER_VERSION}-stable.tar.xz -O /tmp/flutter/flutter-install.tar.xz
RUN tar -xf /tmp/flutter/flutter-install.tar.xz -C /home
ENV PATH="$PATH:/home/flutter/bin"
RUN git config --global --add safe.directory /home/flutter
RUN flutter precache