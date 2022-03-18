# Zero Carbon Proposal (Template)

// To use this template, you will need to have determined:

// rNCT amount:

// 1. the amount of tons of CO2 that you want to offset - [tCO2]. For simplicity, we recommend you to collect validators self reported emissions with a survey and use: (known validators emissions + worst validator emission x # unknown validators) x safety factor. Usually on Cosmos a large validator emission might be around 5-10t per year, on average closer to 1t. The safety factor might be 2x-10x depending on your estimation. A more detailed methodology has been presented by Sarah Baxendell from Regen [https://docs.google.com/document/d/1H-w4dBc1Svcmw_fzEKUFRgK_pga1qsGMHCTsUKUmWEA/edit?usp=sharing](https://docs.google.com/document/d/1H-w4dBc1Svcmw_fzEKUFRgK_pga1qsGMHCTsUKUmWEA/edit?usp=sharing). We are working on providing simple tools for estimation.

// 2. The period you plan to cover with this offset [DateFrom] and [DateTo]

// Token amount:

// 3. the type of token to be sent from the community pool - [TOKEN]. Note that this token needs to find a way to Regen or Osmo token to buy rNCT on Osmosis DEX

// 4. the amount of tokens to be sent from the community pool [#]. You can calculate this amount by [tCO2] x [$ price of rNCT on Osmosis] / [$ price of TOKEN] x 1.2 = [#]. The Factor 1.2 serves as a buffer for price volatility between proposal submission and effective rNCT buy tx.

// Execution:

// The Agent will send the [TOKEN]s for Regen and do the buy tx on Osmosis, retire the rNCT on Regen, and send the left over to the Community Pool. It might be a multisig.

// 5. a trusted Agent - [AGENT NAME] and their officiel Twitter handle [TWTR]

// 6. the protocol account address of the Agent [ADDRESS] to receive the [TOKEN]s


===================================================================

**Proposal:** The Community Pool is authorised to spend [#][TOKEN]  to purchase [tCO2] tonnes of nature-based carbon credits from Regen Network, to offset the estimated carbon emissions of the protocol’s validator node operators, for the network to become carbon-negative from [DateFrom] to the end of [DateTo].

## **Background**

**The Impact Hub launched with a commitment by validators to operate a carbon-neutral blockchain network for the Internet of Impact.**

Blockchain networks have environmental impacts due to the energy consumed to operate validator node infrastructure.

Cosmos Proof-of-Stake networks consume only a fraction of the energy that is required for Proof-of-Work networks, such as Bitcoin and Ethereum.

However, the carbon footprint of operating Validator services, such as the emissions from business flights and office infrastructure, must also be factored into the total environmental costs of maintaining blockchain networks.

Carbon offsets are a generally accepted mechanism for neutralising unavoidable carbon emissions, as these incentivise emission reductions and contribute towards carbon capture activities, such as protecting natural forests.

Whilst carbon offsets are a necessary mechanism to address unavoidable carbon emissions in the near-term, all Validator service providers should plan to transition their power consumption to renewable energy sources, as soon as possible.

Validator Node operators may accrue economic benefits from being verifiably carbon-neutral, as this is likely to influence staking allocations. Consumers may also preferentially choose products and services that are built on carbon-neutral networks.

The Interchain Foundation Earth Program is leading the [ZERO Carbon Commitment](https://earthstate.ixo.world/zero/) for all blockchains in the Cosmos ecosystem to become provably net-zero (or negative) in their carbon emissions, as soon as possible.

CosmosSDK based networks are encouraged to make a ZERO Carbon Commitment through on-chain governance, to offset historical as well as future carbon emissions of operating the network.

The ZERO Carbon Commitment may be achieved at the level of individual Validator Node operators paying for their own offsets and/or through network-wide offsets funded from Community Pool resources and/or any other legitimate mechanisms that are best suited to each sovereign chain.

The Interchain Earth Program recommends that for this initial phase of implementing the Zero Carbon Commitment, a maximum annual carbon footprint estimation should be used to calculate the offset required. In future, the network-wide carbon footprint calculation is likely to become more accurate, as Validators provide more detailed claims about their energy consumption, and more Validators may be incentivised to source renewable energy to power their operations.

[Regen Network](http://regen.network/) is a public proof-of-stake blockchain custom-built for global carbon accounting on the CosmosSDK. Regen Network’s infrastructure originates high-quality nature-based digital carbon in the Interchain economy, unlocking web3 regenerative finance and catalysing solutions to the climate crisis.[](http://regen.network/)

[Regen Network](http://regen.network/) is launching rNCT, a premium digital carbon basket of nature-based projects launched by the Regen Network community in cooperation with the [Osmosis decentralised exchange](https://osmosis.zone/). rNCT is a fungible, IBC-compatible carbon basket backed by nature-based carbon credits that have verifiable ecological, social, and economic benefits issued onto the Regen Ledger blockchain. NCT can be used as a carbon offset and retired on-chain by reversing a basket token and retiring it in the on-chain registry on Regen Ledger.

NCT brings the first IBC-compatible carbon token to the Interchain economy, and provides one of the mechanisms through which application chains can implement the [ZERO Commitment](https://earthstate.ixo.world/zero/) for the Cosmos ecosystem (an initiative of the Interchain Foundation Earth Program). Cosmos-based chains and validators can calculate their carbon footprint using the [POS footprint calculator](https://github.com/bicowg/bicowg/tree/main/Validator-and-protocol-carbon-footprint-methods-and-analysis) offered by Regen Network and may choose to offset their carbon emissions by purchasing NCT on Osmosis, which can be redeemed for EcoCredits that are retired on the Regen Ledger.

## Carbon Footprint Estimation Method

Based on a survey of Impact Hub validators who self-reported their estimated carbon footprint, and using a worst-case scenario calculation to estimate the emissions of the whole network, that is currently operated by [V] Validator is projected to emit at most [X] tonnes of carbon for each 12 months of operation.

## **Proposal Details**

**Proposal 11: Offset the maximum estimated carbon emissions of the Impact Hub for the network to become carbon-neutral for the period from [DateFrom] to [DateTo].**

- Voting YES to this proposal approves [#][TOKEN] to be sent from the Community Pool to **purchase and retire [tCO2] NCT**carbon credits to offset the highest estimated carbon emissions of the network for period from [DateFrom] **to [DateTo].**
- Voting NO to this proposal indicates that funding should NOT be allocated from the Community Pool to purchase and retire [tCO2] rNCT carbon credits for offsetting the estimated carbon emissions of the network for the period [DateFrom] to [DateTo].

**Method**

- The network Community Pool will spend [#] [TOKEN] tokens on purchasing [tCO2] NCT on the Osmosis DEX from the NCT:REGEN Pool, using a programmatic SEND transaction to account address [ADDRESS].
- The Controller of the receiving account address [ADDRESS] will serve as a trusted Agent of the network.
- The Agent is [AGENT NAME] and this account address can be verified in a public post that has been published from the @[TWTR] Twitter account.
- The Agent will redeem an equivalent number of EcoCredits for the basket NCT tokens purchased using the Regen Network interface.
- The Agent will retire the equivalent number of EcoCredits on the Regen Ledger using the Regen Network interface, to offset NETWORK’s carbon emissions.
- The Agent will send back to the network Community Pool any balance of [TOKEN] remaining after the transaction has been settled.
- Records of the transactions performed by the Agent on behalf of the Impact Hub will be publicly published on the @[TWTR] Twitter account, with transaction hashes as evidence.

**Target on-chain date:** 18th March 2022

