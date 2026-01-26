---
course: crypto-fundamentals
module: 3
lesson: 10
title: "Public Keys and Addresses"
description: "Understanding the 'email address' of cryptocurrency"
---

# Public Keys and Addresses

![Header](https://storage.googleapis.com/crypto-fundamentals-media/images/lesson_10/crypto-fundamentals_10_header.png)


**Core concept:** Your public address is like your email address—safe to share, needed by anyone who wants to send you something.

---

## Email Address vs. Email Password


![Inline Analogy](https://storage.googleapis.com/crypto-fundamentals-media/images/lesson_10/crypto-fundamentals_10_inline_analogy.png)

Your email has two components:

**Email address (e.g., you@gmail.com):**
- Safe to share publicly
- Anyone can send you messages using it
- Knowing it doesn't let them read your emails
- You print it on business cards

**Email password:**
- Must be kept secret
- Gives full access to your account
- Sharing it is a security disaster

Crypto works similarly:

**Public address:**
- Safe to share publicly
- Anyone can send you crypto using it
- Knowing it doesn't let them spend your crypto
- You share it to receive payments

**Private key:**
- Must be kept secret
- Gives full access to your funds
- Sharing it means losing everything

---

## What Addresses Look Like

Different blockchains have different address formats:

**Bitcoin:**
- Starts with 1, 3, or bc1
- Example: bc1qxy2kgdygjrsqtzq2n0yrf2493p83kkfjhx0wlh
- 26-35 characters

**Ethereum (and compatible chains):**
- Starts with 0x
- Example: 0x71C7656EC7ab88b098defB751B7401B5f6d8976F
- Always 42 characters

**Solana:**
- Base58 encoded
- Example: 7xKXtg2CW87d97TXJSDpbD5jBkheTqA83TZRuJosgAsU
- 32-44 characters

The format tells you what blockchain the address belongs to. Sending to the wrong type of address = lost funds (usually).

---

## Addresses Are One-Way


![Infographic](https://storage.googleapis.com/crypto-fundamentals-media/images/lesson_10/crypto-fundamentals_10_infographic.png)

The security of crypto relies on one-way mathematical functions:

```
Private Key → Public Key → Address
(secret)      (derivable)   (shareable)
```

- From private key, you can calculate public key and address
- From address, you CANNOT calculate public key or private key
- From public key, you CANNOT calculate private key

This is like how you can crack an egg but can't uncrack it. The math is easy in one direction, practically impossible in reverse.

This means:
- Sharing your address reveals nothing dangerous
- Someone watching the blockchain sees addresses but can't derive private keys
- Your funds remain secure even though your address is public

---

## Address Privacy Considerations

While sharing your address is safe cryptographically, there are privacy implications:

**Blockchain is public:** Anyone can see all transactions to/from any address. If they know your address, they can see your balance and transaction history.

**Address linking:** If someone knows one of your addresses and sees you send to another, they might figure out both are yours.

**Real-world connections:** If you receive payment from someone, they now know at least one of your addresses and can see related activity.

This is why many people:
- Generate new addresses for each transaction
- Use multiple wallets for different purposes
- Consider privacy-focused cryptocurrencies for sensitive transactions

---

## Addresses vs. Usernames

Some services offer human-readable addresses:

**ENS (Ethereum Name Service):** Instead of 0x71C765... you can register "yourname.eth"

**Similar services exist** on other chains (Solana Name Service, etc.)

These work like domain names—easy to remember, resolve to the underlying address. But they're optional additions, not replacements for the cryptographic address underneath.

---

## Checking Addresses Carefully

When sending crypto, always verify addresses carefully:

**Copy-paste carefully:** Malware exists that swaps addresses in your clipboard

**Double-check first and last characters:** Most people verify just these

**Use QR codes when possible:** Reduces typing/copy errors

**Send small test amount first:** Especially for large transfers

Unlike bank transfers, crypto transactions are irreversible. Wrong address = lost funds, usually permanently.

---


![Summary](https://storage.googleapis.com/crypto-fundamentals-media/images/lesson_10/crypto-fundamentals_10_summary.png)

## Key Takeaways

- **Public addresses are like email addresses**—safe to share, needed to receive funds
- **Different blockchains have different address formats**—sending to wrong format = lost funds
- **Addresses are one-way derived**—from private key, not reversible
- **Blockchain is public**—anyone can see transactions to/from known addresses
- **Human-readable names (ENS)** can map to addresses but are optional
- **Always verify addresses carefully**—mistakes are usually irreversible
