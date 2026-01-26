---
course: crypto-fundamentals
module: 2
lesson: 5
title: "What is a Blockchain?"
description: "Understanding blockchain as a shared, unchangeable record book"
---

# What is a Blockchain?

![Header](https://storage.googleapis.com/crypto-fundamentals-media/images/lesson_05/crypto-fundamentals_05_header.png)


**Core concept:** A blockchain is like a shared Google Doc that everyone can see, no one can secretly edit, and which keeps a perfect history of every change ever made.

---

## The Shared Google Doc


![Inline Analogy](https://storage.googleapis.com/crypto-fundamentals-media/images/lesson_05/crypto-fundamentals_05_inline_analogy.png)

Imagine a Google Doc that:
- Everyone in the world can view
- Anyone can add new lines (following rules)
- No one can delete or change old lines
- Every change is timestamped and permanent
- Thousands of people have identical copies

That's essentially what a blockchain is—a shared document (ledger) that records transactions. The "chain" comes from how new records link to old records, making the history tamper-evident.

Instead of a bank keeping private records of who has what, the blockchain is a public record that anyone can verify. No single entity controls it.

---

## Breaking Down the Name


![Infographic](https://storage.googleapis.com/crypto-fundamentals-media/images/lesson_05/crypto-fundamentals_05_infographic.png)

**Block:** A collection of transactions bundled together. Like a page in a ledger book. Every 10 minutes (Bitcoin) or few seconds (other blockchains), a new "page" gets added.

**Chain:** Each new block includes a reference to the previous block, creating a chain. Block 100 references Block 99, which references Block 98, and so on back to the first block.

This chaining is crucial: if someone tried to change Block 50, the reference in Block 51 wouldn't match anymore, and neither would any block after. You'd have to change everything—which is practically impossible.

---

## What's Actually Recorded?

Blockchain transactions typically include:

**Sender:** Who's sending (represented as a public address, not a name)

**Recipient:** Who's receiving (another public address)

**Amount:** How much is being transferred

**Timestamp:** When it happened

**Unique identifier:** A transaction ID for reference

**Cryptographic proof:** Mathematical evidence that the sender authorized this

All of this is public. Anyone can see every transaction ever made on the network. What they can't see is who the addresses belong to (unless you tell them).

---

## Who Maintains the Record?

Traditional ledgers have a single keeper—the bank maintains their records. If they make a mistake or act dishonestly, you might never know.

Blockchain ledgers have thousands of keepers. Everyone running the network software (called nodes) keeps a complete copy. They're constantly checking each other.

If one computer tries to record something false, thousands of other computers will disagree, and the false record gets rejected. It's like having thousands of witnesses to every transaction.

---

## Why This Matters

The blockchain structure creates several properties:

**Transparency:** Anyone can audit the complete history of transactions

**Immutability:** Old records can't be secretly changed

**Decentralization:** No single party controls the ledger

**Censorship resistance:** No one entity can block transactions

**Verifiability:** You don't have to trust anyone—you can check yourself

These properties enable "trustless" systems. Not "without trust" but rather "trust isn't required"—you verify instead of trust.

---

## What Blockchain Doesn't Do

Blockchain isn't magic. It doesn't:

**Guarantee correctness of initial data:** If someone records false information originally, it will be permanently and transparently false.

**Solve all verification problems:** The blockchain can confirm Transaction X happened, but can't inherently verify that the real-world event it represents actually occurred.

**Make everything private:** Most blockchains are extremely public. Privacy requires additional layers.

**Replace all databases:** Blockchain is slower and more expensive than centralized databases. It only makes sense when the specific properties above matter.

Understanding what blockchain doesn't do is as important as understanding what it does.

---


![Summary](https://storage.googleapis.com/crypto-fundamentals-media/images/lesson_05/crypto-fundamentals_05_summary.png)

## Key Takeaways

- **Blockchain is a shared, public ledger** that records transactions for everyone to see
- **"Blocks" of transactions are "chained" together** with cryptographic references
- **Thousands of computers keep identical copies**, making manipulation extremely difficult
- **Anyone can verify any transaction**—no trust required
- **Properties include transparency, immutability, and censorship resistance**
- **Blockchain has limitations**—it doesn't guarantee truth of initial data or suit all use cases
