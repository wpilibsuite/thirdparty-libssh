# thirdparty-libssh

This repo contains the build tools to build [libssh](https://www.libssh.org) with [OpenSSL](https://www.openssl.org) as the backend. OpenSSL is built by first configuring with `perl Configure no-shared` to build a static library. LibSSH is built with CMake. The two libraries are then merged together to form one static library for distribution.

### Building Instructions

`./gradlew build` will initiate the build for your platform. The built headers, sources, and libraries will be placed in `build/allOutputs`. Note that you **must** use a VS Developer Prompt on Windows.