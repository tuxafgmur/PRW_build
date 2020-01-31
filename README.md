# android_build

Path: build/make


This is the Makefile-based portion of the Android Build System.

This Makefile-based system is in the process of being replaced with [Soong], a
new build system written in Go. During the transition, all of these makefiles
are read by [Kati], and generate a ninja file instead of being executed directly.
That's combined with a ninja file read by Soong so that the build graph of the
two systems can be combined and run as one.

[Kati]:  https://github.com/google/kati
[Soong]: https://android.googlesource.com/platform/build/soong/+/master
