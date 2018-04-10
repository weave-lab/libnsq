[![pipeline status](https://gitlab.getweave.com/weave-lab/comm/libnsq/badges/master/pipeline.svg)](https://gitlab.getweave.com/weave-lab/comm/libnsq/commits/master)
[![coverage report](https://gitlab.getweave.com/weave-lab/comm/libnsq/badges/master/coverage.svg)](https://gitlab.getweave.com/weave-lab/comm/libnsq/commits/master)

## Installation
```bash
go get weavelab.xyz/libnsq
```

For more information on `weavelab.xyz`, see the projects [readme](https://gitlab.getweave.com/weave-lab/ops/xyz/blob/master/README.md).

## libnsq

async C client library for [NSQ][1]

### Status

This is currently pretty low-level, but functional.  The raw building blocks for communicating
asynchronously via the NSQ TCP protocol are in place as well as a basic "reader" abstraction that facilitates
subscribing and receiving messages via callback.

TODO:

 * maintaining `RDY` count automatically
 * feature negotiation
 * better abstractions for responding to messages in your handlers

### Dependencies

 * [libev][2]
 * [libevbuffsock][3]

[1]: https://github.com/bitly/nsq
[2]: http://software.schmorp.de/pkg/libev
[3]: https://github.com/mreiferson/libevbuffsock
