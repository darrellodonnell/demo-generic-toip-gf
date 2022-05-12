# Ecosystem Layer 2

## Layer 2 Peer-to-Peer Protocols

The participants of the ecosystem use [DIDComm v1 and Hyperledger Aries
protocols](https://github.com/hyperledger/aries-rfcs) for messaging between
ecosystem, and [AnonCreds](https://anoncreds-wg.github.io/anoncreds-spec/)
verifiable credentials. Specifically:

* [Aries Interop Profile 1.0](https://github.com/hyperledger/aries-rfcs/tree/master/concepts/0302-aries-interop-profile#aries-interop-profile-version-10)
    * AIP 1.0 is considered to be deprecated and support is provided for backwards compatibility.
* [Aries Interop Profile 2.0](https://github.com/hyperledger/aries-rfcs/tree/master/concepts/0302-aries-interop-profile#aries-interop-profile-version-20), including the following sub-targets:
    * [Mediate](https://github.com/hyperledger/aries-rfcs/tree/main/concepts/0302-aries-interop-profile#mediate-mediator-coordination)
    * [AnonCreds](https://github.com/hyperledger/aries-rfcs/tree/main/concepts/0302-aries-interop-profile#indycred-indy-based-credentials)
    * [DIDComm V2 Prep](https://github.com/hyperledger/aries-rfcs/tree/main/concepts/0302-aries-interop-profile#didcommv2prep-didcomm-v2-prep)
    * [Chat](https://github.com/hyperledger/aries-rfcs/tree/main/concepts/0302-aries-interop-profile#chat-chat-related-features)

At this time the sub-targets related to JSON-LD and BBS+ based verifiable credentials are not supported in the ecosystem.

The [Aries Agent Test
Harness](https://github.com/yperledger/aries-agent-test-harness) and the [Aries
Mobile Test Harness](https://github.com/hyperledger/aries-mobile-test-harness)
are used to demonstrate Layer 2 interoperability across Aries frameworks
and mobile apps.
