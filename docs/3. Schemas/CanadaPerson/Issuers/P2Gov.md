# Government of PROVINCE2

## Introduction

The "Canada Person" verifiable credential is issued by the Province of PROVINCE2 to Holders that are residents of the Province of PROVINCE2. The credential contains authoritative digital identity data attributes about the Holder held by the province, including their name and date of birth (see full list of attributes below). The credential is a cornerstone in the use of online digital identity for the residents of PROVINCE2.

## Technical Information

### Ledger Information

* Ledger: [CANdy-Dev](https://candyscan.idlab.org/home/CANDY_DEV)
* Government of PROVINCE2 Issuer DID for the Canada Person verifiable credential: &lt;DID with Link to Ledger Txn>
* Credential Definition ID: &lt;CRED_DEF ID with Link to Ledger Txn>
* &lt;Link to Overlays Capture Architecture: Source>
* &lt;Link to Overlays Capture Architecture: Published>

## Authority to Issue

The Province of PROVINCE2 is legislatively authorized to collect and manage digital identity data about the residents of the Province of PROVINCE2. The Province of PROVINCE2 is authorized to issue credentials containing a resident’s digital identity data to the resident in various forms, including as a “paper” credential (the PROVINCE2 Driver's License), and in digital form, such as in the form of verifiable credentials. The purpose of providing residents with these credentials is to allow them to share the credentials with others as they see fit, without the knowledge or permission of the Government of PROVINCE2.

## The Government of PROVINCE2 Issued Canada Person Credential

The "Canada Person" credential provides the Holder with core digital identity attributes held by the Province of PROVINCE2 about the resident, such that the Holder can share those attributes with the verifiers of their choice.

### Issuer-Specific Credential Information

The following sections describes the differences between the ["Canada Person" Schema documentation](../README.md) and the verifiable credentials issued by PROVINCE2 using this schema.

#### Attributes Not Published

PROVINCE2 issued "Canada Person" credentials do not publish the following attributes:

* None

#### Attributes Handled Differently

* None

### Holders

The PROVINCE2 "Canada Person" verifiable credential is available to a limited set of residents of the Province of PROVINCE2 who consent to participate in a series of experimental applications of verifiable credential technology. These experiments may result in an expansion of the residents to which the PROVINCE2 "Canada Person" credential is made available.

#### Pre-Issuance Verification

Prior to issuing the PROVINCE2 "Canada Person" credential, the Issuer does the following verification of the Holder:

* The Holder must be a resident of the Province of PROVINCE2.
* The Holder must be using the PROVINCE2 Wallet mobile application (link to be added).
* The Holder must authenticate with the Issuer.

### Revocation

The PROVINCE2 "Canada Person" credential is revocable. A given "PROVINCE2 Person" credential may be revoked under the following conditions:

* The credential was issued in error.
* The Holder’s digital identity data that is included in the "Canada Person" credential changes (e.g. name change, corrected date of birth, etc.).
* Based on the Person credential lifecycle policy of the Government of PROVINCE2 (to be determined).
    * For example, a Government of PROVINCE2 policy may be defined that the verifiable credential be reissued every N years, even if it does not change.
* If the Schema for the credential changes, and the Government of PROVINCE2 determines that a reissuance using the new Schema is appropriate.

## Intended Use of the PROVINCE2 "Canada Person" Credential

The PROVINCE2 "Canada Person" credential is intended to allow a PROVINCE2 resident to prove that they are a resident of PROVINCE2 (possession of the credential), and to provide authoritative demographic information about themselves to a verifier.

Note that all of the demographic information in the PROVINCE2 "Canada Person" credential is Personally Identifiable Information (PII) and as such,

* The Holder/Resident should take care in deciding with whom they share the information, and for what purpose.
    * The PROVINCE2 Wallet mobile application is planned to have features that help the Holder in making such decisions.
* Verifiers receiving the information MUST handle the data in a manner consistent with the Privacy Laws of the Province of PROVINCE2.
* Verifiers MUST NOT request attributes from the PROVINCE2 "Canada Person" credential for purposes of which they are not needed.
    * For example, when verifying the age of a person when purchasing alcohol, the "Canada Person" credential can be used to prove the person is over the age of 19 without sharing any other information from the credential.

Example uses of the PROVINCE2 "Canada Person" credential are plentiful:

* Collecting the name of a person opening a bank account.
* Collecting the name of a new hire joining a company.
* Providing the name of a person requesting a Criminal Records Check.
* Completing an online form requiring the entry of data from the credential.
* Verifying the person is a resident of PROVINCE2 for a discount on goods.
* Verifying a person is of age to, for example, purchase alcohol.

## Contact for Additional Information

For more more information about the use this document please contact the Government of PROVINCE2 using this email address: [digidinfo@gov.prov3.ca](mailto:digidinfo@gov.prov3.ca)

## Sample Presentation Requests


