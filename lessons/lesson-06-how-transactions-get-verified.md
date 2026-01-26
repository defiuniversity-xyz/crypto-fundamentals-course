---
course: crypto-fundamentals
module: 2
lesson: 6
title: "How Transactions Get Verified"
description: "Understanding consensus mechanisms without the technical complexity"
---

# How Transactions Get Verified
![Header](https://storage.googleapis.com/crypto-fundamentals-media/images/lesson_06/crypto-fundamentals_06_header.png)


**Core concept:** Blockchain transactions are verified by multiple independent parties agreeing on what happened—like having multiple witnesses sign a document.

---

## Multiple Witnesses Signing a Document


![Inline Analogy](https://storage.googleapis.com/crypto-fundamentals-media/images/lesson_06/crypto-fundamentals_06_inline_analogy.png)
Imagine you're signing an important contract. Instead of one notary, you have 1,000 independent notaries who all:
- Watch you sign
- Check that your signature is valid
- Record the signing in their own records
- Compare notes with each other

For the contract to be "official," the majority of these witnesses must agree it happened correctly. No single witness can fake your signature because all the others would notice and disagree.

This is how blockchain verification works. Many independent parties (called validators or miners) check every transaction. Only when enough of them agree does the transaction become "confirmed."

---

## What Gets Checked


![Infographic](https://storage.googleapis.com/crypto-fundamentals-media/images/lesson_06/crypto-fundamentals_06_infographic.png)
When you send cryptocurrency, validators verify:

**Do you have enough?** They check your address's balance in the blockchain history. If you're trying to send 5 BTC but only have 2 BTC, the transaction is rejected.

**Is your authorization valid?** The transaction includes a cryptographic signature proving you control the sending address. Validators verify this signature matches the public key.

**Are there any conflicts?** They check that you're not trying to spend the same funds twice (called "double-spending"). This is the core problem blockchain solves.

**Does it follow the rules?** Each blockchain has rules (like maximum transaction size). Validators ensure transactions comply.

---

## Proof of Work: Bitcoin's Approach

Bitcoin uses "Proof of Work" for verification. Here's the simple version:

**Miners** are people running powerful computers that:
1. Collect pending transactions into a block
2. Race to solve a mathematical puzzle
3. The winner adds their block to the chain
4. The winner gets newly created Bitcoin as reward

The puzzle requires enormous computing power to solve but is easy to verify once solved. This makes cheating expensive (you'd need more computing power than everyone else combined) while keeping verification cheap.

**Downsides:** Uses significant electricity. Can be slow. Limited transactions per second.

---

## Proof of Stake: Ethereum's Approach

Ethereum (and many newer blockchains) use "Proof of Stake":

**Validators** put up cryptocurrency as collateral ("stake"). They:
1. Get chosen to propose blocks (probability based on stake size)
2. Verify transactions and create blocks
3. Other validators check their work
4. Earn rewards for honest behavior
5. Lose stake if they act maliciously

The security comes from having "skin in the game." Cheating means losing your staked funds, which could be worth millions.

**Upsides:** Far less energy use. Faster. Can handle more transactions.

**Downsides:** Critics argue it favors the wealthy. Different security assumptions.

---

## Why Multiple Verification Matters

Traditional verification relies on trusting one party (your bank). Problems:
- Single point of failure
- Must trust they're honest
- Must trust they're competent
- If compromised, whole system fails

Blockchain verification distributes trust across thousands of parties:
- No single point of failure
- Don't need to trust any individual
- Majority must be honest (easier threshold)
- Compromising the system requires compromising the majority

It's the difference between trusting one security guard versus having a crowd where any witness can blow the whistle.

---

## Confirmation Times and Finality

After your transaction is included in a block, you wait for "confirmations":

**1 confirmation:** Included in most recent block. Good for small amounts.

**3-6 confirmations:** Standard for medium amounts. Very unlikely to be reversed.

**12+ confirmations:** High security for large amounts. Reversing would be practically impossible.

Each new block added makes reversing old blocks harder. Time = security.

Different blockchains have different confirmation times:
- Bitcoin: ~10 minutes per block
- Ethereum: ~12 seconds per block
- Solana: ~0.4 seconds per block

Faster isn't always better—there are trade-offs between speed and security.

---


![Summary](https://storage.googleapis.com/crypto-fundamentals-media/images/lesson_06/crypto-fundamentals_06_summary.png)

## Key Takeaways

- **Transactions are verified by many independent parties** reaching consensus, not a single authority
- **Validators check: funds available, valid signature, no double-spending, rule compliance**
- **Proof of Work (Bitcoin):** Miners compete by solving puzzles, expensive to cheat
- **Proof of Stake (Ethereum):** Validators stake collateral, lose it if they cheat
- **Multiple confirmations increase security**—more blocks = harder to reverse
- **Different blockchains make different speed/security trade-offs**

---

## Media Specifications

### Header Image
**Concept:** Document surrounded by multiple witnesses/notaries all holding stamps of approval
**Style:** Official, multi-party verification visual
**Dimensions:** 1200x630px

### Concept Infographic
**Title:** "What Validators Check"
**Content:** Checklist showing: ✓ Sufficient funds, ✓ Valid signature, ✓ No double-spend, ✓ Follows rules. Show the flow from transaction to confirmed.
**Style:** Verification checklist with checkmarks

### Analogy Illustration
**Concept:** 1,000 notaries watching a signing, contrasted with one notary alone
**Style:** Crowd of witnesses vs. single point of trust

### Audio Notes
- Start with the multiple witnesses analogy
- Explain what gets checked in simple terms
- Cover PoW and PoS at high level—don't get too technical
- Duration target: 4-5 minutes

### Video Concept
- Animation of transaction being broadcast to many validators
- Show them all checking the same things
- Consensus forming as majority agrees
- Duration: 2-3 minutes
