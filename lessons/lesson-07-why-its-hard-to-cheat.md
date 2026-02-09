---
module: 2
lesson_number: 7
course: crypto-fundamentals
---

🎧 Lesson Podcast
{% embed url="https://storage.googleapis.com/crypto-fundamentals-media/lesson-07/audio/lesson7-Why_You_Can_t_Rewrite_Blockchain_History.m4a" %}

🎬 Video Overview
{% embed url="https://storage.googleapis.com/crypto-fundamentals-media/lesson-07/video/lesson7-Why_Blockchains_Are_Immutable.mp4" %}

# Why It's Hard to Cheat

![Header](https://storage.googleapis.com/crypto-fundamentals-media/images/lesson_07/crypto-fundamentals_07_header.png)


**Core concept:** Changing one transaction in blockchain history is like changing one puzzle piece—it breaks the entire picture, and everyone notices.

---

## The Puzzle Piece Analogy


![Inline Analogy](https://storage.googleapis.com/crypto-fundamentals-media/images/lesson_07/crypto-fundamentals_07_inline_analogy.png)

Imagine a completed 10,000-piece puzzle displayed in a public square. Everyone has a photo of what the completed puzzle looks like.

Now try to secretly replace one piece with a different one. What happens?

- That piece doesn't fit quite right
- The surrounding pieces look wrong
- The changed area doesn't match everyone's photos
- Someone notices and points it out

Blockchain works similarly. Each "block" is linked to the previous block through a cryptographic hash—a kind of fingerprint. Change anything in an old block, and its fingerprint changes. That breaks the link to the next block, which breaks the link to the block after that, all the way to the present.

To successfully cheat, you'd need to rebuild every puzzle piece from the changed one to today—while everyone watches and while others are still adding new pieces faster than you can keep up.

---

## What Is a Hash?


![Infographic](https://storage.googleapis.com/crypto-fundamentals-media/images/lesson_07/crypto-fundamentals_07_infographic.png)

A hash is a digital fingerprint created by running data through a mathematical function:

**Input:** "Send 5 BTC from Alice to Bob"
**Output (hash):** "7f83b1657ff1fc53b92dc18148a1d65d" (example)

Key properties:

**Deterministic:** Same input always produces same output.

**One-way:** Easy to create hash from input. Practically impossible to reverse.

**Avalanche effect:** Tiny input changes create completely different outputs. "Send 5 BTC" vs "Send 6 BTC" produces totally different hashes.

Each block contains the hash of the previous block. Change anything in block 100, and block 100's hash changes. Now block 101's reference to "block 100's hash" is wrong—it points to something that doesn't exist.

---

## The 51% Attack (And Why It's Hard)

The main theoretical way to cheat a blockchain is a "51% attack":

If someone controls more than half of the network's validation power (computing power for Bitcoin, staked funds for Ethereum), they could potentially:
- Reverse recent transactions
- Double-spend their funds
- Censor specific addresses

Why this is extremely difficult for major blockchains:

**Bitcoin:** You'd need more computing power than thousands of professional mining operations combined. The cost is estimated in billions of dollars, plus ongoing electricity costs. Even if you could afford it, acquiring that much hardware would take years and tip people off.

**Ethereum:** You'd need to buy and stake more ETH than all current validators combined—tens of billions of dollars worth. And you'd be attacking your own investment, since success would crash the value.

The economics make attacks irrational for large networks. The potential gain is smaller than the certain cost.

---

## Smaller Networks Are Riskier

The 51% protection works because major networks are massive. Smaller blockchains don't have this protection:

**Ethereum Classic** (a smaller Bitcoin-like chain) was 51% attacked multiple times. Attackers rented mining power temporarily to double-spend on exchanges.

**Multiple small coins** have been successfully attacked for profits.

This is why "how big/secure is the network?" matters when evaluating a cryptocurrency. Security comes from decentralization AND scale.

---

## Other Security Layers

Beyond hash linking and decentralization:

**Time:** Each block that passes makes old blocks harder to change. Six Bitcoin confirmations means an attacker would need to rewrite six blocks while the network continues adding more.

**Economic incentives:** Validators/miners profit from honest behavior. Cheating risks their income stream.

**Social coordination:** If an attack happened, the community could coordinate a response (like forking away from the attacker).

**Cryptographic signatures:** Even if someone changed a block, they couldn't create valid signatures for others' transactions without their private keys.

---

## What CAN Go Wrong

Blockchain security is strong but not absolute:

**Smart contract bugs:** The blockchain can be secure while applications built on it have vulnerabilities.

**User error:** Sending to wrong addresses, losing keys, falling for scams.

**Exchange hacks:** The blockchain is fine; the exchange wasn't.

**51% attacks on small chains:** Rare but happen.

**Fundamental cryptographic breaks:** If the math underlying encryption fails (currently very unlikely), everything would need redesigning.

Understanding both the strengths and limitations helps you make informed decisions about what to trust blockchain with.

---


![Summary](https://storage.googleapis.com/crypto-fundamentals-media/images/lesson_07/crypto-fundamentals_07_summary.png)

## Key Takeaways

- **Hash linking** makes changing old blocks break all subsequent blocks
- **Rebuilding the chain is impractical**—you'd race against the entire network adding new blocks
- **51% attacks are theoretically possible** but economically irrational for major networks
- **Small networks have less security**—decentralization AND scale matter
- **Multiple layers protect blockchain**: cryptography, economics, social coordination, and time
- **Blockchain isn't invulnerable**—risks include smart contract bugs, user error, and exchange failures
