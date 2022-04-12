# DRAFT Layer 4 Verifier GF: BC Government Verifier of BC Person and LSBC Membership Credentials

## Introduction

This document is a Governance Framework (GF) created to inform those presenting claims from verifiable credentials issued by the Government of British Columbia (BC Person) and the Law Society of British Columbia (LSBC Membership) to the Government of British Columbia’s Ministry of Justice (MoJ) for gaining access to MoJ-provided services.

The document covers details such as:



* The business purpose for requesting the claims,
* the set of holders asked to share these claims,
* the authority of the Verifier to request the claims,
* the claims requested,
* additional business validation performed on the claims after verification,
* how the claims are stored and/or used, and
* with whom the claims are shared.

This governance framework has been developed in accordance with the[ Trust Over IP's Governance Metamodel Specification](https://trustoverip.org/permalink/ToIP-Governance-Metamodel-Specification-V1.0-2021-12-21.pdf).


## References:

This document references the following Trust over IP Governance Documents.

### ToIP Layer 4 GFs:

* [DRAFT Layer 4 Credential Issuer GF: BC Government Issuer of BC Person Credential](../../Credentials/BCGov/BCPerson.md)
* DRAFT Layer 4 Credential Issuer GF: LSBC Issuer of LSBC Membership Credential


## Assumptions, Terminology and Notation

Readers of this document are assumed to be familiar with the concepts of verifiable credentials, Trust over IP, the participants in the exchange of verifiable credentials (issuers, holders and verifiers) and the underlying technology in those exchanges.

A glossary covering verifiable credentials and Trust over IP concepts can be found [here](https://trustoverip.github.io/toip/glossary).


## Localization

The standard language for this governing framework is Canadian English. A translation into Canadian French will be made available at a later date.


## Overview:

The BC Ministry of Justice (MoJ) requests the presentation of claims from Holders requesting access to the MoJ Access to Audio system.



* Purpose: To authorize access to the service(s) based on having a high level of assurance of the name of the person and that they are an active Lawyer in the Province of British Columbia.
* Source Credentials: Claims are requested from credentials issued by the  Government of British Columbia and the Law Society of British Columbia (LSBC).


## Holders Presenting Claims:

The Holders presenting claims must:



* Be residents of British Columbia and have a valid (not revoked) BC Person credential.
* Be a member of the Law Society of British Columbia with an active membership, meaning they are currently authorized to practice Law in the Province of British Columbia, and have an active (not revoked) LSBC Membership credential.

Those without non-revoked instances of those credentials should not request access or respond to the presentation request if they request access.


## Authority to Verify

Access to certain MoJ services are limited to authorized users only. The use of verifiable credentials is the method used to verify the authorization of one category of users of the MoJ services — Lawyers with active certifications from the Law Society of British Columbia (LSBC).


## Presentation Request(s)

The presentation request is as follows:



* Requested attributes:
    * Names: surname, givenNames
        * Restrictions: BC Person credential issued by the Government of British Columbia (see [References](#references) section for issuer information)
    * Names: surname, membershipNum
        * Restrictions: LSBC Membership credential issued by the Law Society of British Columbia (see [References](#references) section for issuer information)
* Predicates:
    * None
* Self-Certified Attributes:
    * None


### Verification and Validation:

The presentation must pass cryptographic verification, including that the credentials are not revoked, and that the credentials were issued based on the same linked secret.

After verification, the following validation checks are performed:



* All requested attributes must be revealed.
* The two “surname” fields must match.


## Use of the Collected Claims

The collected claims from the presentation are used for the following purposes:



* Authentication: The verification and validation of the credentials is evaluated for granting access to the protected service.
* Auditing: The GivenNames, surname and MembershipNum are recorded in the audit log records recorded about the actions taken by the user in using the service.
    * Audit records are used in the forensic analysis of incidents discovered about the use of the service.


## Sharing of Collected Claims with Others

When potential breaches of security, privacy are detected, or there are incidents of unauthorized use of the service, data recording in the audit logs, including data from claims, MAY be shared with the Law Society of British Columbia to further identify and collect additional information about the user, including contact information (e.g. Law Firm, telephone number, email address, mailing address, etc.).


## Additional Information:

For more more information about the use this document please contact the Ministry of Justice using this email address: [mojcio@gov.bc.ca](mailto:mojcio@gov.bc.ca).


## Technical Information:


### Ledger Information:

Ledger: [CANdy-Dev](https://candyscan.idlab.org/home/CANDY_DEV)

Verifier Public DID: &lt;to be added>
