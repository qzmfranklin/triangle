# These binaries can be built on a Ubuntu 18.04.2 amd64 machine with the vanilla
# GCC 7.4.0 toolchain.  No special configuration is needed to get things done.
#
# However, it might be a little hassle to make it build with clang, especially
# with the C++11 abi breakage.

cc_binary(
    name = 'triangle',
    srcs = [
        'triangle.c',
        'triangle.h',
    ],
)

cc_binary(
    name = 'showme',
    srcs = ['showme.c'],
    linkopts = [
        # Requires the X11 library.
        '-lX11',
        '-L/usr/include/X11',
    ],
)

