# Ecosystem Overview

## Introduction

The site is the (_demonstration!!_) Pan-Canadian Ecosystem Governance Framework
(PCEGF) for Verifiable Credentials, an implementation of a [Layer 4 Trust over
IP Ecosystem Governance
Framework](https://trustoverip.org/wp-content/toip-model/). This site provides
information about all 4 Layers of the Trust over IP Governance Stack for all
issuers, holders and verifiers that participate in the Pan-Canadian verifiable
credential ecosystem.

> **CAVEAT:** This site is a proof-of-concept Ecosystem Governance Framework for
  demonstration purposes only. It is not an authorized publication of any
  organization.

The (future) authoritative participants in the PCEGF (e.g., Canadian
governments) use this site to publish the governance documents for the
ecosystem, and manage the contributions of other organizations that publish
documents about how they participate in the ecosystem. Entities wishing to
participant in the ecosystem (e.g., public or private organizations), such as
being a verifier of government issued verifiable credentials, can use the
information published here to understand how to receive and process the
verifiable credentials being issued. Further, the use of a GitHub repository
that is the source for this site enables the curated evolution of the PCEGF
itself with questions (issues), suggestions (pull requests) managed by
authorized Editors that enable an open, collaborative and tightly governed
manner.

The following are examples of information to be found on this site.

* Guidance about the [Technical
  Stack](2.%20Technical%20Stack/Layer%202/README.md) being used by the ecosystem
  participants.
    * Used by those wanting to be Issuers, Verifiers and Holders to know what
      [ToIP Layer 1 Utility
      networks](2.%20Technical%20Stack/Layer%201/README.md) and [ToIP Layer 2
      Protocols and Apps](2.%20Technical%20Stack/Layer%202/README.md) that must
      be supported to participate in the ecosystem.
* A list of documents about the [Schemas](3.%20Schemas/README.md) used in the
  ecosystem, including the purpose and schema semantics, and for each, the set
  of verifiable credential Issuers using of the Schema.
    * Used by Issuers to ensure they issue credentials aligned with others using
      the same Schema.
    * Used by Verifiers to know what claims to request, what the received claims
      mean, and the policies and technical specifics of each Issuer.
* A list of documents published by [Verifiers](4.%20Verifiers/README.md)
  describing the presentation requests they make and how they use the presented
  claims.
    * Used by Holder applications (including mobile Wallets) to provide
      information about verifiers to the Wallet owner.
* A set of Ecosystem Governance documents that describe how the ecosystem
  operates and evolves.
    * This is the "meta" of the site that defines how the information published
      on this site is managed -- who can change what, how and when.

For more information about this site and how to use it, please see the [Using
this Site](1.%20Using%20This%20Site/README.md) section.

## Out of Scope

This site is not intended to be a full Governance Framework for every ToIP Layer
and document published on this site. Consider the
[schemas](3.%20Schemas/README.md) that are published here. The process
("governance framework") used to define and evolve a schema, and who is involved
in that process, is outside the scope of this site. What is published here is a
summary document from the schema publisher containing the technical/policy
details about the schema sufficient for Issuers, Holders and Verifiers to
understand what the Schema is for and how to use it in this ecosystem. Likewise
for:

* The Issuers that used the schema published here.
* The Verifiers that request presentations based on schemas published here.
* The[ ToIP Layer 1 Utilities](2.%20Technical%20Stack/Layer%201/README.md) and
  [ToIP Layer 2 Protocols and Apps](2.%20Technical%20Stack/Layer%202/README.md)
  that are used in this ecosystem. Their governance framework is managed
  elsewhere, and all that is here are the technical details needed by the
  ecosystem participants.

## The MVP Ecosystem Approach

We are using a minimum viable product (MVP) approach to building this ecosystem
governance framework by starting with what is thought to be the minimum
necessary information required for the audience of each document, and using
feedback from the audience members to decide how to evolve the documents. The
feedback might lead us to update a specific document in question, or to update
the templates upon which all the documents of a given type are based.

## Assumptions About the Audience

Using an MVP approach implies that we will (at least at first) assume that
the audience for the PCEGF has a background in:

* The use of verifiable credentials, and particularly, verifiable credentials
  using Hyperledger Indy ledgers and AnonCreds format verifiable credentials.
* The participants in verifiable credential exchanges: Issuers, Holders and
  Verifiers.
    * Plus an extra participant in AnonCreds verifiable credential exchanges --
      Schema Publishers
* [Trust over IP (ToIP)](https://trustoverip.org) and especially the [ToIP
  model](https://trustoverip.org/wp-content/toip-model/).
* Hyperledger Aries, Aries agents, the protocols defined in the Aries and how
  they all fit together.
* Hyperledger Indy as a ToIP Layer 1 utility ledger, including the objects
  published by Issuers and in some cases, Verifiers on an Indy ledger.

The level of knowledge needed by those using this Governance Framework
repository (listed above) is sufficient for the short term, but far too high for the
long term. An important part of the feedback and evolution of this site will
include getting the right level here, and pointers to other sources of
information for those needing more.

Those contributing to the Governance Framework must also understand using
GitHub, git, markdown, submitting pull requests (PRs), reviewing and approving
PRs and merging PRs. It's a lot. Please see the [contributing](../Layer%204/CONTRIBUTING.md)
document for an overview of how to contribute.
