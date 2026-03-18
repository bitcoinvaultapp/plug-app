# PLUG.

**Programmable Locking UTXO Gateway**

Bitcoin Script contracts. Ledger signed. No custody.

---

### What is PLUG?

PLUG is a Bitcoin programmability tool, not a wallet. It lets you create smart contract transactions on Bitcoin's base layer, signed exclusively by your Ledger hardware wallet. Your keys never leave the device.

### Features

- **Time-Lock Vaults** `CLTV` Lock sats until a future block
- **Inheritance** `CSV` Heir access after inactivity
- **Hash Time-Lock** `HTLC` Conditional payments with SHA256 preimage
- **Payment Channels** `2-of-2` Multisig with timeout refund
- **Multisig Pool** `M-of-N` Shared custody
- **P2P Atomic Swap** `HTLC x 2` Trustless exchange, no intermediary
- **CoinJoin** `PSBT` Collaborative transactions for privacy
- **OP_RETURN** `DATA` Embed data on the blockchain
- **Taproot** `P2TR` Multi-key contracts with script-path spending

### Architecture

- Native iOS (Swift / SwiftUI)
- Ledger signing via BLE (Nano X / Stax / Flex)
- V2 merkleized PSBT protocol
- P2WSH and P2TR script construction
- Mempool.space API
- No server, no token, no custody

### Security

- Zero private keys on device, only xpubs
- Ledger signs every transaction
- Address rotation, never reuse spent-from addresses
- Coin control for UTXO selection
- Encrypted backups (AES-256-GCM + PBKDF2)
- Optional Tor routing

### Status

Testnet4 launching soon.

### Links

- Website: [bitcoin-plug.com](https://bitcoin-plug.com)
- Twitter: [@seeduser99](https://x.com/seeduser99)

---

*Not your keys, not your coins. Not your script, not your rules.*
