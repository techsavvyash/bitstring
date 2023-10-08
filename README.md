# Bitstring
This bitstring module is a hacky tweak to make the [original bitstring package](https://github.com/digitalbazaar/bitstring) play nice with typescript.

## Install

To install get the latest version from NPM:

```
npm install @sunbird-rc/bitstring
```

To install locally for development:

```
git clone https://github.com/techsavvyash/bitstring.git
cd bitstring
npm install
```

## API

### set(position, on)
Sets the value of a bit for the given position to the given boolean.
```js
bitstring.set(1, true);
```

### get(position)
Gets the value of a bit for the given position.
```js
bitstring.get(3);
```

### encodeBits()
Compresses and encodes bits to a base64url encoded string.

```js
await bitstring.encodeBits();
```

### decodeBits({encoded})
Decodes and uncompresses a given base64url encoded string to a Uint8Array.
```js
await Bitstring.decodeBits({encoded});
```

### compressBits()
Compresses bits to a Uint8Array.
```js
await bitstring.compressBits();
```

### uncompressBits({compressed})
Uncompresses compressed bits.
```js
await Bitstring.uncompressBits({compressed});
```

## Contribute

Please follow the existing code style.

PRs accepted.

If editing the Readme, please conform to the
[standard-readme](https://github.com/RichardLitt/standard-readme) specification.

## Commercial Support

Commercial support for this library is available upon request from
Digital Bazaar: support@digitalbazaar.com

## License

[BSD-3-Clause](LICENSE.md) © Digital Bazaar
