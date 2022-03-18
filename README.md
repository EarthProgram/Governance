# Blockchain Governance - Templates for Protocol Proposals

To use the Zero Carbon Emissions template, you will need to have determined:

rNCT amount:

1. the amount of tons of CO2 that you want to offset - [tCO2]. For simplicity, we recommend you to collect validators self reported emissions with a survey and use: (known validators emissions + worst validator emission x # unknown validators) x safety factor. Usually on Cosmos a large validator emission might be around 5-10t per year, on average closer to 1t. The safety factor might be 2x-10x depending on your estimation. A more detailed methodology has been presented in https://docs.google.com/document/d/1H-w4dBc1Svcmw_fzEKUFRgK_pga1qsGMHCTsUKUmWEA/edit?usp=sharing. We are working on providing simple tools for estimation.

2. The period you plan to cover with this offset [DateFrom] and [DateTo]

Token amount:

3. the type of token to be sent from the community pool - [TOKEN]. Note that this token needs to find a way to Regen or Osmo token to buy rNCT on Osmosis DEX

4. the amount of tokens to be sent from the community pool [#]. You can calculate this amount by [tCO2] x [$ price of rNCT on Osmosis] / [$ price of TOKEN] x 1.2 = [#]. The Factor 1.2 serves as a buffer for price volatility between proposal submission and effective rNCT buy tx.

Execution:

The Agent will send the [TOKEN]s for Regen and do the buy tx on Osmosis, retire the rNCT on Regen, and send the left over to the Community Pool. It might be a multisig.

5. a trusted Agent - [AGENT NAME] and their officiel Twitter handle [TWTR]

6. the protocol account address of the Agent [ADDRESS] to receive the [TOKEN]s
