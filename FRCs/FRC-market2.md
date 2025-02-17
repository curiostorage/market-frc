---
fip: "<to be assigned>" <!--keep the qoutes around the fip number, i.e: `fip: "0001"`-->
title: Market 2.0 
author: "Andrew Jackson (@snadrus), Mayank Pandey (@lexluthr)"
discussions-to: <URL>
status: Draft
type: FRC
category Interface
created: 2025-02-17
spec-sections: 
  - <section-id>
  - <section-id>
requires (*optional): <FIP number(s)>
replaces (*optional): <FIP number(s)>
---

# Market 2.0

## Simple Summary
A market with DDO compatability, paid deals, and other clean-ups will benefit Storage Providers, Data-Owners, and the network as a whole. 

## Abstract
Solving for today's needs hampering the flow from data-owners to Storage Providers will bring a healthier ecosystem. 
Using the chain for static state and simple http for exchanging info will enable healthy cross-region behavior and reach into the Web2 needs. 

## Change Motivation
Market 1.0 & 1.1 are mostly avoided for other side-channels to get SPs data, often with an offline focus. 
A variety of tools and companies attempt to fill the void (aggregators, multi-company SPs). 

## Specification
<!--The technical specification should describe the syntax and semantics of any new feature. The specification should be detailed enough to allow competing, interoperable implementations for any of the current Filecoin implementations. -->
The technical specification should describe the syntax and semantics of any new feature. The specification should be detailed enough to allow competing, interoperable implementations for any of the current Filecoin implementations.

## Design Rationale
Needs: 
- SPs cannot benefit from Spark_FIL+ & get the discounts DDO offers.
- Paid deals are an upcoming requirement from Storage Providers. 
- Browsers cannot directly engage with SPs today without a middleman.
- Making the connection:
  - What is needed for an SP to store my deal?
  - Which SP is best for my needs?

Design: 
HTTP(S) solves the cross-region & web2 reachability. 

## Backwards Compatibility
The HTTP server should not block endpoints needed for Markets 1.0 so the same endpoints can be used. 

## Test Cases
Making deals, reading state, etc should all be possible with a Web 2.0 Front-end test suite and a block explorer (equivalent).

## Security Considerations
N/A. SPs decide what they wish to share and offer. HTTP requires DDoS protections. 

## Incentive Considerations
Aggregators using this technology are free to provide considerably less for the same effectiveness: payment management, SP lists, and an API. 
Paid deals will invite open discussions of value. 

## Product Considerations
SPs won't need to sign agreements with anyone to get data from people they don't know on terms they want. 

## Implementation
Curio Storage intends to build this out for its flagship product for open-source SP operations. 

## TODO
<!--A section that lists any unresolved issues or tasks that are part of the FIP proposal. Examples of these include performing benchmarking to know gas fees, validate claims made in the FIP once the final implementation is ready, etc. A FIP can only move to a “Last Call” status once all these items have been resolved.-->
A section that lists any unresolved issues or tasks that are part of the FIP proposal. Examples of these include performing benchmarking to know gas fees, validate claims made in the FIP once the final implementation is ready, etc. A FIP can only move to a “Last Call” status once all these items have been resolved.

## Copyright
Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
