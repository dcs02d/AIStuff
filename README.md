# The Proof-of-Personhood AI Protocol
### A Human-Powered, Decentralized AI Network

## 1. Vision & Core Principles
Today’s most powerful AI systems are controlled by a small number of corporations with massive centralized data centers. This project proposes a different path: build and run AI using verified human participation, not capital concentration.

```text
+-------------------------------------------------------+
|           DECENTRALIZED AI NETWORK ARCHITECTURE       |
|                                                       |
|      [Node A] <-------> [Node B] <-------> [Node C]   |
|         |                  |                  |       |
|         v                  v                  v       |
|   +-----------+      +-----------+      +-----------+ |
|   | Human &   |      | Human &   |      | Human &   | |
|   | Personal  |      | Personal  |      | Personal  | |
|   | Computer  |      | Computer  |      | Computer  | |
|   +-----------+      +-----------+      +-----------+ |
|         ^                  ^                  ^       |
|         |                  |                  |       |
|         +-------> [ SHARED AI MODEL ] <-------+       |
|         |        (Distributed & Public)       |       |
|         v                  v                  v       |
|      [Node D] <-------> [Node E] <-------> [Node F]   |
|                                                       |
|   * No Central Server  * Peer-to-Peer  * Human Owned  |
+-------------------------------------------------------+
```

The Proof-of-Personhood AI Protocol is a decentralized network where every participant is a real human, the AI is trained and hosted across personal computers, and contributions are rewarded in non-financial priority credits. It is an attempt to create AI as public infrastructure—owned and maintained by people.

At its core, this protocol is trying to balance three competing forces: Egalitarianism, Efficiency, and Anti-Capital Capture. This balance is inherently difficult to strike. This proposal explicitly favors egalitarianism and anti-capital capture, accepting that this comes at some cost to raw technical efficiency.

Core Principles:

One Person, One Account: Each human can create only one permanent identity.

No Financial Tokens: Credits earned cannot be sold or traded.

Contribution Unlocks Access: Priority access to the AI is earned by helping build and run it.

Hardware Equality with Incentives: Better hardware is rewarded slightly more to prevent network stagnation, but strictly capped to prevent capital dominance.

Open Governance: System parameters evolve through community voting.

## 2. Technical Scope

This protocol is intentionally designed to support medium-sized, highly efficient open models (e.g., the 7B–13B parameter range), distributed fine-tuning, and swarm-based inference.

To overcome the latency and bandwidth limits of standard consumer internet, the network will leverage asynchronous federated learning and parameter-efficient architectures—such as Low-Rank Adaptation (LoRA) or distributed low-communication (DiLoCo) methods—which drastically reduce the amount of data each device must transmit.

It is not currently intended to compete with frontier corporate supercomputer clusters. The goal is resilient, distributed, public AI infrastructure—not maximal scale at any cost.

## 3. Identity and Reputation

To prevent bots and multi-account abuse, participation is anchored to strict human verification. We acknowledge that achieving a flawless, privacy-preserving "One Person, One Account" system remains an open research challenge in the field of decentralized networks; however, this protocol builds upon the most recent open-source attempts to resolve this—such as the early 2026 open-sourcing of the Human Network (the cryptographic foundation of Human Passport), which utilizes zero-knowledge proofs and verifiable Oblivious Pseudorandom Functions (vOPRF) to establish strict Sybil resistance without exposing underlying personal data.


```text
+-------------------------------------------------------+
|        ZERO-KNOWLEDGE PROOF IDENTITY VERIFICATION     |
|                                                       |
|  [ PROVER (User) ]               VERIFIER (Network) ] |
|         |                                     |       |
|  +------+------+                      +------+------+ |
|  | Private Data|                      |   Request   | |
|  | (Biometrics)| <---- Challenge ---- |   Proof     | |
|  +------+------+                      +------+------+ |
|         |                                     |       |
|   Generate ZK-Proof                           |       |
|   (Mathematical Guarantee)                    |       |
|         |                                     |       |
|         +---------> Send ZK-Proof ----------->+       |
|                                               |       |
|                                       Verify Proof    |
|                                 (Without seeing data) |
|                                               |       |
|                                       +------+------+ |
|                                       | [✓] VERIFIED| |
|                                       | Unique Human| |
|                                       +-------------+ |
+-------------------------------------------------------+
```
The Permanent ID: Each participant completes a verification process to receive a non-transferable digital identity.

    Anti-Farming Economics: Creating identities requires progressively higher upfront contribution work. This makes large-scale fake identity farming economically irrational.

    The Reputation System: Each node builds a reputation score based on successful task completion, accuracy, and reliability. This reputation dictates network routing preference and decays slowly with inactivity.

## 4. Earning Credits (The Task Board)

Credits are earned exclusively through verified work in two main categories:

A. Training & Data Contribution (The Data Studio)
Participants help improve the AI by submitting new public knowledge, processing data into usable formats, and completing training tasks.

    This can be done manually (curating original text) or through approved bulk-processing scripts.

B. Running Inference (Proof of Inference)
The finished AI is hosted directly on the network of user devices. Participants earn credits when:

    Their device processes real AI prompts and the response passes verification.

    They maintain a minimum monthly active contribution level.

Note: Devices are not paid simply for being online; they are paid only for successful work.
## 5. Performance Rewards & The Hardware Floor

To ensure the decentralized swarm processes AI prompts at a usable speed, the network establishes a minimum hardware baseline (e.g., a standard $500 consumer computer).

    Fair but Capped: To prevent network stagnation, faster and more reliable machines earn modestly higher rewards. However, these multipliers are strictly capped (e.g., 1.5× maximum).

    This ensures a standard consumer computer remains fully viable and encourages hardware improvement without allowing capital domination.

## 6. Distributed Consensus and Audits

The AI is built piece-by-piece on the computers of the users. To prevent cheating and ensure accuracy across millions of different devices:
```text
+-------------------------------------------------------+
|       DISTRIBUTED CONSENSUS & AUDIT PROTOCOL          |
|                                                       |
|    Task Generator (Network)                           |
|           |                                           |
|           +---> [Creates Task X]                      |
|           |                                           |
|    +------+-------+           +-------+-------+       |
|    | Sends to     |           | Secretly sends|       |
|    | Node A       |           | to Node B     |       |
|    +------+-------+           +-------+-------+       |
|           |                           |               |
|    [ Node A processes ]       [ Node B processes ]    |
|           |                           |               |
|    +------+-------+           +-------+-------+       |
|    | Submits      |           | Submits       |       |
|    | Result A     |           | Result B      |       |
|    +------+-------+           +-------+-------+       |
|           |                           |               |
|           +-----> [ NETWORK COMPARATOR ] <----+       |
|                       |                               |
|             DO RESULTS MATCH (within tolerance)?      |
|                       |                               |
|           [YES] ------+------ [NO]                    |
|             |                   |                     |
|    +--------+--------+  +-------+---------+           |
|    | Award Credits   |  | Trigger Audit / |           |
|    | Update Reputation| | Penalize Nodes  |           |
|    +-----------------+  +-----------------+           |
+-------------------------------------------------------+
```
