# Blockchain Governance - Templates for Protocol Proposals

You can find in this repo templates for common Protocol Proposals that may be useful for all protocols. The template may be used as it is after filling the [...] and it may also be amended to fit special purposes.


## Zero Carbon Emissions template
To use the Zero Carbon Emissions template, you need to determine:

NCT amount:

1. the amount of tons of CO2 that you want to offset: [tCO2]. 

This implies a **Carbon Footprint Estimation Method** for the [V] Validators of the protocol having a total estimated emission of [X] tCO2.
For simplicity, we recommend you to collect validators self reported emissions with a survey and use the formula: 

[X] = sum of known validators emissions + ( worst validator emission x # unknown validators )

[tCO2] = [X] x safety factor 

Usually on Cosmos SDK an average validator emission per network is in the order of 1t, a more secure validator emission might be around 5-10t per year, and it has been reported at most 25t. Make sure to only count your network emissions as validators may validate several at once. The safety factor might be 2x-5x depending on your estimation accuracy, to be on the safer side. A more detailed methodology has been presented in https://docs.google.com/document/d/1H-w4dBc1Svcmw_fzEKUFRgK_pga1qsGMHCTsUKUmWEA/edit?usp=sharing. We are working on providing simple tools for estimation. If you choose another method, you may update that part in the proposal template.

2. The period you plan to cover with this offset [DateFrom] and [DateTo]. The standard emissions calculators are generally providing emissions per year, make sure to take the period duration into account in your [tCO2], typically by multiplying by ( # days in period ) / 365.

Token amount:

3. the type of token to be sent from the community pool: [TOKEN]. Note that this token needs to find a way to Regen or Osmo token to buy NCT on Osmosis DEX

4. the amount of tokens to be sent from the community pool: [#]. 

This amount is [tCO2] x [$ price of NCT on Osmosis] / [$ price of TOKEN] x 1.2 = [#]. The Factor 1.2 serves as a buffer for price volatility between proposal submission and effective NCT buy tx.

Execution:

The protocol needs to pick a trusted Agent to execute the multiple steps of the proposal. The Agent will IBC the [TOKEN]s to Osmosis, sell for Regen tokens, buy NCT, IBC the NCT to Regen network, retire the NCT, sell the left over Regen tokens for [TOKEN] and IBC the [TOKEN] to the Community Pool on the protocol network. The Agent might be a multisig.

5. a trusted Agent: [AGENT NAME] and their officiel Twitter handle [TWTR]

6. the protocol account address of the Agent [ADDRESS] to receive the [TOKEN]s
