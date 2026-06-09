# Kudos (KUDS)

A good deed token. Share a Kudos when someone does something kind. Pass it forward.

That's the whole idea. No price, no trading, no roadmap to the moon. Just a way to say *I saw what you did, and it mattered* — recorded permanently on a blockchain.

**Live on Solana mainnet** → [verify the token yourself](https://explorer.solana.com/address/7PxuFRWRfzyBz1jYFYn4shGTHY5U5YhTCNXbKwt3CuGZ)

---

## Why this exists

I kept noticing that small acts of kindness disappear. Someone helps you move, talks you off a ledge before an interview, shows up when they didn't have to — and a week later there's no trace of it anywhere.

So I made a token for it. 500 Kudos exist. That's it, forever. When you give someone a KUDS, you're giving them something genuinely scarce. The first ones went to my family.

I also built this to answer a question for myself: could I take a technology I knew nothing about and ship something real on it? I started with zero blockchain experience. This repo is the answer.

## Token details

| | |
|---|---|
| **Name** | Kudos |
| **Symbol** | KUDS |
| **Network** | Solana (mainnet-beta) |
| **Standard** | SPL Token |
| **Total supply** | 500 (fixed) |
| **Decimals** | 0 — you can't give someone half a kudos |
| **Mint address** | `7PxuFRWRfzyBz1jYFYn4shGTHY5U5YhTCNXbKwt3CuGZ` |

## Design decisions

**Fixed supply of 500.** Scarcity is the point. If kudos were infinite, they'd mean nothing — same reason a handwritten note beats a like.

**Zero decimals.** A kudos is whole or it isn't given.

**Deliberately non-financial.** KUDS has no liquidity pool, no listing, and no intended monetary value. It's a social object that happens to live on a blockchain because blockchains are good at two things this needs: permanence and verifiable scarcity.

**Mint authority not yet revoked.** I know the standard advice is to revoke it immediately. I kept it for now — deliberately — while I finish the project's first phase. Revoking is one command and it's on the list. I'd rather be honest about that than pretend the project is more "done" than it is.

## How it was built

Zero to mainnet, roughly in this order:

1. Wrote a short whitepaper to force myself to define what this actually was
2. Set up a Solana wallet and learned the CLI
3. Created the SPL token on **devnet** first — minted, transferred, broke things where it was free to break them
4. Designed the tokenomics (supply, decimals, distribution)
5. Created the mint on **mainnet**, minted the full 500 supply
6. Attached metadata and logo (hosted in this repo)
7. Sent the first Kudos to my family

Stack: Solana CLI, SPL Token program, JSON metadata hosted on GitHub.

The honest version: most of the time went into understanding *why* each step exists, not running the commands. Devnet-to-mainnet is a small change in a config flag and a big change in how careful you suddenly become.

## What's in this repo

- `kudos-metadata.json` — on-chain token metadata
- `kuds-logo (2).png` — the KUDS logo

## Give a kudos

If you hold KUDS and someone does something kind, send them one from any Solana wallet using the mint address above. Tell them why. That part matters more than the token.

---

Built by [Harshni Desai](https://hdesai96.github.io) · [LinkedIn](https://www.linkedin.com/in/harshni-desai)
