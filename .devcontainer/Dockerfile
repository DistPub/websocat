FROM rust:1.63.0-alpine3.15 as build
ENV RUSTFLAGS='-Clink-arg=-s -Ctarget-feature=+crt-static'

# env prepare
RUN apk add --no-cache git musl-dev pkgconfig openssl-dev openssl-libs-static
ENV OPENSSL_STATIC=1
ENV OPENSSL_LIB_DIR=/usr/lib
ENV OPENSSL_INCLUDE_DIR=/usr/include/openssl
