# IotaKit

The IOTA Swift API Library

**Please, be careful, it's a work-in-progress project**

- [x] Full support for address generation (with Keccak written in C)
- [x] Basic commands to a full-node
- [x] One-func account retrieval
- [x] Automatic node selector
- [x] Local PoW
- [x] Attach to tangle (0i tx)
- [x] Replay Bundle
- [x] Transfer (>0i tx)
- [x] Promote
- [ ] Multisignature Support

## Compatibility

IotaKit is compatible with all architectures, tested on iOS/MacOS/Ubuntu.

## Dependencies

`Foundation`

`Dispatch`

## Compile

### MacOS

Compile it directly from Xcode project or follow the Ubuntu instructions

### Ubuntu

`cd IotaKit`

`swift build -Xcc -ISources/IotaKit/include/sha3`

## Install

### CocoaPods

pod 'IotaKit', '~> 0.5.5'

## Example

The usage should be straightforward, it is very similar to the [official JS lib](https://github.com/iotaledger/iota.lib.js)

```
let iota = Iota(node: "http://localhost", port: 14265)

iota.nodeInfo({ (result) in
	print(result)
}) { (error) in
	print(error)
}
```

## Author

IotaKit is maintained by [Pasquale Ambrosini](https://pascalbros.github.io)

You can follow me on Twitter at [@PascalAmbro](http://twitter.com/PascalAmbro).


## License
IotaKit is licensed under the terms of the MIT License. Please see the LICENSE file for full details.
