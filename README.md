# TRC20 Address

a Golang package to generate a new TRC20 wallet address offline or get one from private key.

## Usage

```golang
import (
  "github.com/spcily/trc20/address"
)
```

### Generate a new address

```golang
privateKey, hexAddress, base58Address := address.Generate()
```

### Get from private key

privateKeyHex is a hex string of private key. eg. `0xf5737b0a37b87451a52863e0bbec15ab06983540f41b5b06b322ad1a1f8eef72`.

```golang
privateKey, hexAddress, base58Address := address.GetFromPrivateKey(privateKeyHex)
```

### Return

Both functions returns a Address struct

address.PrivateKeyHex: private key in hex string format

address.AddressHex: wallet address in hex string format

address.Base58Address: wallet address in base58check format

# LICENSE

MIT
