# CLibpq

[![Platform][platform-badge]][platform-url]
[![License][mit-badge]][mit-url]
[![Slack][slack-badge]][slack-url]

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

- Generate Xcode project
```bash 
$ swift build -Xcc -I/usr/local/include -Xlinker -L/usr/local/lib/ -Xswiftc -I/usr/local/include -X
```

- Build on Linux
```bash
$ swift build -Xcc -I/usr/include/postgresql
```

## Community

[![Slack][slack-image]][slack-url]

We have an amazing community of open and welcoming developers. Join us on [Slack][slack-url] to get to know us!

## License

All **Zewo** modules are released under the MIT license. See LICENSE for details.

[platform-badge]: https://img.shields.io/badge/Platform-Mac%20%26%20Linux-lightgray.svg?style=flat
[platform-url]: https://swift.org
[mit-badge]: https://img.shields.io/badge/License-MIT-blue.svg?style=flat
[mit-url]: https://tldrlegal.com/license/mit-license
[slack-image]: http://s13.postimg.org/ybwy92ktf/Slack.png
[slack-badge]: https://zewo-slackin.herokuapp.com/badge.svg
[slack-url]: http://slack.zewo.io
