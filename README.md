# X25519

X25519 adapter for WebAssembly and JS implementations

```bash
npm i @hazae41/x25519
```

[**Node Package 📦**](https://www.npmjs.com/package/@hazae41/x25519)

## Features

### Current features
- 100% TypeScript and ESM
- No external dependencies

## Usage

### Berith (WebAssembly)

```typescript
import { X25519 } from "@hazae41/x25519"
import { Berith } from "@hazae41/berith"

await Berith.initBundledOnce()
const x25519 = X25519.fromBerith(Berith)
```

### Noble (JavaScript)

```typescript
import { X25519 } from "@hazae41/x25519"
import * as noble_ed25519 from "@noble/curves/ed25519"

const x25519 = X25519.fromNoble(noble_ed25519.x25519)
```
