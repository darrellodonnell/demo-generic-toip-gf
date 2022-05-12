# Summary: Ecosystem Technical Stack

While this site contains all of the details about each of the ToIP Layers used
within the ecosystem, the following is a brief overview of the ecosystem's ToIP Layers
1, 2 and 3 technical components.

## Layer 1 Public Utilities

Several Hyperledger Indy-based Layer 1 utility instances are used in the
ecosystem.

* [CANdy](Layer%201/CANdy.md), an instance of Hyperledger Indy operated by
  several Canadian provincial jurisdictions for the use of their issuers.
* [Sovrin MainNet](Layer%201/Sovrin.md), an instance of Hyperledger Indy
  operated by the Sovrin Foundation and available for use by legal entities
  (including governments) that agree to operate based on the [Sovrin Governance
  Framework](https://sovrin.org/library/sovrin-governance-framework/).

Associated with each Layer 1 utility is a test instance of that utility that can
be used be ecosystem participants for testing purposes. Access to the test
instances is included in the details about the Layer 1 utilities.

## Layer 2 Peer-to-Peer Protocols

[DIDComm v1 and Hyperledger Aries
protocols](https://github.com/hyperledger/aries-rfcs) for used in the ecosystem
messaging between participants, and
[AnonCreds](https://anoncreds-wg.github.io/anoncreds-spec/) verifiable
credentials are issued and verified. Specifically:

* [Aries Interop Profile 1.0](https://github.com/hyperledger/aries-rfcs/tree/master/concepts/0302-aries-interop-profile#aries-interop-profile-version-10)
    * AIP 1.0 is considered to be deprecated and support is provided for backwards compatibility.
* [Aries Interop Profile 2.0](https://github.com/hyperledger/aries-rfcs/tree/master/concepts/0302-aries-interop-profile#aries-interop-profile-version-20), including the following sub-targets:
    * [Mediate](https://github.com/hyperledger/aries-rfcs/tree/main/concepts/0302-aries-interop-profile#mediate-mediator-coordination)
    * [AnonCreds](https://github.com/hyperledger/aries-rfcs/tree/main/concepts/0302-aries-interop-profile#indycred-indy-based-credentials)
    * [DIDComm V2 Prep](https://github.com/hyperledger/aries-rfcs/tree/main/concepts/0302-aries-interop-profile#didcommv2prep-didcomm-v2-prep)
    * [Chat](https://github.com/hyperledger/aries-rfcs/tree/main/concepts/0302-aries-interop-profile#chat-chat-related-features)

At this time the AIP 2.0 sub-targets related to JSON-LD and BBS+ based verifiable credentials are not supported in the ecosystem.

The [Aries Agent Test
Harness](https://github.com/yperledger/aries-agent-test-harness) and the [Aries
Mobile Test Harness](https://github.com/hyperledger/aries-mobile-test-harness)
are used to demonstrate ecosystem Layer 2 interoperability across Aries frameworks
and mobile apps.

## Layer 3 Data Exchange Protocols

As noted in the Layer 2 overview, the participants in the ecosystem use
[AnonCreds](https://anoncreds-wg.github.io/anoncreds-spec/) format verifiable
credentials for the trusted data exchange of claims. As such, this site contains
Layer 3 verifiable credential information from ecosystem participants, including:

* All published AnonCreds Schemas
* The issuing of verifiable credentials by all Credential Issuers
* The presentations requested by some Verifiers in the ecosystem

The schema, issuer and verifier documents are created and maintained by
their respective authorities (schema publishers, issuers and verifiers).
