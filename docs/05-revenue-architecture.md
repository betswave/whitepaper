---
icon: material/currency-usd
---

# 5. Revenue Architecture

BetsWave's revenue model is structured to sustain platform operations and fund ongoing development while maintaining a low-cost environment for platform users. Revenue sources are diversified to support long-term operational viability.

## 5.1. Primary Revenue Source

The primary revenue source is a fixed Service Processing Fee of **1%** applied to each service transaction processed through the platform. Active ORCA NFT holders are eligible for a reduced Service Processing Fee of **0.5%**. This fee is the principal mechanism by which the platform funds operational continuity, development, and ecosystem programs.

## 5.2. Supplementary Revenue Sources

- **ORCA NFT Membership Sales:** Revenue generated from the issuance of ORCA NFT memberships, which must be acquired using WAVE Tokens.

- **Virtual Analytics Environment Operations:** Revenue from immersive interactive data suite experiences and digital asset activity within the Virtual Analytics Environment.

- **Custom Service Deployments:** Revenue from branded service activations, partner-driven processing formats, and themed platform engagements.

- **Cross-Platform Partnerships:** Commission-based revenue and revenue-sharing arrangements arising from integrations with third-party applications, decentralized applications (DApps), and complementary services.

## 5.3. Service Delivery Models

The BetsWave platform supports two primary service delivery models, each designed to address different user preferences and liquidity profiles.

### 5.3.1. Standard Processing — Pool-Based Model

The Standard Processing model enables participants to submit service requests against the protocol's pooled liquidity reserves, funded through community staking contributions and protocol reserve allocations. This model provides liquidity-guaranteed service request execution without requiring identification of a specific opposing participant.

**Operational Flow:**

1. A participant submits a standard processing request with selected service parameters and pays the applicable 1% Service Processing Fee.
2. The request enters a Created/Pending state within the StandardProcessing.sol smart contract.
3. The service amount is allocated to the global ServicePool.sol contract.
4. Upon processing completion, outputs are retrieved from integrated data APIs or oracle systems and verified on-chain.
5. If the participant's service request is validated and completed, funds are released automatically by smart contract logic and the request is marked as Completed.

### 5.3.2. Direct Processing — Peer-to-Peer Model

The Direct Processing Agreement model represents BetsWave's peer-to-peer service delivery framework, designed to support flexible, trustless, and decentralized service transaction data verification between participants. This model supports both Open Request formats (partial fill permitted) and Confirmed Request formats (full data verification required prior to execution).

#### A) Open Request — Partial Fill Enabled

In this format, service requests may execute upon partial data verification of the total commitment.

1. Participants browse the Processing Board, filter for Open Requests, and view service listings displaying available commitment and fill percentage.
2. A participant selects a service request and may accept any percentage of the available commitment through a slider or input interface, subject to platform-defined minimum and maximum limits.
3. The system calculates the service amount, applicable Service Processing Fee, total payable, and potential payout at confirmed terms.
4. Upon confirmation and on-chain approval, the accepted portion is immediately executed and recorded as a live service request.
5. The original request creator receives confirmation, the Processing Board updates available commitment in real time and the request moves to pending/active requests.
6. Insufficient funds, out-of-range amounts, or expired requests trigger contextual alerts or automatic refund processing.

#### B) Confirmed Request — Full Fill Required

In this format, execution occurs only when the service request has been fully data verified by all participating counterparties.

1. Participants access Confirmed Requests on the Processing Board, where each listing displays Target Commitment, Fill Percentage, and Deadline.
2. Participants commit an amount toward the target within defined minimum and maximum parameters.
3. Upon commitment confirmation, funds are escrowed on-chain and the request remains in a Pending Fill state with live progress tracking.
4. Once the request reaches 100% fill, it automatically executes at confirmed terms and moves to active/live status.
5. If the request fails to reach full fill prior to the deadline, all committed funds are automatically returned to participants.
6. Commitments outside defined limits are rejected; edited or cancelled requests trigger immediate refund processing. Optional pre-fill withdrawal is available, subject to applicable network transaction fees.

#### C) Private Requests

Participants may designate a service request as Private, removing it from the public Processing Board. Private requests may be shared via direct invite links, enabling specifically invited participants to join while preserving the same on-chain execution logic and settlement guarantees applicable to public requests.

## 5.4. Revenue Distribution Model

To maintain a self-sustaining ecosystem and fund core operations, BetsWave charges a fixed 1% Service Processing Fee on all service transactions. Service Processing Fee revenue is redistributed across the platform ecosystem in accordance with the following allocation model. These ratios are subject to modification through the community governance process, and changes will be communicated through appropriate platform channels.

| Allocation | Percentage | Purpose |
|------------|-----------|---------|
| Token Burn | 51% | Permanently removed from circulation (deflationary supply mechanism) |
| Standard Processing Pool | 14% | Contributed to Standard Processing Pool liquidity reserve |
| Community & Staking | 10% | Community Incentive programs and staking pool distributions |
| Treasury & Operations | 25% | Treasury management and operational expenditures |

> Revenue distribution ratios are subject to modification through the community governance process. These allocations describe current design intentions and do not create any contractual entitlement to receive any particular distribution. Changes will be announced through official platform communication channels.