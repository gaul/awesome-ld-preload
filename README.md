# Awesome LD\_PRELOAD

This is a list of resources related to LD\_PRELOAD, a mechanism for changing
application behavior at run-time.  Libraries can override specified functions
with another, for example, making `time(3)` always return 0.  This is often
useful for testing or modifying application behavior without source code
changes.

To use, set the environment variable
`LD_PRELOAD=/full/path/to/your_shared_lib.so` before launching your
application.

LD\_PRELOAD works on Linux systems and some BSDs.  macOS implements similar
functionality via DYLD\_INSERT\_LIBRARIES.

## Libraries

* [angrymlocker](https://github.com/stiletto/angrymlocker) - library for keeping corresponding process in memory
* [arg-inject](https://github.com/jktr/arg-inject) - add support for config files
* [cleancache](https://github.com/kahing/bin/blob/master/cleancache.c) - drop files content from page cache after closing, useful for backups
* [flockit](https://github.com/smerritt/flockit) - add file locking to programs that don't do it
* [ld-preload-open](https://github.com/fritzw/ld-preload-open) - map files or directories to another location
* [libeatmydata](https://github.com/stewartsmith/libeatmydata) - disable all forms of writing data safely to disk. fsync() becomes a no-op, O\_SYNC is removed, etc.
* [libfaketime](https://github.com/wolfcw/libfaketime) - libfaketime modifies the system time for a single application
* [libinput-force-middle-click-emulation](https://github.com/gaul/libinput-force-middle-click-emulation) - force libinput to emulate a middle click when pressing left and right buttons simultaneously
* [libkeepalive](https://github.com/msantos/libkeepalive) - enable TCP keepalive socket options
* [libleakmydata](https://github.com/DavidBuchanan314/libleakmydata) - disable SSL certificate verification
* [libnoxattr](https://github.com/gaul/libnoxattr) - disable all forms of extended attribute access
* [openssl-hook](https://github.com/sebcat/openssl-hook) - log data to/from SSL\_write/SSL\_read to disk
* [otherport](https://github.com/FiloSottile/otherport) - redirect connections to other ports
* [timeskew](https://github.com/vi/timeskew) - override time reporting in Linux processes (accelerate/slowdown games, test code involving timers/delays)
* [unrandom](https://github.com/whitequark/unrandom) - make `srand()` always use the seed 0
* [lkl](https://github.com/lkl/linux#lkl-hijack-library) use mordern Linux kernel on old Centos5/6 (2.6 kernel) machines.

## Meta

* [GitHub ld-preload tag](https://github.com/topics/ld-preload)
* [StackOverflow ld-preload tag](https://stackoverflow.com/questions/tagged/ld-preload)

## Links

* [LD\_PRELOAD is super fun. And easy!](https://jvns.ca/blog/2014/11/27/ld-preload-is-super-fun-and-easy/) (Julia Evans)
* [LD\_PRELOAD: The Hero We Need and Deserve](https://blog.jessfraz.com/post/ld_preload/) (Jessie Frazelle)

## License

Copyright (C) 2020 Google LLC

Licensed under the Creative Commons Attribution License, Version 4.0
