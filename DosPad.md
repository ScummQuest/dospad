**This page is intended for developers**

# Introduction #

DOSPAD is based on dosbox (current version 0.74), and SDL 1.3 (still in development).  Dosbox uses SDL 1.2 at the time of writing, so a major part in dosbox changes are adopting to SDL 1.3 interfaces.  To boost performance, SDL 1.3 is modified to suit our needs.

# Development Convention #

All changes in dosbox and SDL are marked by IPHONEOS macros.  You're encouraged to do so as well so life will be a lot easier when we are going to port new dosbox/SDL changes. And we should keep the modification as simple as possible.

To simplify build process, we only support building from xcode, that means, we are throwing away configure scripts. To configure dosbox components, you will need to modify config.h inside dosbox.

Zero warning tolerance. Use the default build settings in xcode, a clean build should not generate warnings.