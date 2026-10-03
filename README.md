# Multi-Chain Wallet Generator

A simple, client-side multi-chain wallet generator that creates **one recovery phrase** for:

- Bitcoin
- Ethereum & all EVM-compatible chains
- Solana

Everything is computed **100% in your browser**. No data is ever sent to any server.

---

## Features

- Generate a 12 or 24-word BIP-39 recovery phrase
- Optional BIP-39 passphrase support
- Custom Account Index
- Instantly derive addresses for Bitcoin, Ethereum (EVM), and Solana
- Fully client-side (works offline once loaded)
- Clean and simple interface

---

## Important Security Warning

> **Anyone who has your recovery phrase + passphrase can control your funds.**

- This tool is intended for **learning and testing**.
- For serious amounts of money, we strongly recommend:
  - Generating the wallet on an offline/air-gapped computer, or
  - Using a hardware wallet (Ledger, Trezor, Coldcard, etc.)

Never enter your recovery phrase on a website you don’t fully trust.

---

## How to Use

1. Open the generator in your browser.
2. Choose your preferred settings:
   - **Phrase length**: 12 or 24 words (24 words recommended)
   - **Account index**: Leave at `0` for the default wallet
   - **Passphrase** (optional): Add an extra password for higher security
3. Click **Generate new wallet**.
4. Write down the 24-word recovery phrase and passphrase (if used) on paper.
5. Store the backup in a safe place.

You can also click **Use my own phrase** to import an existing recovery phrase.

---

## Supported Chains

| Chain              | Address Type          | Derivation Standard     |
|--------------------|-----------------------|-------------------------|
| Bitcoin            | Native SegWit (bc1)   | BIP84                   |
| Ethereum + EVM     | Standard 0x address   | BIP44                   |
| Solana             | Standard Solana       | BIP44 / Phantom path    |

---

## Technical Details

- Uses standard **BIP-39** mnemonic generation
- Supports optional **BIP-39 passphrase**
- All key derivation happens locally in the browser using well-known cryptographic libraries
- No backend, no tracking, no analytics

---

## Disclaimer

This software is provided "as is", without warranty of any kind.  
The authors are not responsible for any loss of funds.  
Always verify addresses and test with small amounts first.

Use at your own risk.

---

## License

MIT License
