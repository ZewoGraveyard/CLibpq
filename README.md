CLibpq
======

[![Swift 3.0](https://img.shields.io/badge/Swift-3.0-orange.svg?style=flat)](https://swift.org)
[![Platforms Linux](https://img.shields.io/badge/Platforms-Linux-lightgray.svg?style=flat)](https://swift.org)
[![License MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=flat)](https://tldrlegal.com/license/mit-license)
[![Slack Status](http://slack.zewo.io/badge.svg)](http://slack.zewo.io)

**CLibpq** provides PostgreSQL for **Swift 3.0**.

## Documentation

- libpq [`documentation`](http://www.postgresql.org/docs/9.1/static/libpq.html)

## Installation

- OSX

```bash
$ brew install postgresql
```

- Linux

```bash
$ apt-get install libpq-dev
```

- Add `CLibpq` to your `Package.swift`

```swift
import PackageDescription

let package = Package(
	dependencies: [
		.Package(url: "https://github.com/Zewo/CLibpq.git", majorVersion: 0, minor: 5)
	]
)

```

- Build on OSX

```bash
$ swift build -Xcc -I/usr/local/include -Xlinker -L/usr/local/lib/
```

- Build on Linux

```bash
$ swift build -Xcc -I/usr/include/postgresql
```

## Community

[![Slack](http://s13.postimg.org/ybwy92ktf/Slack.png)](http://slack.zewo.io)

Join us on [Slack](http://slack.zewo.io).

License
-------

**CLibpq** is released under the MIT license. See LICENSE for details.
