# Guidance<!-- omit in toc -->

The following guidance is for those that are arriving at this site and want to
know how to quickly create and/or find the information they need.

- [Schema Publishers](#schema-publishers)
- [Verifiable Credential Issuers](#verifiable-credential-issuers)
- [Verifiers](#verifiers)
- [Holders / Wallet Apps Creators](#holders--wallet-apps-creators)
- [Ecosystem Participants / Contributors](#ecosystem-participants--contributors)

## Schema Publishers

Schema Publishers are organizations (perhaps made up of organizations) that
define and create Schema (and hence, types of verifiable credentials) objects
that are used within this ecosystem. An issuer of a type of verifiable credential
might also publish the schema for the verifiable credential, or, an issuer
might collaborate with other organizations to define the schema, and many
organizations are issuers of that type of schema.

For example, a single authority, such as the Law Society in a given
jurisdiction, might publish a schema for a type of verifiable credential to be
issued to their members. In that case, the Law Society is the Schema Publisher,
as well as the sole issuer of that type of verifiable credential. Alternatively,
the Law Societies across a set of jurisdictions (perhaps across Canada) might
work together to define the schema for all the Law Societies to use. The group
of collaborators becomes the Schema Publisher, and each Law Society an issuer of
that type of verifiable credential. Note that "Governance Framework" for the
schema will be managed elsewhere from this site by the collaborators, in
whatever form they wish. All that is needed on this site is a description of the
schema in a format matching the [Schema Template](../6.%20Templates/Schema.md)
used on this site, perhaps with a reference in the document back to the "full"
Governance Framework.

To be a schema publisher, follow these steps:

* Review the ToIP Layer 1 and Layer 2 sections of the site to understand
  AnonCreds verifiable credentials and the best practices in defining schemas
  suitable for use by multiple issuers.
* See if there are any Schemas that could serve er your purpose.
    * Reusing existing schemas helps everyone in the ecosystem.
    * If you have questions about specific published schemas, use the contact
      information found in the relevant Schema document to learn more about how
      you can issue credentials using the schema.
* Collaborate (as needed) with other organizations that plan to issue
  credentials based on the published schema.
* Publish the schema on the appropriate ToIP Layer 1 utility.
* Create a pull request in the source GitHub repository for this site to add a
  Schema document, [based on this template](../6.%20Templates/Schema.md)).
* Work with this site's
  [Editors](../5.%20Governance/Governance.md#current-editors) to have
  your pull request approved and merged so that it appears on the site.

## Verifiable Credential Issuers

Verifiable Credential Issuers are organizations that issue verifiable
credentials based on a defined Schema. An issuer of a type of verifiable
credential might also publish the schema for the verifiable credential, or,
issue credentials based on a [published schema](#schema-publishers).

* Review the [Technical Stack](../2.%20Technical%20Stack/README.md) section of
  the site to understand what (for now) Hyperledger Indy ledgers are used in the
  ecosystem, and what Aries Protocols your agents should support.
* Review the [Schemas](../3.%20Schemas/README.md) on this site to see if you can
  use for them for the credentials you want to issue.
    * Reusing existing schemas helps everyone in the ecosystem.
    * If you have questions about specific published schemas, use the contact
      information found in the relevant Schema document to learn more about how
      you can issue credentials using the schema.
* If you have to create your own schema, follow the steps above for [Schema
  Publishers](#schema-publishers).
* Do the technical work to create your issuer.
* Create a pull request in the [source GitHub
  repository](https://github.com/cloudcompass/demo-pancdn-toip-gf) for this site
  to add a Credential Issuer document [based on this
  template](../6.%20Templates/Issuer.md) in the folder of the Schema your are
  using.
*  Work with this site's
  [Editors](../5.%20Governance/Governance.md#current-editors) to have
  your pull request approved and merged so that it appears on the site.

## Verifiers

Verifiers request presentations from Holders and verify claims from verifiable
credentials issued by the Issuers in this ecosystem, which in turn are based on
[Schemas](../3.%20Schemas/README.md) defined in this ecosystem. Publishing a
verifier document on this site is optional. However, doing so is recommended as
it allows the ecosystem's participating organizations to provide visibility for
Holders and other ecosystem participants about your verifier policies.

To become a known verifier in this ecosystem, follow these steps:

* Review the [Technical Stack](../2.%20Technical%20Stack/README.md) section of
  the site to understand what (for now) Hyperledger Indy ledgers are used in the
  ecosystem, and what Aries Protocols your agents should support.
* Review the [Schema and Credential Issuer documents](../3.%20Schemas/README.md)
  on this site to determine what issued credential you are interested in
  verifying, and how you can use those credentials in your business processes.
    * If you have questions about specific published schemas or issuers, use the
      contact information found in the relevant schema or issuer documents to
      learn more about the semantics of the schema and the issuing processes of
      the Issuers.
* Do the technical work to create your issuer.
* If you think it appropriate, create a pull request in the [source GitHub
  repository](https://github.com/cloudcompass/demo-pancdn-toip-gf) for this site
  to add a Verifier document [based on this
  template](../6.%20Templates/Verifier.md) in the
  [Verifiers](../4.%20Verifiers/README.md) folder about each of your verifiers.
*  Work with this site's
  [Editors](../5.%20Governance/Governance.md#current-editors) to have
  your pull request approved and merged so that it appears on the site.

## Holders / Wallet Apps Creators

If you want to know how Verifiers that are part of this ecosystem collect and
use the information from credentials you might hold, follow the steps below.
Wallet apps that act as holders may want to use the verifiers information on
this site to let their users know about the verifiers requesting their data.

* Review the Layer 3 Verifier documents on this site.
    * If you have questions about specific verifiers, use the contact
      information found in the relevant Verifier documents.

## Ecosystem Participants / Contributors

If you want to know how this ecosystem operates, or you want to participate in,
or contribute to, this ecosystem, follow these steps.

* Review the ToIP Layer 4 section of this site to understand how the site is
  the Governance Framework, and how contributions to the Governance Framework
  are managed.
* If you have questions, submit an issue to the source GitHub repository for
  this site.

If in using this site you see any issues with documents in the site you are
encouraged to either create an issue or, if you have the technical experience,
create a pull request in the source GitHub repository.
