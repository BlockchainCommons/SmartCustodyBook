# Overview of Digital Custodianship Responsibilities

_Caring for other peoples' assets_

***Version: 2018-09-21 1.0.0***

## Introduction to Fiduciary Responsibilities

Digital currency is a groundbreaking new asset class that allows for easier individual control and management of assets than previous classes. This has created a somewhat *laissez faire* attitude toward digital currency custodianship, even when it extends from personal ownership to custodianship of digital assets for family, friends, trusts, or customers. This is a grave mistake because digital custodianship requires the same high levels of faith, trust, and protection as any
other asset that one might oversee and safeguard.

Generally, digital custodianship falls under ***fiduciary law***. This is a lesser know type of law that rises to preeminence when one person (a fiduciary) holds some position of trust for another person (a client), particular when the fiduciary is holding money or property. In the case of cryptocurrency, a fiduciary holds digital assets for a client. Fiduciary law creates specific responsibilities that cannot be waived by *either party* even under a contract.

When a trustee holds a client’s digital assets they must uphold a ***fiduciary duty*** in regard to those assets, acting in the *best interest* of the owner. The specifics of these duties vary from jurisdiction to jurisdiction, but it generally requires the “highest standard of care”. Wikipedia offers a more extensive definition: *“When a fiduciary duty is imposed, equity requires a different, stricter ... standard of behavior than the comparable tortious duty of care at common law.”*

These duties may include “duties of care”, where the fiduciary is required to keep himself informed for the benefit of his client, and “duties of loyalty”, where the fiduciary must put the interests of his client foremost and cannot act in his own self-interest. Duties of confidentiality, disclosure, good faith, and prudence may also be recognized. The [*2003 SEC regulations*](https://www.sec.gov/rules/final/ia-2176.htm) are likely to apply most directly to the fiduciary duties of digital custodians.

## Best Practices of Digital Custodianship

The wider financial industry has long practiced and defined the “different, stricter” requirements of fiduciary duty. One requirement regularly rises to the forefront and should also be considered a minimum level of care to support the fiduciary duty required by digital custodianship:

***Dual control*** requires that two people be present for certain sensitive financial operations. In the classic financial world, two employees might exercise dual control when transferring a cash drawer, while a banker and customer might exercise dual control to open a safety deposit box. In some cases, one of the controllers may need to be from outside the company, such as an auditor.

For digital custodianship, dual control can easily be represented with a multi-sig, which requires two or more people to sign off on cryptocurrency transactions. If a custodian is actively investing and transferring digital currencies, then a multi-sig could require the signatures of two people at the investment house, while if it’s simply holding the cryptocurrency, it could require a signature of a custodian and their client.

A 2-of-2 multi-sig is the most obvious analogue to a physical dual-control scenario, but increasing the number of possible signers (without increasing the number of required signers) can reduce cryptocurrency’s issues of key fragility. Generally, increasing the number of required signers will increase the security at the cost of fragility while increasing the the number of possible signers will decrease the fragility at the cost of security. A 2-of-3 multi-sig may be a good compromise, where any two people from a group of three can sign off on transactions. (Shamir secret sharing is another technical option for dual control, but is generally considered less secure due, ironically, to its ease of implementation.)

Dual control in digital currency can also go beyond these simple technical means. It can (and should) be baked into other sensitive areas, such as the creation of scripts, which should be checked by at least two engineers as a general policy.

Dual control is built on the larger concept of ***separation of duties***, which generally says that that different people should be involved in different parts of a transaction. This goes beyond simply protecting the most sensitive financial operations; it should be built into any digital custodianship as a best practice for all phases of operation.

Separation (or segregation) of duties can be best achieved by breaking down the lifespan of digital custodianship into its constituent parts. This includes phases like intake of fiat currency, intake of cryptocurrency, purchase of digital currency, sale of digital currency, transfer of digital currency, and transfer of fiat currency. Having different people responsible for some or all of these duties helps to ensure that neither fraud, incompetence, or accident is likely to impact digital currency custodianship.

### Additional Requirements for High Value Accounts

Additional fiduciary requirements and responsibilities may apply when higher values of digital assets are held by a custodian. The SEC requires that the traditional Registered Investment Advisor (RIA) model use an external qualified custodian to hold amounts larger than \$150 million. It remains unclear if these regulations apply to cryptocurrencies, as the SEC has said that Bitcoin and Ether are not securities.

However, digital custodians should carefully consider and reconsider their setup to see if a qualified custodian is suggested if they reach a \$150 million plateau of value, which is very easy given the rapid upswings in cryptocurrency price that have occurred in the past. They should also keep abreast of local laws, state laws, or international laws that might regulate custodianship at certain high-value breakpoints.

## References

“Breach of Fiduciary Duty Law and Legal Definition”. USLegal.com.
[*https://definitions.uslegal.com/b/breach-of-fiduciary-duty*](https://definitions.uslegal.com/b/breach-of-fiduciary-duty)

“Custody: Uncharted Waters for Digital Assets”. FinOps Report.
[*https://finops.co/investors/custody-unchartered-waters-for-digital-assets/*](https://finops.co/investors/custody-unchartered-waters-for-digital-assets/)

“Custody of Funds or Securities of Clients by Investment Advisers”. SEC.
[*https://www.sec.gov/rules/final/ia-2176.htm*](https://www.sec.gov/rules/final/ia-2176.htm)

“Dual Control”. Money Services Business.
[*http://moneyservicesbusiness.com/risk-mgt/dual-control/*](http://moneyservicesbusiness.com/risk-mgt/dual-control/)

“Fiduciary”. Wikipedia.
[*https://ipfs.io/ipfs/QmXoypizjW3WknFiJnKLwHCnL72vedxjQkDDP1mXWo6uco/wiki/Fiduciary\_duty.html*](https://ipfs.io/ipfs/QmXoypizjW3WknFiJnKLwHCnL72vedxjQkDDP1mXWo6uco/wiki/Fiduciary_duty.html)

“Fiduciary Duty”. Cornell Law School: Legal information institute.
[*https://www.law.cornell.edu/wex/fiduciary\_duty*](https://www.law.cornell.edu/wex/fiduciary_duty)

“Separation of Duties”. University of Washington.
[*https://finance.uw.edu/fr/internal-controls/separation-of-duties*](https://finance.uw.edu/fr/internal-controls/separation-of-duties)

“URGENT: Fragmented Backups Vulnerability”. Bitcoin Armoy.
[*https://btcarmory.com/fragmented-backup-vuln/*](https://btcarmory.com/fragmented-backup-vuln/)
