# Layer 3 Verifier: BC Ministry of Justice

## Introduction

The BC Ministry of Justice (MoJ) requests the presentation of claims from
Holders requesting access to the MoJ Access to Audio system.

* Purpose: To authorize access to the service(s) based on having a high level of
  assurance of the name of the person and that they are an active Lawyer in the
  Province of British Columbia.
* Source Credentials: Claims are requested from credentials issued by the
  Government of British Columbia and the Law Society of British Columbia (LSBC).

## References

This document references the following Trust over IP Governance Documents.

* [Layer 3 BC Government Issuer of BC Person Credential](../../Credentials/BCGov/BCPerson.md)
* [Layer 3 LSBC Issuer of LSBC Member Credential](../../../Credentials/LSBC/LSBCMember.md)

## Holders Presenting Claims

The Holders presenting claims must:

* Have a valid (not revoked) BC Person credential.
* Be a member of the Law Society of British Columbia with an active membership,
  meaning they are currently authorized to practice Law in the Province of
  British Columbia, and have an active (not revoked) LSBC Membership credential
  showing a status of "Practicing."

Those without non-revoked instances of those credentials should not request
access or respond to the presentation request if they request access.

## Authority to Verify

Access to certain MoJ services are limited to authorized users only. The use of
verifiable credentials is the method used to verify the authorization of one
category of users of the MoJ services — Lawyers with active certifications from
the Law Society of British Columbia (LSBC) and a "person" credential with Level
1 assurance.

## Presentation Request(s)

The presentation request is as follows:

* Requested attributes:
    * Names: surname, givenNames
        * Restrictions: BC Person credential issued by the Government of British
          Columbia (see [References](#references) section for issuer information)
    * Names: surname, membershipNum, membershipStatus
        * Restrictions: LSBC Membership credential issued by the Law Society of
          British Columbia (see [References](#references) section for issuer
          information)
* Predicates:
    * None
* Self-Certified Attributes:
    * None

## Verification and Validation

The presentation must pass cryptographic verification, including that the
credentials are not revoked, and that the credentials were issued based on the
same linked secret.

After verification, the following validation checks are performed:

* All requested attributes must be revealed.
* The “surname” fields from the different source credentials must match.
    * Should the "surname" not match, the user should contact the relevant
      authority (BC Gov or LSBC) to have the source data corrected and a new
      credential issued.
* The "membershipStatus" is checked and MUST be "Active"

## Use of the Collected Claims

The collected claims from the presentation are used for the following purposes:

* The PPID claim is used to match to an existing Account record for the user.
    * The PPID is not used as the identifier on the account; a new identifier for
      the account is created. The PPID becomes an attribute on the account.
    * If no existing Account record is found, a new Account record is created and
      all collected data added as attributes
* The account identifier, givenNames and surname are put into the audit log of
  actions by the user.

* Authentication: The verification and validation of the credentials is
  evaluated for granting access to the protected service.
* Auditing: The GivenNames, surname and MembershipNum are recorded in the audit
  log records recorded about the actions taken by the user in using the service.
    * Audit records are accessible to authorized members of the Ministry of
      Justice team that manage the Access to Audio service.
    * Audit records are used in the forensic analysis of incidents discovered
      about the use of the service.

## Sharing of Collected Claims with Others

When potential breaches of security or privacy are detected, or there are
incidents of unauthorized use of the service, data recording in the audit logs,
including data from claims, MAY be shared with the Law Society of British
Columbia to further identify and collect additional information about the user
in question. In such a situation, the PPID will be shared with LSBC to retrieve
other information about the user, such as contact information (e.g. Law Firm,
telephone number, email address, mailing address, etc.).

## Contact for Additional Information

For more more information about the use this document please contact the
Ministry of Justice using this email address:
[mojcio@gov.bc.ca](mailto:mojcio@gov.bc.ca).

## Technical Information

### Presentation Request

A link to the presentation request can be found here.

### Ledger Information

* Ledger: [Sovrin MainNet](../../../../Layer%201/Sovrin.md)
* Verifier Public DID: &lt;to be added>
