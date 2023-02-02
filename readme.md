# FlatBuffers

![Build status](https://github.com/google/flatbuffers/actions/workflows/build.yml/badge.svg?branch=master)
[![BuildKite status](https://badge.buildkite.com/7979d93bc6279aa539971f271253c65d5e8fe2fe43c90bbb25.svg)](https://buildkite.com/bazel/flatbuffers)
[![Fuzzing Status](https://oss-fuzz-build-logs.storage.googleapis.com/badges/flatbuffers.svg)](https://bugs.chromium.org/p/oss-fuzz/issues/list?sort=-opened&can=1&q=proj:flatbuffers)
[![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/google/flatbuffers/badge)](https://api.securityscorecards.dev/projects/github.com/google/flatbuffers)
[![Join the chat at https://gitter.im/google/flatbuffers](https://badges.gitter.im/google/flatbuffers.svg)](https://gitter.im/google/flatbuffers?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
[![Discord Chat](https://img.shields.io/discord/656202785926152206.svg)](https:///discord.gg/6qgKs3R)
[![Twitter Follow](https://img.shields.io/twitter/follow/wvo.svg?style=social)](https://twitter.com/wvo)
[![Twitter Follow](https://img.shields.io/twitter/follow/dbaileychess.svg?style=social)](https://twitter.com/dbaileychess)


**FlatBuffers** is a cross platform serialization library architected for
maximum memory efficiency. It allows you to directly access serialized data without parsing/unpacking it first, while still having great forwards/backwards compatibility.

Go to the [landing page][] to browse the documentation.

## Quickstart

To build on Linux:
```
cmake -G "Unix Makefiles" -DCMAKE_BUILD_TYPE=Release
make
sudo make install
```
Build reference: https://google.github.io/flatbuffers/flatbuffers_guide_building.html

To run the sample:
```
cd samples
./../flatc --python monster.fbs
python3 sample_binary_python3.py
```

Sample output for reference:
```
~/Documents/flatbuffers$ cd samples/
~/Documents/flatbuffers/samples$ ./../flatc --python monster.fbs 
~/Documents/flatbuffers/samples$ python3 sample_binary_python3.py 
buffer: bytearray(b'\x1c\x00\x00\x00\x18\x00 \x00 \x00\x00\x00\x1e\x00\x18\x00\x00\x00\x14\x00\x13\x00\x0c\x00\x0b\x00\x04\x00\x18\x00\x00\x00L\x00\x00\x00\x00\x00\x00\x01 \x00\x00\x00\x00\x00\x00\x00$\x00\x00\x000\x00\x00\x00\x00\x00,\x01\x00\x00\x80?\x00\x00\x00@\x00\x00@@\x02\x00\x00\x004\x00\x00\x00\x1c\x00\x00\x00\n\x00\x00\x00\x00\x01\x02\x03\x04\x05\x06\x07\x08\t\x00\x00\x03\x00\x00\x00Orc\x00\xf4\xff\xff\xff\x00\x00\x05\x00\x18\x00\x00\x00\x08\x00\x0c\x00\x08\x00\x06\x00\x08\x00\x00\x00\x00\x00\x03\x00\x0c\x00\x00\x00\x03\x00\x00\x00Axe\x00\x05\x00\x00\x00Sword\x00\x00\x00')
monster: 150 300 b'Orc' 0
equipped type: 1
monster equipped: ['Bytes', 'Get', 'GetArrayAsNumpy', 'GetSlot', 'GetVOffsetTSlot', 'GetVectorAsNumpy', 'Indirect', 'Offset', 'Pos', 'String', 'Union', 'Vector', 'VectorLen', '__class__', '__delattr__', '__dir__', '__doc__', '__eq__', '__format__', '__ge__', '__getattribute__', '__gt__', '__hash__', '__init__', '__init_subclass__', '__le__', '__lt__', '__module__', '__ne__', '__new__', '__reduce__', '__reduce_ex__', '__repr__', '__setattr__', '__sizeof__', '__slots__', '__str__', '__subclasshook__']
The FlatBuffer was successfully created and verified!
```

## Supported operating systems
* Windows
* macOS
* Linux
* Android
* And any others with a recent C++ compiler (C++ 11 and newer)

## Supported programming languages

Code generation and runtime libraries for many popular languages.

1. C
1. C++ - [snapcraft.io](https://snapcraft.io/flatbuffers)
1. C# - [nuget.org](https://www.nuget.org/packages/Google.FlatBuffers)
1. Dart - [pub.dev](https://pub.dev/packages/flat_buffers)
1. Go - [go.dev](https://pkg.go.dev/github.com/google/flatbuffers/go)
1. Java - [Maven](https://search.maven.org/artifact/com.google.flatbuffers/flatbuffers-java)
1. JavaScript - [NPM](https://www.npmjs.com/package/flatbuffers)
1. Kotlin
1. Lobster
1. Lua
1. PHP
1. Python - [PyPi](https://pypi.org/project/flatbuffers/)
1. Rust - [crates.io](https://crates.io/crates/flatbuffers)
1. Swift - [swiftpackageindex](https://swiftpackageindex.com/google/flatbuffers)
1. TypeScript - [NPM](https://www.npmjs.com/package/flatbuffers)
1. Nim

## Versioning

FlatBuffers does not follow traditional Semver versioning (see [rationale](https://github.com/google/flatbuffers/wiki/Versioning)) but rather uses a format of the date of the release.

## Contribution

* [FlatBuffers Issues Tracker][] to submit an issue.
* [stackoverflow.com][] with [`flatbuffers` tag][] for any questions regarding FlatBuffers.

*To contribute to this project,* see [CONTRIBUTING][].

## Community

* [FlatBuffers Google Group][] to discuss FlatBuffers with other developers and users.
* [Discord Server](https:///discord.gg/6qgKs3R)
* [Gitter](https://gitter.im/google/flatbuffers)


## Security

Please see our [Security Policy](SECURITY.md) for reporting vulnerabilities.

## Licensing
*Flatbuffers* is licensed under the Apache License, Version 2.0. See [LICENSE][] for the full license text.

<br>

   [CONTRIBUTING]: http://github.com/google/flatbuffers/blob/master/CONTRIBUTING.md
   [`flatbuffers` tag]: https://stackoverflow.com/questions/tagged/flatbuffers
   [FlatBuffers Google Group]: https://groups.google.com/forum/#!forum/flatbuffers
   [FlatBuffers Issues Tracker]: http://github.com/google/flatbuffers/issues
   [stackoverflow.com]: http://stackoverflow.com/search?q=flatbuffers
   [landing page]: https://google.github.io/flatbuffers
   [LICENSE]: https://github.com/google/flatbuffers/blob/master/LICENSE.txt
