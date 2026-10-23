# Audit Reports: Côme du Crest

Smart contract security researcher. This repository collects a selection of public audit reports from my work at Gnosis Ltd (2023–2026) and my independent engagements.

**45 public reports · 2024–2026 · 12 High and 17 Medium severity findings**

Clients and projects include Gnosis (Gnosis Pay, Circles, Zodiac, Gnosis Chain bridges), CoW Protocol, Midas, Wildcat, Acre, HOPR, karpatkey and Balmy.

Most of my audit work (80+ audits at Gnosis, plus independent engagements) is under NDA and can't be published. Additional samples and references are available on request.

Contact: come.ducrest@gmail.com · [Sherlock profile](https://audits.sherlock.xyz/watson/cducrest-brainbot)

---

## Start here

If you only have a few minutes, these reports are the most representative:

| Report | Date | Why read it |
|---|---|---|
| [HOPR](hopr.pdf) | 2024-08 | High: incorrect elliptic curve addition (`ecAdd`) in the protocol's cryptographic primitives |
| [Acre](Acre.pdf) | 2025-08 | Bitcoin staking: 2 High (miscalculated migration of deposited assets, withdrawal queue stuck after upstream upgrade) |
| [Zodiac V3](zodiac-v3.pdf) | 2026-08 | Full audit of Gnosis Guild's Zodiac Roles v3 core: ABI decoding, condition evaluation, signature authentication (Med: signature manipulation) |
| [Midas Q2 Contracts](Midas-q2-contracts.pdf) | 2026-08 | Large RWA vault audit: 3 High (storage layout conflicts, zero average rate ignored, missing greenlist check on burn) |
| [Circles CMG](circles-cmg.pdf) | 2024-04 | High: anyone can break the group vault by sending worthless collateral |
| [Balmy Earn](balmy.pdf) | 2024-12 | Yield vaults and strategy connectors: High (performance fees on vault share deposits) and 3 Medium |
| [Circles LBP](circles-lbp.pdf) | 2025-01 | Balancer LBP and CoW Swap integration: 2 High (missing slippage protection) |
| [Flex Pool](flex-pool.pdf) | 2025-07 | Cross-chain solver liquidity pools integrating Across, CCTP and 1inch Fusion: 2 Medium |

---

## Full index

### Gnosis Chain infrastructure

| Report | Date | Notable findings |
|---|---|---|
| [Tokenbridge Fast Confirmation Rule](tokenbridge-fcr.pdf) | 2026-08 | Bridge validator client change (no issues) |
| [Tokenbridge Finality Check](tokenbridge-finality-check.pdf) | 2026-05 | Bridge validator client: beacon chain finality checks |
| [xDAI Bridge USDS Upgrade](bridge-USDS-upgrade3.pdf) | 2025-11 | Upgrade review following a signature replay issue |
| [Autoclaim Registry](ClaimRegistry.pdf) | 2025-03 | Med: batch claims break with claim action |
| [Balancer Claim](balancer-claim.pdf) | 2026-02 | Recovery of rescued funds after the 2025 Balancer hack |

### Zodiac / Safe modules

| Report | Date | Notable findings |
|---|---|---|
| [Zodiac V3](zodiac-v3.pdf) | 2026-08 | Med: authentication signature manipulation |
| [Zodiac Signature Patch](zodiac-signature-patch.pdf) | 2026-06 | Verification of patched Delay and Roles modifiers |
| [Auto Top-up Module](auto-top-up-module.pdf) | 2026-01 | Gnosis Pay / Gnosis App Safe module |

### Circles

| Report | Date | Notable findings |
|---|---|---|
| [Circles Multi Affiliate Group Registry](circles-multi-affiliate-group.pdf) | 2026-06 | No issues |
| [Circles Score Group](circles-score-group.pdf) | 2026-05 | High (unexploitable): policy tricked by sending the same collateral twice |
| [Circles Social Recovery](circles-social-recovery.pdf) | 2026-04 | Passkey recovery module: 2 Low |
| [Circles Payment Gateway](circles-payment-gateway.pdf) | 2025-12 | No issues |
| [Circles Base Group Mint Router](circles-base-group-mint-router.pdf) | 2025-10 | Group mint fix review |
| [Circles Token Offer](circles-token-offer.pdf) | 2025-09 | Low: incorrect time comparison |
| [Circles Invitation At Scale](circles-invitation-at-scale.pdf) | 2025-07 | Safe, 4337 and WebAuthn account creation |
| [Circles Invitation Escrow](circles-invitation-escrow.pdf) | 2025-06 | Low: unsafe assembly block |
| [Circles LBP Group](circles-lbp-group.pdf) | 2025-05 | Low: decimals scaling |
| [Circles Base Group](circles-base-group.pdf) | 2025-04 | No issues |
| [Circles LBP](circles-lbp.pdf) | 2025-01 | 2 High: missing slippage protection |
| [Circles CMG](circles-cmg.pdf) | 2024-04 | High: group vault can be broken |

### CoW Protocol

| Report | Date | Notable findings |
|---|---|---|
| [cow-shed Update](CoW-shed-update.pdf) | 2025-08 | Low: proxy storage layout inconsistency |
| [CoW AMM LP Oracle](cow-amm-lp-oracle.pdf) | 2025-04 | LP token fair pricing |
| [Flash Loan Router](CoW-flash-loan-router.pdf) | 2025-04 | No issues |

### Midas (RWA tokenization)

| Report | Date | Notable findings |
|---|---|---|
| [Midas Q2 Contracts](Midas-q2-contracts.pdf) | 2026-08 | 3 High, 1 Med |
| [Midas mWIN Update](Midas_mWIN_Update.pdf) | 2026-08 | Deployment and configuration review |
| [Midas mToken Min Balance](Midas-mToken-Min-Balance.pdf) | 2026-07 | Fee-after-burn bug found and fixed |
| [Midas Burner Fix](Midas_Burner_Fix.pdf) | 2026-07 | Cross-chain blacklist bypass fix |
| [Midas mWIN Deployment](Midas_mWIN_Deployment.pdf) | 2026-06 | On-chain deployment verification |
| [Midas Permissioned Token](Midas_Permissioned.pdf) | 2026-03 | Whitelist-only mToken |
| [Midas Vault Strategy Integration](Midas_Vault_Strategy_Integration.pdf) | 2026-03 | Aave, Morpho and mToken vaults |
| [Midas LayerZero and Axelar Integration](Midas_LZ_Axelar.pdf) | 2025-11 | Cross-chain bridging and composer |
| [Midas Max Supply](Midas_Max_Supply.pdf) | 2025-08 | High: storage layout incompatibility |
| [Midas Custom Recipient](Midas_Custom_Recipient.pdf) | 2025-07 | Vault updates |
| [Midas USTB](Midas_USTB.pdf) | 2025-06 | Med: redemption fee paid by protocol |
| [Midas](Midas_Audit.pdf) | 2024-08 | Initial full audit: 3 Med |

### Lending, vaults and DeFi

| Report | Date | Notable findings |
|---|---|---|
| [0xCurvy](0xCurvy.pdf) | 2026-08 | Med: `tx.origin` used for recovery |
| [Wildcat Collateral Contracts](Wildcat-collateral-contracts.pdf) | 2026-02 | Collateral liquidation for delinquent markets |
| [Wildcat ERC-4626 Wrapper](Wildcat4626Wrapper.pdf) | 2025-12 | Rounding and ERC-4626 compliance |
| [karpatkey Tokenized Fund: KpkShares](karpatkey-tokenized-fund-update.pdf) | 2025-11 | Med: performance fees can be disabled |
| [karpatkey Tokenized Fund](karpatkey-tokenized-fund.pdf) | 2024-10 | Med: EnumerableMap ordering assumption |
| [Acre](Acre.pdf) | 2025-08 | 2 High, 1 Med |
| [Flex Pool](flex-pool.pdf) | 2025-07 | 2 Med |
| [Balmy Earn](balmy.pdf) | 2024-12 | 1 High, 3 Med |

### HOPR

| Report | Date | Notable findings |
|---|---|---|
| [HOPR v4 Update](hopr_v4_update.pdf) | 2026-02 | Memory safety in node stake factory |
| [HOPR](hopr.pdf) | 2024-08 | High: incorrect `ecAdd` implementation |

---

## Competitive audits

Sherlock (2023–2024): 13 contests, 9 top-10 finishes, 5 podiums, 18 High severity findings. [Profile](https://audits.sherlock.xyz/watson/cducrest-brainbot)
