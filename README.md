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
|       |                                   |           |
|       +-----> [ NETWORK COMPARATOR ] <----+           |
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

Secret Duplication: A small percentage of all tasks (training and inference) are secretly duplicated and sent to multiple nodes. The mathematical results are compared for consistency.

Because consumer hardware can produce slight numerical differences and AI generation is often probabilistic, direct answer comparison can be unreliable. For audited tasks, the protocol enforces deterministic generation settings (e.g., fixed seeds and zero temperature) to ensure reproducible outputs. The network operates under an optimistic fraud-proof model: results are assumed valid by default, but any participant may challenge a suspicious output. Verified misconduct results in penalties, making dishonest computation economically irrational.

Strict Penalties: Dishonest behavior or submitting intentionally junk data results in immediate reputation loss, temporary exclusion from the network, and a reset of participation progress. Cheating is mathematically designed to cost more than it earns.

## 7. Credit Design (The Economy of Priority)

The time credits earned by users are strictly utility tokens used to prioritize AI access when network demand is high.

No Speculation: They cannot be sold, transferred, or converted to cash.

Credit Decay: To prevent early adopters from hoarding priority forever, credits decay slowly over time if hoarded excessively.

## 8. AI Curriculum Governance

While the AI automatically flags its own weak points for the task queue, participants may spend their credits to propose new datasets or specialization areas for the AI to learn.

Dynamic Topic Pricing: To prevent ideological capture or spam, dominant topics become progressively more expensive to push to the queue. Rare or underrepresented knowledge domains remain inexpensive. Diversity of knowledge is structurally encouraged.

## 9. System Governance

The network is not controlled by a central foundation. Key adjustable parameters require community voting to change, including:

Minimum hardware baseline

Performance multiplier cap

Credit decay rate

Monthly contribution requirement

Audit frequency

## 10. Bootstrapping: The Academic Launchpad

Launching a massive network from scratch is incredibly difficult. Traditionally, projects rely on venture capital, which inevitably leads to investor capture, pressure to monetize, and centralized control.

To protect the protocol, it will not begin as a startup. It will be bootstrapped through academic grants and university research labs.

Phase 1: Research and Prototyping (1-2 Years): Funded by public-interest and AI safety grants, a university lab will build the initial code, test the security, and launch a small pilot network. All code will be strictly open-source. The university hosts the research; it does not own the AI.

Phase 2: The Genesis Launch: Once the protocol is stable, the network goes live to the public, and the university completely steps away.

The Scaffolding Must Disappear
To guarantee the institution does not become a permanent dictator, hardcoded transition rules will apply:

No Backdoors: The original developers retain zero master keys, admin privileges, or override switches.

No Founder Perks: Governance rights are strictly earned through participation. The founding researchers enter the live system with the exact same zero-balance standing as a new user.

The Self-Destruct Clause: Any foundation or nonprofit created to coordinate the launch must include a legally binding sunset clause, forcing it to dissolve once the community takes over.

This approach intentionally trades the rapid growth of a tech startup for the durability of a public utility. The academic phase is merely scaffolding—it is designed to be torn down the moment the network can stand on its own.

