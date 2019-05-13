
# Go cross compiler (xgo): Go 1.12.x
# Copyright (c) 2019 Péter Szilágyi. All rights reserved.
#
# Released under the MIT license.

FROM karalabe/xgo-1.12

MAINTAINER Soopsio <admin@soops.io>

# Configure the root Go distribution and bootstrap based on it
ENV GO_VERSION 1125

RUN \
  export ROOT_DIST=https://storage.googleapis.com/golang/go1.12.5.linux-amd64.tar.gz      && \
  export ROOT_DIST_SHA=aea86e3c73495f205929cfebba0d63f1382c8ac59be081b6351681415f4063cf && \
  \
$BOOTSTRAP_PURE

RUN apt-get -y install libpam-dev
