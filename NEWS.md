# News

## version 2.4.9

Released 9 August 2024

This release is built against libmapper version 2.4.9 and liblo version 0.32. It also includes the following improvements:

- The `mpr.in` external now previews arguments to check for the `thru` attribute so that is can be activated before the object is registered with a parent device.
- The instance `overflow` message now has the correct number of arguments (none).
- A fix for inconsistent handler arguments in `oscmulticast`

## Version 2.4.4b

Released 11 October 2023

This release is built against libmapper version 2.4.4. It also includes the following improvements:

- Fix for crash if the `instance` attribute was set on an unconnected `mpr.in` or `mpr.out` object, i.e. if no `mpr.device` object was present in the patcher or (grand)parent patcher.
- Fix for parsing object metadata added using messages rather than object arguments.
- Improvements to help patchers and documentation files.
- The `mpr.in` object now has an attribute `thru` which controls whether input will be echoed to its outlet.
- The `mpr.in` object now accepts a `set` message which will update the signal value without echoing to the object outlet, regardless of whether the `thru` attribute is set to `1`.
- added `.plist` files for macOS externals.

## Version 2.4.4

Released 20 September 2023

This release is built against libmapper version 2.4.4. It also includes the following improvements:

- Improvements to help patchers.
- The `mpr.in` object now echoes its input to its outlet (e.g. when setting the value using a locally-generated update).
- Fix for storing string list properties for `mpr.in` and `mpr.out` objects.

## Version 2.4.1

Released 8 June 2023

This release is built against libmapper version 2.4.1. It also includes scripts for automatically building externals under MacOS and Windows!

## Version 1.2.4

Released 31 January 2020

This version includes better help patch documentation and improved thread protection for avoiding problems in overdrive mode.

## Version 1.2.3

Released 4 September 2018

This version includes fixes for modifying existing maps.

## Version 1.2.2

Released 1 August 2018

This version fixes problems with oscmulticast when the only interface available is lo0 (local loopback).

## Version 1.2.1

Released 23 March 2018

Changes in this version:
– oscmulticast bundle now includes and links to local copy of liblo (universal build)
– some updates to build settings (updated Max API version, etc)

## Version 1.2

Released 17 November 2017

Changes in the version

– XCode projects have been modified to build universal binaries so the max externals will now work in 64bit Max
– some simplification of XCode build settings
