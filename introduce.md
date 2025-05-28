---
description: Ivy is a FaaS (Finality-as-a-service) Protocol for sloving scalability and interoperability issues of Ethereum.
cover: assets/Frame.png
coverY: 0
---

# Introduce
Ivy is a **Finality-as-a-Service (FaaS)** protocol that provides fast and secure finality confirmation services for integrated rollup chains and bridged external chains.

The essence of scalability and interoperability challenges lies in the global awareness of finalized blockchain states. Therefore, Ivy Protocol builds a unified finality confirmation service that inherits Ethereum economic security. Chains connected to this service form a unified and provable communication channel. Through this channel, Ivy enables both secure and fast finality confirmation for Ethereum scalability, and verifiable omnichain interoperability across the blockchain ecosystem.

Ivy Protocol’s finality confirmation service is characterized by the following features:

* **Fast Finality Confirmation:**  
  Ivy Protocol Designed the IvyBFT consensus algorithm, which enables state finality confirmation within seconds (\~1s). This allows integrated rollup chains to achieve secure confirmation of Layer 2 transactions in a very short time. Each rollup chain can flexibly construct its own sequencing layer while leveraging Ivy’s service to guarantee high throughput with low latency.  
* **Omnichain Verifiable Interoperability:**  
  States finalized within Ivy Protocol can circulate and be utilized freely across the ecosystem to verify cross-chain operation. This supports various use cases including cross-chain asset transfers and general message passing.  
* **Inheriting Ethereum’s Security:**  
  Through liquidity & native tokens restaking, Ivy Network inherits Ethereum’s economic security. This allows Ivy nodes to join and exit permissionlessly, collaboratively participate in state finality confirmation, and provide security guarantees.  
* **Support for Decentralized Sequencers:**  
  Ivy decouples transaction sequencing from state finality confirmation, enabling a modular design for sequencing layers. The provided standard SDK supports rollup chains in selecting either centralized or decentralized sequencing models as needed. Regardless of the sequencing approach, state transitions remain secure, trustworthy, and fork-free. Finality confirmation is conducted independently within isolated partitions, ensuring that faults in one chain do not affect the rest of the network.

The following questions help illustrate Ivy Protocol’s core design principles:

**Why Fast Finality?**  
Slow finality leads Layer 2 users to rely on pre-confirmations from centralized sequencer, reducing security and introducing the risk of forks. Ivy reduces the finality delay within seconds (\~1s) , backed by sufficient economic security, effectively eliminating trust costs.

**Why Restake?**  
By inheriting Ethereum’s economic security through restaking, Ivy also incentivizes deep participation from Ethereum validators in the Ivy ecosystem via a reward mechanism.

**Why Fraud Proof & Slashing?**  
While the restaked BFT network reduces inherent attack risks, Ivy further enforces security through fraud-proof mechanisms and slashing. All detectable misbehaviors—including consensus forks, invalid state transitions, and malicious reorgs—are slashable, enforcing cryptoeconomic security.

**Why Permissionless Election?**  
A more fair and decentralized validator election mechanism allows any node to participate. The validator committee is elected based on the total delegated stake.

**Why Omnichain Interoperability?**  
Interoperability must go beyond internal ecosystem boundaries to include external chains. Both messages and assets need to transfer reliably throughout the entire blockchain landscape.