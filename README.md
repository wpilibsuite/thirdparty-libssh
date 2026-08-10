# thirdparty-libssh

This repo contains the build tools to build [libssh](https://www.libssh2.org) with [aws-lc](https://github.com/aws/aws-lc) as the backend. aws-lc is built with CMake and everything disabled, leaving only the crypto library. libssh2 is built with CMake using the "OpenSSL" backend and manually specifying the aws-lc install path. The two libraries are then merged together to form one static library for distribution.

### Building Instructions

`./gradlew build` will initiate the build for your platform. The built headers, sources, and libraries will be placed in `build/allOutputs`. Note that you **must** use a VS Developer Prompt on Windows.
