# ORCA Utility (VIP Membership NFTs)

ORCA NFTs are premium, non-transferable membership tokens designed for power users and long-term participants within the platform. ORCA memberships provide access to enhanced features, reduced fees, and exclusive experiences, while reinforcing sustained engagement and ecosystem alignment.

ORCA NFTs are issued in a fixed and capped supply to ensure scarcity and prevent uncontrolled membership inflation over time.

## Supply & Structure

- **Total Supply:** 100,000 ORCA NFTs (fixed)
- **Membership Model:** Annual subscription
- **Tier System:** 10 tiers, **10,000 NFTs per tier**
- **Pricing (Annual):**
  - Tier 1: **$10/year**
  - Tier 10: **$100/year**
- **NFT Standard:** **ERC-721 (soulbound, non-transferable)**
- **Metadata:** Stores membership tier and expiration timestamp on-chain

Each ORCA NFT represents an active membership for a defined period and automatically expires unless renewed.

## Fee Benefits

ORCA membership provides reduced platform fees compared to non-members:

- **Non-ORCA Members:** flat **1.5%** platform fee applied upfront
- **ORCA Members:** flat **0.5%** platform fee applied upfront

Fees are designed to be transparent and enforced on-chain.

## Access Control & Enforcement

All membership benefits are enforced through an on-chain access validation function that verifies:

- ORCA NFT ownership
- Membership tier
- Active (non-expired) status

Only wallets holding a valid ORCA NFT are permitted to access gated features, ensuring fair usage and preventing abuse.

## Design Rationale

The tiered, annual membership model is designed to:

- Encourage long-term participation over short-term speculation
- Align user incentives with platform growth and sustainability
- Provide predictable, recurring value to engaged users
- Maintain exclusivity through capped supply and non-transferability

By combining scarcity, utility, and time-based access, ORCA NFTs function as a sustainable membership layer rather than a speculative asset.
