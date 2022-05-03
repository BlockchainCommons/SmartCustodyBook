# SmartCustody v2.0

v2.0 of the Smart Custody book will generally expand the book to include new hardware solutions and also to provide new solutions for multisignatures.

## New Table of Contents

## Updated Table of Contents

Our original table-of-contents for a 2.0 is somewhat dated, as we've since written four new articles and a new scenario, some or all of which will be incorporated into the book, and also identified a lot of other potential material. We've also largely decided to push risk modeling back in the book, to make the introduction to smart custody less intimidating. Nonetheless, this table of contents has some large scale thoughts on new content for 2.0.

```
FRONT MATTER

i. Disclaimer
ii. Credits
  a. The #SmartCustody Team
  b. Copyright & Contributing
  c. Sponsors
iii. Foreword
  a. The Key Management of Digital Assets
iv. Preface to the Book
  a. About the #SmartCustody Project
iv. Introduction: The Power of Randomness
  a. Introduction to Randomness
  b. The Danger of Randomness
  c. The Core of Custody
v. Introduction: The Power of Checklists **NEW**
  a. Introduction to Self-Custody **NEW**
  b. Introduction to the Custody Scenarios **REVISED**
  c. How the Scenarios Were Created **REVISED FROM ARTICLE**
  d. Procedures **EXPANDED**

PART ONE: COLD CUSTODY SCENARIO BUILDING

  A. Why to Use Cold Storage
  
II. Chapter Two: Cold Storage Self-Custody Scenario **REVISED**
  A. Introduction to the Cold Storage Self-Custody Scenario
  B. Why Cold Storage?
  C. The Basic Procedure
  D. Optional Steps
  E. Alternative Procedures
  F. SPOCs & SPOFs in this Scenario **NEW**

III. Chapter Three: Hardware Wallets **NEW**
  A. Introduction to Hardware Wallets **NEW**
     1. Two Generations **NEW**
  B. Alternate Trezor Procedures **NEW**

PART TWO: MULTISIG SCENARIO BUILDING

  A. Why to Use Multisig

IV. Chapter Four: Multisig Self-Custody Scenario **NEW FROM ARTICLE**
  A. Introduction to the Multisig Self-Custody Scenario
  B. Why Multisig?
  C. The Basic Procedure
  D. Optional Steps
  E. Alternative Hardware Wallet Procedures
  F. SPOCs & SPOFs in this Scenario

V. Chapter Five: Designing Multisig Scenarios **NEW FROM ARTICLE**
  A. Multisig Design Article: https://github.com/BlockchainCommons/SmartCustody/blob/master/Docs/Multisig.md **REVISED TO FIT**

VI. Chapter Six: Designing SSKR Scenarios **NEW FROM ARTICLE**
  A. SSKR Design Article: https://github.com/BlockchainCommons/SmartCustody/blob/master/Docs/SSKR-Sharing.md **REVISED TO FIT**
  B. The Dangers of SSKR: https://github.com/BlockchainCommons/SmartCustody/blob/master/Docs/SSKR-Dangers.md **REVISED TO FIT**
  
PART THREE: RISK MODELING

VII. Chapter Seven: Risk Modeling
  A. Introduction to Risk Modeling
  B. Section I: Asset Characterization
  C. Section II: Risk Characterization
  D. Section III: Risk Resolution
  E. Section IV: Process Repetition
  F. Summary
VIII. Chapter Eight: Adversaries
  A. Introduction to Adversaries
  B. Category: Loss by Acts of God
  C. Category: Loss by Computer Error
  D. Category: Loss by Crime, Theft
  E. Category: Loss by Crime, Other Attacks
  F. Category: Loss by Government
  G. Category: Loss by Mistakes
  H. Category: Privacy-related Problems
VIIIa. Chapter Eight-and-a-Half: Alternative Risk Models [Optional]

PART FOUR: FIDUCIARY DUTIES

IX. Chapter Nine: Digital Custodianship Responsibilities
  A. Introduction to Fiduciary Responsibilities
  B. Best Practices of Digital Custodianship
  C. Multisig Procedures **NEW**
  D. References
X. Chapter Ten: The Frank Family Fund Example
  A. Introduction to the Frank Family Fund
  B. Section I: Asset Characterization
  C. Section II: Risk Characterization
  D. Section III: Risk Resolution
  E. Section IV: Process Repetition

PART FIVE: THE FUTURE OF SMARTCUSTODY

XI. New Technologies on the Horizon **NEW**
  A. Taproot
  B. Schnoor
XII. New Technology Spotlight: Timelocks **ADAPTED FROM ARTICLE**
  A. Paper: https://github.com/BlockchainCommons/Gordian/blob/master/Docs/Timelocks.md
  B. Mori-cli Prototype: https://github.com/BlockchainCommons/mori-cli

APPENDICES

i. Appendix I: Preserving Assets for Yoru Heirs
ii. Appendix II: Sample Digital Assets Letter
iii. Author Bios
iv. Blockchain Commons Links
```

## Updated Material

The following Additional material will expand current chapters.

### Chapter Seven: Risk Modeling

* Mention Torino Scale as another 5-point scale
* Consider showing a color version of risk graph for green/yellow/red in different regions

### Chapter Eight: Adversaries

#### New Adversaries

The following adversaries will all be considered for inclusion:

* **AirDrop Scam:** https://www.bsc.news/post/airdrop-scams-continue-to-surface-on-layer-1-defi-networks (a new type of social engineering, or something new entirely).
* **Boundary Breaker:** See Below
* **Centralization:** This is a new adversary, currently missing from #SmartCustody, and more problematic on Ethereum. A single private key tends to be used to unlock personally held funds, to access smart contracts, and to create signatures. If that private key is lost or stolen then all functionality goes with it.
   * This was primarily a centralization hack, further empowered by convenience: https://www.theblockcrypto.com/post/139761/axie-infinitys-ethereum-sidechain-ronin-hit-by-600-million-exploit (four validators subject to same attacks; 1 that signed for free)
* **Cost:** A close kin to Convenience, this new adversary arises when the monetary cost of security is too high to adopt it. Again, Ethereum really shows off the problem because it can cost $100 to move funds to cold storage due to astronomical gas fees.
* **DoS:** Possibly related to Censorship. See https://github.com/btcpayserver/btcpayserver/issues/3190
* **Exposure:** This is a primarily secondary adversary, something that can arise from using cryptocurrency, without necesarily endangering your cryptocurrency. It's when your personal information gets revealed. NFTs show how this can happen, since the URL of the NFT can track your IP address, among other things.
* **Rollup Attack:** you attack a social network of peers using secrets and use that social network to make it easier to attack the rest of the social network.

#### Hacks that May Be Examples or Adversaries

The following hacks may reveal additional adversaries, or just be good examples for existing ones.

* [Actual Kidnapping Example](https://www.elespanol.com/espana/20211103/fundador-tuenti-denuncia-secuestro-manos-millones-bitcoin/624188600_0.html?utm_medium=Social&utm_campaign=Echobox&utm_source=Twitter#Echobox=1635924343)
* [Trezor Hack](https://www.theverge.com/2022/1/24/22898712/crypto-hardware-wallet-hacking-lost-bitcoin-ethereum-nft) — PIN loss case study, "Hardware Hack" adversary?
* [Mars Stealer Hack](https://cointelegraph.com/news/hodlers-beware-new-malware-targets-metamask-and-40-other-crypto-wallets) and [also](https://cryptobriefing.com/mars-stealer-can-grab-your-crypto/) with [specifics](https://3xp0rt.com/posts/mars-stealer).
* [Metamask Social Engineering](https://twitter.com/serpent/status/1515545806857990149?s=21&t=JjMXGdO1X1VCl0_B4SUcVQ)

#### Boundary Breaker

**Assumptions:**

* Public goods often have boundaries (in particular to keep the viability of the system intact, see Ostrom)
* Established boundaries are often perceived as unfair.
* We don’t want to destroy the value of the system, we want part of it.
* May perceive any legitimate means of changing the boundary as not possible, too slow, too expensive, etc. * Related systems may be used for leverage.

**Motivation:**

* Because of my lack of agreement on the boundaries of membership, I desire to change/subvert the boundaries (to include me or others like me, or exclude someone else).
* Because the process to change boundaries is “unfair” (has favoritism), I desire to change/subvert the process.
* Because I don’t have access to process to change the boundaries, break the process.

#### Identity Adversaries

More broadly: we've done some work on adversaries that are primarily related to identity. We may want to do more on these and also do want to see which are related to the wider world of digital assets.

#### Alternative Methods of Thinking About Attackers

These articles should be considered for whether they deserve attention on their own, slight mentions, footnotes, or nothing. If there's sufficient material, they could lead to the optional Chapter 8.5 mentioned.

* Attack Tree
   - [Academic: Attack Trees - Schneier on Security](https://www.schneier.com/academic/archives/1999/12/attack_trees.html)
   - [Designing Trusted Services with Group Controls](https://www.fon.hum.uva.nl/rob/Courses/InformationInSpeech/CDROM/Literature/LOTwinterschool2006/szabo.best.vwh.net/groupcontrols.html)
   - [Attack tree - Wikipedia](https://en.wikipedia.org/wiki/Attack_tree)
* Motivations
- [Understanding cyber attacker motivations to best apply controls | AT&T Cybersecurity](https://cybersecurity.att.com/blogs/security-essentials/understanding-cyber-attacker-motivations-to-best-apply-controls)
* [Casa Threat Listing](https://docs.keys.casa/wealth-security-protocol/)

### Open Questions

Has BCC created any tools such as LetheKit that would be worthwhile to integrate, or is that too specific?

## Support #SmartCustody 2.0

If you would like to support the development of SmartCustody v2.0, then please [contribute to our BTCPay](https://btcpay.blockchaincommons.com/). We are looking to raise 5 Bitcoins to allow the redevelopment and expansion of the book.
