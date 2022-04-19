# SmartCustody v2.0

v2.0 of the Smart Custody book will generally expand the book to include new hardware solutions and also to provide new solutions for multisignatures.

## New Topics

**New Risk-Modeling.**

* Torino Scale as another 5-point scale
* Consider showing a color version of risk graph for green/yellow/red in different regions

**New Adversaries.** Rollup Attack: you attack a social network of peers using secrets and use that social network to make it easier to attack the rest of the social network.

AirDrop Scam: https://www.bsc.news/post/airdrop-scams-continue-to-surface-on-layer-1-defi-networks (a new type of social engineering, or something new entirely).

DoS: Possibly related to Censorship. See https://github.com/btcpayserver/btcpayserver/issues/3190

Centralization: This is a new adversary, currently missing from #SmartCustody, and more problematic on Ethereum. A single private key tends to be used to unlock personally held funds, to access smart contracts, and to create signatures. If that private key is lost or stolen then all functionality goes with it.

Cost: A close kin to Convenience, this new adversary arises when the monetary cost of security is too high to adopt it. Again, Ethereum really shows off the problem because it can cost $100 to move funds to cold storage due to astronomical gas fees.

Exposure: This is a primarily secondary adversary, something that can arise from using cryptocurrency, without necesarily endangering your cryptocurrency. It's when your personal information gets revealed. NFTs show how this can happen, since the URL of the NFT can track your IP address, among other things.

Boundary Breaker: See Below

Who Knows, But a Big Hack: https://www.theblockcrypto.com/post/139761/axie-infinitys-ethereum-sidechain-ronin-hit-by-600-million-exploit (four validators subject to same attacks; 1 that signed for free)

**New Hardware Wallets.** A new Chapter Three will offer variable options for Hardware Wallets, currently planned to include KeepKey, Ledger, and Trezor. These will cleanly slot into the middle of the cold-storage procedure. A short article will also discuss deciding among the hardware wallets. This will also require a revision of the scenario section, which will allow us to more cleanly divide the core scenario, the Hardware Wallets, and the optional steps.

**New Multisignatures.** A new PART will discuss multisignatures, first detailing why they're important and how to use them, then providing a variant of the core procedure for using multisignatures in a self-sovereign methodology. An open question for this section is: do we present it as a modification to the base scenario, or as its own scenario; this question will resolve itself as we write the scenario.

**Fidicuiary Multisignatures.** Finally, we combine the lessons learned above to offer our first complete fiduciary scenario, using multisignatures to ensure separation of duties.

**Other New Technologies.** Consider incorporating other #SC articles written since 1.0

***Multisigs:***
* [Designing Multisig for Indepedence & Resilience](https://github.com/BlockchainCommons/SmartCustody/blob/master/Docs/Multisig.md) (March 2021) - Design process & sample multisigs (released).

***SSKR Shares:***
* [Designing SSKR Share Scenarios](https://github.com/BlockchainCommons/SmartCustody/blob/master/Docs/SSKR-Sharing.md) (August 2021) - How to manage SSKR shares (preliminary)
* [The Dangers of Secret-Sharing Schemes](https://github.com/BlockchainCommons/SmartCustody/blob/master/Docs/SSKR-Dangers.md) (August 2021) - How secret-sharing can be subverted (preliminary)

***Timelocks:***
* [Using Timelocks to Protect Digital Assets](https://github.com/BlockchainCommons/SmartCustody/blob/master/Docs/Timelocks.md) (July 2021) - Using Timelocks (very preliminary).


**New Methods of Thinking About Attackers.**

Attack Trees [2021-12-13]
- [Academic: Attack Trees - Schneier on Security](https://www.schneier.com/academic/archives/1999/12/attack_trees.html)
- [Designing Trusted Services with Group Controls](https://www.fon.hum.uva.nl/rob/Courses/InformationInSpeech/CDROM/Literature/LOTwinterschool2006/szabo.best.vwh.net/groupcontrols.html)
- [Attack tree - Wikipedia](https://en.wikipedia.org/wiki/Attack_tree)

Motivations [2021-12-13]
- [Understanding cyber attacker motivations to best apply controls | AT&T Cybersecurity](https://cybersecurity.att.com/blogs/security-essentials/understanding-cyber-attacker-motivations-to-best-apply-controls)

**How Do You Think About Smart Custody Designs?**

## Updated Table of Contents

Obviously this table of contents is subject to change. In particular, wer're considering moving the risk modeling to later in the book to make it more approachable.

We've also added some new potential topics since writing this ToC, including other new technologies (comprising several extensive articles) and new methods of thinking about attackers.

```
FRONT MATTER

i. Disclaimer
ii. Credits
  a. The #SmartCustody Team
  b. Copyright & Contributing
  c. Sponsors
iii. Foreword
  a. The Key Management of Digital Assets
  b. Preface to the Book
    1. Why Cold Storage?
    2. About the #SmartCustody Project
iv. Introduction: The Power of Randomness
  a. Introduction to Randomness
  b. The Danger of Randomness
  c. The Core of Custody

PART ONE: RISK MODELING

I. Chapter One: Risk Modeling
  A. Introduction to Risk Modeling
  B. Section I: Asset Characterization
  C. Section II: Risk Characterization
  D. Section III: Risk Resolution
  E. Section IV: Process Repetition
  F. Summary

PART TWO: BASIC SCENARIO BUILDING

II. Storage Scenarios **REVISED**
  A. Introduction to the Custody Scenarios **REVISED**
  B. Procedures **EXPANDED**

III. Chapter Two: Cold Storage Self-Custody Scenario **REVISED**
  A. Introduction to the Cold Storage Self-Custody Scenario
  B. The Basic Procedure

III. Chapter Three: Hardware Wallets **NEW**
  A. Introduction to Hardware Wallets **NEW**
  B. KeepKey Procedures **NEW**
  C. Ledger Procedures **NEW**
  D. Trezor Procedures **NEW**

IV. Chapter Four: Other Alternatives **REVISED**
  A. Introduction to Other Alternatives **REVISED**
  B. Alternative Scenarios **REVISED**
  C. Optional Steps **REVISED**

PART THREE: ADVERSARIAL ANALYSIS

V. Chapter Five: Adversaries
  A. Introduction to Adversaries
  B. Category: Loss by Acts of God
  C. Category: Loss by Computer Error
  D. Category: Loss by Crime, Theft
  E. Category: Loss by Crime, Other Attacks
  F. Category: Loss by Government
  G. Category: Loss by Mistakes
  H. Category: Privacy-related Problems

PART FOUR: MULTISIGNATURE USAGE **NEW**

VI. Chapter Six: Multisignatures **NEW**
  A. Introduction to Multisignatures **NEW**
  B. Multisignature Creation **NEW**
  C. Multisignature Spending **NEW**
VII. Chapter Seven: Self-Sovereign Multisignature Scenario* **NEW**
  A. Introduction to the Self-Soveriegn Multisignature Scenario **NEW**
  B. The Multi-sig Scenario **NEW**

PART FIVE: FIDUCIARY DUTIES

VIII. Chapter Eight: Digital Custodianship Responsibilities
  A. Introduction to Fiduciary Responsibilities
  B. Best Practices of Digital Custodianship
  C. References
IX. Chapter Nine: The Frank Family Fund Example
  A. Introduction to the Frank Family Fund
  B. Section I: Asset Characterization
  C. Section II: Risk Characterization
  D. Section III: Risk Resolution
  E. Section IV: Process Repetition
X. Chapter Ten: Fiduciary Multisignature Scenario **NEW**
  A. Introduction to the Fiduciary Multisignature Scenario **NEW**
  B. The Fiduciary Scenario **NEW**

APPENDICES

i. Appendix I: Sample Digital Assets Letter
ii. Author Bios
iii. Blockchain Commons Links
```

## Identity Adversaries

We've done some work on adversaries that are primarily related to identity. We may want to do more on these and also do want to see which are related to the wider world of digital assets.

**Boundary Breaker:**

Assumptions:
* Public goods often have boundaries (in particular to keep the viability of the system intact, see Ostrom)
* Established boundaries are often perceived as unfair.
* We don’t want to destroy the value of the system, we want part of it.
* May perceive any legitimate means of changing the boundary as not possible, too slow, too expensive, etc. * Related systems may be used for leverage.
Motivation:
* Because of my lack of agreement on the boundaries of membership, I desire to change/subvert the boundaries (to include me or others like me, or exclude someone else).
* Because the process to change boundaries is “unfair” (has favoritism), I desire to change/subvert the process.
* Because I don’t have access to process to change the boundaries, break the process.

## Open Questions

Has BCC created any tools such as LetheKit that would be worthwhile to integrate, or is that too specific?

## Other Sources

These are other sources that might provide insights into adversaries

* [Casa Threat Listing](https://docs.keys.casa/wealth-security-protocol/)
* [Actual Kidnapping Example](https://www.elespanol.com/espana/20211103/fundador-tuenti-denuncia-secuestro-manos-millones-bitcoin/624188600_0.html?utm_medium=Social&utm_campaign=Echobox&utm_source=Twitter#Echobox=1635924343)
* [Trezor Hack](https://www.theverge.com/2022/1/24/22898712/crypto-hardware-wallet-hacking-lost-bitcoin-ethereum-nft) — PIN loss case study, "Hardware Hack" adversary?
* [Mars Stealer Hack](https://cointelegraph.com/news/hodlers-beware-new-malware-targets-metamask-and-40-other-crypto-wallets) and [also](https://cryptobriefing.com/mars-stealer-can-grab-your-crypto/) with [specifics](https://3xp0rt.com/posts/mars-stealer).
* [Metamask Social Engineering](https://twitter.com/serpent/status/1515545806857990149?s=21&t=JjMXGdO1X1VCl0_B4SUcVQ)

## Support #SmartCustody 2.0

If you would like to support the development of SmartCustody v2.0, then please [contribute to our BTCPay](https://btcpay.blockchaincommons.com/). We are looking to raise 5 Bitcoins to allow the redevelopment and expansion of the book.
