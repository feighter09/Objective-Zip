

Objective-Zip
=============


Introduction
------------

Objective-Zip is a small Objective-C library that wraps ZLib and MiniZip in
an object-oriented friendly way.


What is contained here
----------------------

The source repository contains full sources for ZLib, MiniZip and
Objective-Zip, together with some unit tests. The versions included are:

- 1.2.8 for [ZLib](http://zlib.net).
- 1.1 for [MiniZip](https://github.com/nmoinvaz/minizip).
- latest version for Objective-Zip.

Please note that ZLib and MiniZip are included here only to provide a
complete and self-contained package, but they are copyrighted by their
respective authors and redistributed on respect of their software
license. Please refer to their websites (linked above) for more
informations.


Getting started
---------------

Please see [Getting Started](https://github.com/gianlucabertani/Objective-Zip/blob/master/GETTING_STARTED.md).


License
-------

The library is distributed under the New BSD License.


Version history
---------------

Version 1.0.0:

- Added official podspec to distribute via CocoaPods.
- Added API docs.
- Added nullability annotations.
- Refactored DIY tests as unit tests.
- Added targets for static libraries.
- Added alternative interfaces with NSError pattern in place of exceptions.
- Added support for legacy 32-bit zip files.
- Added class prefix "OZ" to make Objective-Zip a good citizen.
- Fully ARC-ified (removed ARCHelper)
- Some code clean-up.

Version 0.8.3:

- Finally used correctly the 64 bit APIs. Thanks to Nathan Moinvaziri for advicing.
- Updated test code to zip & unzip up to 5 GB.
- Added tests with unzip & check of zip files create with Mac OS X 10.8 and Windows 7.

Version 0.8.2:

- Updated ZLib to 1.2.8
- Updated MiniZip to Nathan Moinvaziri's Version (thanks [Sergio](http://mrsergio.com) for the suggestions)
- Added test code to zip & unzip up to (slighlty less than) 4 GB:
  the library is able to create and expand files up to
  4,293,387,000 bytes (compressed); use the test with caution,
  requires 4 GB of free space and around 10 minutes on the
  iOS simulator

Version 0.8.1:

- Added support for ARC through Nick Lockwood's [ARC Helper](https://gist.github.com/1563325)

Version 0.8:

- Updated ZLib to 1.2.7
- Updated MiniZip to 1.1
- Added method to get file name from a ZipFile instance

Version 0.7.3:

- Fixed memory leak in test app

Version 0.7.2:

- Added variant of writeFileInZipWithName that accepts also a file date
- Fixed bug with date handling

Version 0.7.1:

- Fixed a bug in creation of an encrypted zip file

Version 0.7.0:

- Initial public beta release


Compatibility
-------------

Version 1.0.0 has been tested with iOS up to 8.4.1 and OS X up to 10.10.5, but
should be compatible with earlier versions too, down to iOS 5.1 and OS X 10.7.
Le me know of any issues that should arise.

