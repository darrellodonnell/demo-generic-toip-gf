# Government of BC

## Introduction

The Canada Person verifiable credential is issued by the Province of British Columbia’s Ministry of Citizens' Services to Holders that are residents of the Province of British Columbia. The credential contains authoritative digital identity data attributes about the Holder held by the province, including their name and date of birth (see full list of attributes below). The credential is a cornerstone in the use of online digital identity for the residents of British Columbia.

## Technical Information

### Ledger Information

* Ledger: [CANdy-Dev](https://candyscan.idlab.org/home/CANDY_DEV)
* Government of BC Issuer DID for the Canada Person verifiable credential: &lt;DID with Link to Ledger Txn>
* Credential Definition ID: &lt;CRED_DEF ID with Link to Ledger Txn>
* &lt;Link to Overlays Capture Architecture: Source>
* &lt;Link to Overlays Capture Architecture: Published>

## Authority to Issue

The Province of British Columbia is legislatively authorized to collect and manage digital identity data about the residents of the Province of British Columbia, per [BC’s FREEDOM OF INFORMATION AND PROTECTION OF PRIVACY AMENDMENT ACT, 2011](https://www.bclaws.gov.bc.ca/civix/document/id/bills/billsprevious/4th39th:gov03-3). The Province of British Columbia is authorized to issue credentials containing a resident’s digital identity data to the resident in various forms, including as a “paper” credential (the BC Services Card), and in digital form, such as in the form of verifiable credentials. The purpose of providing residents with these credentials is to allow them to share the credentials with others as they see fit, without the knowledge or permission of the Government of British Columbia.

The Province of British Columbia has delegated the authority to manage digital identity data to the Ministry of Citizens’ Services, and the Ministry is the Issuer of this credential.

## The Government of BC Issued Canada Person Credential

The Canada Person credential provides the Holder with core digital identity attributes held by the Province of British Columbia about the resident, such that the Holder can share those attributes with the verifiers of their choice.

### Issuer-Specific Credential Information

The following sections describes the differences between the [Canada Person Schema documentation](../README.md) and the verifiable credentials issued by BC using this schema.

#### Attributes Not Published

BC issued Canada Person credentials do not publish the following attributes:

* photo_id: is "" in all issuances

#### Attributes Handled Differently

* All name-related items (full_name, given_name, given_names and surname) are in CAPITAL letters.

### Holders

The BC "Canada Person" verifiable credential is available to a limited set of residents of the Province of British Columbia who consent to participate in a series of experimental applications of verifiable credential technology. These experiments may result in an expansion of the residents to which the BC "Canada Person" credential is made available.

#### Pre-Issuance Verification

Prior to issuing the BC "Canada Person" credential, the Issuer does the following verification of the Holder:

* The Holder must be a resident of the Province of British Columbia.
* The Holder must have a BC Services Card.
* The Holder must have a Mobile BC Services Card.
    * To receive a Mobile BC Services Card, the Holder must have successfully completed one of the following identity proofing processes:
        * Participate in an in-person verification of their Services Card at a Services BC location
        * Complete a video call verification of their Services Card with Services BC
        * Provide a video verification recording to Services BC
* The Holder must be using the BC Wallet mobile application (link to be added).
* The Holder must authenticate with the Issuer using their Mobile BC Services Card.

The authentication using the Mobile BC Services card provides a linkage between the Holder and their BC Wallet mobile app, and the digital identity record for the Holder held by the Province. The verifiable credential is constructed from the digital identity record, signed and issued to the Holder’s wallet.

### Revocation

The BC Person credential is revocable. A given BC Person credential may be revoked under the following conditions:

* The credential was issued in error.
* The Holder’s digital identity data that is included in the Person credential changes (e.g. name change, corrected date of birth, etc.).
* Based on the Person credential lifecycle policy of the Ministry of Citizens’ Services (to be determined).
    * For example, a Ministry of Citizens’ Services policy may be defined that the verifiable credential be reissued every N years, even if it does not change.
* If the Schema for the credential changes, and the Ministry of Citizens’ Services determines that a reissuance using the new Schema is appropriate.

## Intended Use of the BC Person Credential

The BC Person credential is intended to allow a BC resident to prove that they are a resident of BC (possession of the credential), and to provide authoritative demographic information about themselves to a verifier.

Note that all of the demographic information in the BC Person credential is Personally Identifiable Information (PII) and as such,

* The Holder/Resident should take care in deciding with whom they share the information, and for what purpose.
    * The BC Wallet mobile application is planned to have features that help the Holder in making such decisions.
* Verifiers receiving the information MUST handle the data in a manner consistent with the Privacy Laws of the Province of British Columbia.
* Verifiers MUST NOT request attributes from the BC Person credential for purposes of which they are not needed.
    * For example, when verifying the age of a person when purchasing alcohol, the Person credential can be used to prove the person is over the age of 19 without sharing any other information from the credential.

Example uses of the BC Person credential are plentiful:

* Collecting the name of a person opening a bank account.
* Collecting the name of a new hire joining a company.
* Providing the name of a person requesting a Criminal Records Check.
* Completing an online form requiring the entry of data in the credential.
* Verifying the person is a resident of BC for a discount on goods.
* Verifying a person is of age to, for example, purchase alcohol.

## Contact for Additional Information

For more more information about the use this document please contact the Ministry of Citizens’ Services using this email address: [idiminfo@gov.bc.ca](mailto:idiminfo@gov.bc.ca)

## Sample Presentation Requests
