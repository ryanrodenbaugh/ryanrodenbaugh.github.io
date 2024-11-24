---
layout: post
title: "RWA Protocol Fee Comparison: A Deep Dive into DeFi Credit Protocols"
date: 2023-02-09
category: crypto
---

*This post originally appeared on the [Wallfacer Labs Substack](https://wallfacerlabs.substack.com/p/comparing-fees-of-credit-protocols)*

## Intro

As yields in DeFi have been squashed, market participants have begun looking for sources of yield off-chain. As a result, "real-world assets" (RWA) have become an area of increasing focus within crypto markets with teams looking to bring off-chain asset exposure on-chain.

RWA protocols have the opportunity to bridge the gap between off-chain opportunities and on-chain participants. Many believe that bringing products like treasury bills or investment-grade bonds on-chain will increase the use cases and sustainability of crypto.

In the excitement about the financial products RWA protocols can offer, few are asking how sustainable the underlying protocols are themselves.

In this post, we will look at the fee models used by Centrifuge, TrueFi, Maple, Goldfinch, and Credix and compare the different models.

## Summary of Fee Types

There are 3 types of fees common in credit protocols:

- Origination fees (paid at the start of a loan)
- Repayment/performance fees (paid at the end of a loan as a % of interest generated)
- Platform fees (% of AUM) (paid continuously through the life of a loan)

## Protocol Deep Dives

### Centrifuge

Centrifuge was the first protocol to enter this market, currently has the largest TVL, and supports the most complex deal types. All the while, they have not been charging pool fees.

Beginning mid-2022, but really coming to a head in December of 2022, the Centrifuge community put out a forum post looking to enact fees, seeking comments on models that would work best for the protocol. There was a lot of good conversation from their originators who seemed to generally coalesce around the idea that issuers (not lenders or borrowers) should be charged an AUM-based fee.

Benchmarking against traditional finance, ImdioR stated that:

> Securitizations frequently cost between 0.5% and 2% annually in fees charged by various intermediaries (fund administration, payment agents, calculation agents, etc.). The Centrifuge will replace the vast majority of these intermediaries with the lowest fee

Using the data above, in a follow-up forum post and call in January of 2023, Centrifuge governance facilitator, ImdioR, made a proposal to implement a 0.4% (40 bps) fee on all outstanding capital in pools on Centrifuge Chain. The fee would accrue in real-time and be drawn on each withdrawal or repayment made by the issuer.

Kevin Chan of Blocktower made two insightful comments:

1. In traditional markets, fees tend to be charged to investors and issuers, but ultimately higher fees flow to the end borrowers.
2. Centrifuge should set a fee schedule that encourages early adoption and long-term growth. Basically using fee thresholds to encourage early use and continued growth on the platform (i.e., avoid the issue of fees becoming overly extractive for large managers).

Most issuers said that a 40 bps fee on outstanding loans was very fair. Centrifuge has moved the current fee proposal forward and is currently reviewing comments on the technical proposal.

At the time of writing (February 9, 2023), the proposal is currently being put to a vote and is set to be decided by February 15. It is not clear how fast this could be implemented. Additionally, the fees would only apply to pools on Centrifuge's parachain. The entirety of Centrifuge's current TVL ($145,074,182) lives on Ethereum (on Tinlake) and thus the 40bps would not be applied to those pools. As an approximation though, if the 40bps fee were to be applied to Centrifuge's existing pools (it is not) that would yield ~$580k of annual revenues.

### TrueFi

TrueFi has already implemented a very similar model for fees. But, it took the protocol some time to get there. Today, TrueFi's protocol fee is 50 basis points (0.50%) per annum, accrued continuously and paid periodically by the portfolio smart contract.

Previously, TrueFi charged 0.25% origination fees but got rid of them shortly after launch for a number of reasons including that origination fees decrease the "headline rate" shown to lenders and depending on how it's calculated can disincentivize short-term loans.

As one of TrueFi's borrowers said at the time:

> Origination just feels like another attempt to port over some shitty legacy concept from tradfi that really doesn't need to exist. "Reduce complexity, increase transparency".

As a result, TrueFi moved in the direction of 'performance fees' where the protocol would take 10% of the total interest generated.

That model was also eventually scrapped as TrueFi began to move towards its current marketplace model, where portfolio managers can launch their own funds using TrueFi infrastructure. Given TrueFi wants to accommodate high-quality, lower-return strategies (US Treasuries, investment grade bonds, etc.) as well as higher-yielding strategies (EM credit, etc.), it needed a model that was non-prohibitive, enabled lower-yield opportunities, and would not have to be negotiated on a pool-by-pool basis.

As a result, TrueFi introduced a third model of fees, a re-attempt to improve origination fees. The early thinking was to pay fees upfront as a % of the principal on each loan made, in part because using performance fees on longer-duration loans means payments to the protocol would be far out in the future. This fee would be paid by lenders, not by the borrower.

But this turned out to be tricky to implement, as paying the fees upfront led to costs being disproportionately taken on by lenders who were in the pool at the time of origination (vs. lenders who join after a loan is originated). TrueFi refunded fees to affected users (see [Alameda portfolios fee issue: Post mortem & proposed resolution]) and went back to the drawing board.

Finally, in September 2022 TrueFi landed where it is today, where TrueFi collects an annualized fee of 50 BPS (0.5%) on each dollar stored in active TrueFi portfolios.

In this design, fees accrued by a portfolio for a single day of usage would cost lenders 0.0013% (0.5% divided by 365 days). This change is in direct response to feedback from lenders and portfolio managers, and it offers the following benefits:

- The fee is proportional to the usage of the protocol, compared to TrueFi's previous flat fee
- Fees are not incurred during the capital formation period
- Accounting is simplified, and books no longer reflect a sudden drop in asset value
- Funds can move through TrueFi opportunities without incurring additional exit fees

Though 10 bps higher, this fee model is nearly identical to what Centrifuge proposed in January of 2023.

### Maple Finance

When Maple launched in the summer of 2021, it began by allowing pool delegates to charge establishment (origination) and ongoing (performance) fees. These mirrored the fees that the protocol charged.

Today (February 2023), Maple charges two types of fees: recurring fees, and performance fees. Maple moved away from origination fees in September 2022 (when they moved to recurring borrower fees).

In Maple's newest pool managed by AQRU there are:

**Total borrower fees are 50bps:**
- 10 bps to pool delegate
- 40 bps to Maple Treasury

**Total management fees (performance fees) are 15%:**
- 12.50% paid to the pool delegate
- 2.5% paid to the protocol

In earlier Maple pools, such as the "M11 Credit - wETH pool", borrower fees are 99 bps. Taking the Flow Traders loan initiated on November 23, 2022 (and paid back on December 23, 2022) there were:

**Total borrower fees of 99 bps:**
- 33 bps to pool delegate
- 66 bps to the Maple Treasury

**Total management fees (performance fees) of 16%:**
- 2.5% to the protocol
- 13.5% to the pool delegate

For most of Maple's loans, it seems to be the case they had a fixed origination fee of 99 bps (split ⅔ to treasury and ⅓ to delegate) and a performance fee of 20% (split 50/50).

### Credix + Goldfinch

From a fee perspective, Credix and Goldfinch are identical(ish). They both take a 10% 'performance fee' on capital repaid.

Both protocols enable tranching (a topic for another post as all these protocols handle it very differently). Both Credix and Goldfinch charge this 10% performance fee across all tranches.

In Goldfinch, there is also a 0.5% withdrawal fee for redeeming FIDU for USDC on Goldfinch, contributing funding to the Goldfinch treasury. The exit/withdrawal fee structure is unique to Goldfinch and makes up a relatively small percentage of their total revenues today (<10%).

It's unclear whether the exit fee structure is a sustainable long-term model. Yearn long ago removed withdrawal fees, noting that the fees:
- Made it harder to build third-party integrations
- Created a bad UX for depositors
- Misaligned incentives by rewarding Yearn during times of capital flight

## Conclusion

From a historical perspective, this sector has generated just about $10mm in total revenues for their respective treasuries and token holders.

Per Dune:
- Maple has generated $4,775,696
- TrueFi has generated $3,353,407
- Goldfinch has generated $1,601,229
- Credix we think has generated $222,130 (based on 2,221,306 USDC being repaid)
- Centrifuge is just now evaluating turning on fees

Unless protocols are going to focus only on 'high octane' credit opportunities (lending to trading firms, emerging market credit) that allow for higher performance fees, it's likely we will see increasing fee compression as protocols compete to attract the best managers.

As we can see in the chart below, a typical $10mm 180-day loan generates somewhere between $20-$50k in fees for these protocols. Given that we don't expect fee margins to expand significantly from where they are today, credit protocols will need loan volumes in the billions of dollars to achieve long-term sustainability.

Balancing protocol fees, manager fees, and token holders have also proven challenging for many of these protocols. To date, no protocol has an ideal solution:

- TrueFi used to pay out the entirety of its generated revenues to token holders. TrueFi has since voted to divert those fees to its treasury instead to build up its balance sheet.
- Maple stated they would utilize an xToken model, using 50% of its establishment fee revenues to buy MPL and return it to stakers. Per on