# PLUG.

**Programmable Locking UTXO Gateway**

Bitcoin Script contracts. Ledger signed. No custody.

---

### What is PLUG?

PLUG is a Bitcoin programmability tool — not a wallet. It lets you create complex smart contract transactions on Bitcoin's base layer, signed exclusively by your Ledger hardware wallet. Your keys never leave the device.

### Features

- **Time-Lock Vaults** — Lock sats until a future block with `OP_CHECKLOCKTIMEVERIFY`
- **Inheritance** — Automatic heir access after inactivity with `OP_CHECKSEQUENCEVERIFY`
- **Hash Time-Lock (HTLC)** — Conditional payments with SHA256 preimage
- **Payment Channels** — 2-of-2 multisig with CLTV timeout refund
- **Multisig Pool** — M-of-N `OP_CHECKMULTISIG` shared custody
- **P2P Atomic Swap** — Trustless exchange via paired HTLCs, no intermediary
- **CoinJoin** — Serverless collaborative transactions for privacy
- **OP_RETURN** — Embed data on the blockchain
- **Taproot (P2TR)** — Multi-key contracts with key-path and script-path spending

### Architecture

- Native iOS app (Swift / SwiftUI)
- Ledger hardware wallet signing via BLE (Nano X / Stax / Flex)
- V2 merkleized PSBT protocol
- P2WSH and P2TR script construction
- Mempool.space API for network data
- No server, no token, no custody

### Security

- Zero private keys on device — only xpubs
- Ledger signs every transaction
- Address rotation — never reuse spent-from addresses
- Coin control for UTXO selection
- Encrypted backups (AES-256-GCM + PBKDF2)
- Optional Tor routing

### Status

Testnet4 — launching soon.

### Links

- Website: [bitcoin-plug.com](https://bitcoin-plug.com)
- Twitter: [@seeduser99](https://x.com/seeduser99)

---

*Not your keys, not your coins. Not your script, not your rules.*
