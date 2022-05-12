# Demo: A Pan Canadian Verifiable Credential Ecosystem Governance Framework

This repository is a demonstration of expressing a decentralized Pan-Canadian
Ecosystem Verifiable Credential Governance Framework by providing a structured
place for publishing governance documents about the ecosystem so that audiences
can find and understand those documents. Member participants in this ecosystem
(e.g., Canadian governments) can publish the documents over which they are the
authority that define how to participate in the ecosystem. Entities wishing to
participate in the ecosystem (e.g., public or private organizations), such as
being a verifier of government issued verifiable credentials, can use the
information published here to understand how to receive and process the
verifiable credentials being issued. Further, the use of a GitHub repository
enables the curated evolution of the ecosystem governance framework with
questions (issues), suggestions (pull requests) and controlled updates
(maintainers) in an open, collaborative and tightly governed manner.

The following are examples of information to be found in this repository.

* Guidance about the ToIP Layer 1 Utilities being used by the ecosystem
  participants.
  * Used by those wanting to be Issuers, Verifiers and Holders to know what
    utilities must be supported.
* Guidance about the ToIP Layer 2 Peer to Peer Protocols being used by the
  ecosystem participants.
  * Used by those wanting to be Issuers, Verifiers and Holders to know what
    protocols must be supported in order to interact with other participants.
* Documents from Schema Publishers describing the purpose and semantics of the
  Schemas being used.
  * Used by Issuers to ensure they issue credentials aligned with others using
    the same Schema.
  * Used by Verifiers to know what claims to request from credentials using a
    published Schema, and what the data they receive means.
* Documents from credential Issuers describing their usage of the published
  schemas.
  * Used by Verifiers to know the meaning of claims from credentials issued by
    specific Issuer.
* Documents from Verifiers describing the presentation requests they make and
  how they use the presented claims.
  * Used by Holder applications (including mobile Wallets) to provide
    information about verifiers to the Wallet owner.

We are using a minimum viable product (MVP) approach to building this governance
framework by starting with what is thought to be the minimum necessary
information required for the audience of each document and using feedback from
the audience members to decide how to evolve the documents. The feedback might
lead us to update a specific document in question, or to update the templates
upon which all the documents of a given type are based.

Using an MVP approach means that we will (at least at first) assume that
the audience for this Governance Framework has a background in:

* The use of verifiable credentials, and particularly, verifiable credentials
  using AnonCreds.
* The participants in verifiable credential exchanges: Issuers, Holders and
  Verifiers.
  * Plus an extra participant in AnonCreds verifiable credential exchanges --
    Schema Publishers
* Trust over IP (ToIP) and especially the [ToIP
  model](https://trustoverip.org/wp-content/toip-model/), including the ToIP
  Layers (1-4).
* Hyperledger Aries, Aries agents, the protocols defined in the Aries and how
  they all fit together.
* Hyperledger Indy as a ToIP Layer 1 utility ledger, including the objects
  published by Issuers and in some cases, Verifiers on an Indy ledger.

The level of knowledge needed by those using this Governance Framework
repository (listed above) is ok for the short term, but far too high for the
long term. An important part of the feedback and evolution of this site will
include getting the right level here, and pointers to other sources of
information for those needing more.

Those contributing to the Governance Framework must also understand using
GitHub, git, markdown, submitting pull requests (PRs), reviewing and approving
PRs and merging PRs. It's a lot. Please see the [contributing](CONTRIBUTING.md)
document for an overview of how to contribute.

## tl;dr Summary of this Repository

The repository contains Layers 1, 2 and 3 information as follows, each connected
to a document that describes that single part of the overall Ecosystem. In this
first (very MVP) cut of the repository, the Layer 3 items (Schemas, Issued
Credentials and Verifier Presentations) are manually added as documents.
Eventually, the Table of Contents listed here will be generated based on the
documents within the repository.

* Ecosystem governance, including rules for contributing to this
  repository via Issues and Pull Requests.
* Layer 1 utilities are based on Hyperledger Indy.
  * Supported instances for production include:
    * [CANdy ledger](https://candyscan.idlab.org/) for the rooting of
      credentials issued by Canadian governments and the 
    * [Sovrin MainNet](https://indyscan.io/home/SOVRIN_MAINNET) ledger for
      credential issued by non-government entities in the ecosystem.
* Layer 2 peer to peer protocols are based on [Aries Interop Profile 2.0  (AIP
  2.0)](https://github.com/hyperledger/aries-rfcs/tree/master/concepts/0302-aries-interop-profile#aries-interop-profile-version-20)
  * Some [Aries Interop Profile 1.0 (AIP 1.0
    )](https://github.com/hyperledger/aries-rfcs/tree/master/concepts/0302-aries-interop-profile#aries-interop-profile-version-10)
    protocols are still used, including those used in establishing connections,
    issuing credentials and presenting proofs.
* Schemas published by contributors that may be useful in the ecosystem
    * Issuers that issue verifiable credential based on the published schemas
* Verifiers that request proof of verifiable credentials in the ecosystem
