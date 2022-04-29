# Credential Issuer

## Introduction

The BC Person verifiable credential described in this document is issued by the Province of British Columbia’s Ministry of Citizens' Services to Holders that are residents of the Province of British Columbia. The credential contains authoritative digital identity data attributes about the Holder held by the province, including their name and date of birth (see full list of attributes below). The credential is a cornerstone in the use of online digital identity for the residents of British Columbia.

## References

* Link to Schema

### Machine Readable Governance Information:

* Link to Overlays Capture Architecture: Source
* Link to Overlays Capture Architecture: Published

## Authority to Issue

The Province of British Columbia is legislatively authorized to collect and manage digital identity data about the residents of the Province of British Columbia, per [BC’s FREEDOM OF INFORMATION AND PROTECTION OF PRIVACY AMENDMENT ACT, 2011](https://www.bclaws.gov.bc.ca/civix/document/id/bills/billsprevious/4th39th:gov03-3). The Province of British Columbia is authorized to issue credentials containing a resident’s digital identity data to the resident in various forms, including as a “paper” credential (the BC Services Card), and in digital form, such as in the form of verifiable credentials. The purpose of providing residents with these credentials is to allow them to share the credentials with others as they see fit, without the knowledge or permission of the Government of British Columbia.

The Province of British Columbia has delegated the authority to manage digital identity data to the Ministry of Citizens’ Services, and the Ministry is the Issuer of this credential.

## The SCHEMA Credential

The Person credential provides the Holder with the core digital identity attributes held by the Province of British Columbia about the resident, such that the Holder can share those attributes with the verifiers of their choice.

The specific attributes in the credential are defined in the Layer 3 Credential Schema GF document listed in the [References](#references) section of this document.

### Issuer-Specific Credential Information

There is no issuer-specific information about the use of the BC Person credential. The credential is used exactly as described in the Layer 3 Credential Schema GF document listed in the [References](#hreferences) section of this document.

## Holders

The BC Person verifiable credential is available to a limited set of residents of the Province of British Columbia who consent to participate in a series of experimental applications of verifiable credential technology. These experiments may result in an expansion of the residents to which the BC Person credential is available.

### Pre-Issuance Verification

Prior to issuing the BC Person credential, the Issuer does the following verification of the Holder:

* Steps...

The authentication using the Mobile BC Services card provides a linkage between the Holder and their BC Wallet mobile app, and the digital identity record for the Holder held by the Province. The verifiable credential is constructed from the digital identity record, signed and issued to the Holder’s wallet.

### Revocation

The BC Person credential is revocable. A given BC Person credential may be revoked under the following conditions:

* The credential was issued in error.
* ...

## Intended Use of the BC Person Credential

The BC Person credential is intended to allow a BC resident to prove that they are a resident of BC (possession of the credential), and to provide authoritative demographic information about themselves to a verifier.

Note that all of the demographic information in the BC Person credential is Personally Identifiable Information (PII) and as such,

* ...

Example uses of the BC Person credential are plentiful:

* Collecting the name of a person opening a bank account.
* ...

Sample presentation requests are provided in the Layer 3 Credential Schema GF document listed in the [Technical Information](#sample-proof-requests) section of this document.

## Contact for Additional Information

For more more information about the use this document please contact the Ministry of Citizens’ Services using this email address: [idiminfo@gov.bc.ca](mailto:idiminfo@gov.bc.ca)

## Technical Information

### Ledger Information

* Ledger: [CANdy-Dev](https://candyscan.idlab.org/home/CANDY_DEV)
* Person Credential Issuer DID: &lt;DID with Link to Ledger Txn>
* Credential Definition ID: &lt;CRED_DEF ID with Link to Ledger Txn>

### Sample Proof Requests

* Examples
