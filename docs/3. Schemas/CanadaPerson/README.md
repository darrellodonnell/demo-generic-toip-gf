# Canada Person Schema

## Introduction

The Canada Person Schema described in this document was created as a result of a collaboration between the governments of BC, PROVINCE2 and PROVINCE3 for the purpose of enabling provinces to become an issuer of the credential. Credentials issued based on this schema contain authoritative digital identity data attributes about the Holder held by the issuer, such as their name and date of birth (see full list of attributes below).

## Technical Information

### Ledger Information

* Ledger: [CANdy-Dev](https://candyscan.idlab.org/home/CANDY_DEV)
* Schema Creator DID: &lt;DID with Link to Ledger Txn>
* Schema ID: &lt;SCHEMA ID with Link to Ledger Txn>
* &lt;Link to Overlays Capture Architecture: Source>
* &lt;Link to Overlays Capture Architecture: Published>


## Governance Information

The "Governance Framework" information for this schema is defined in [this document](https://docs.google.com/document/d/1wXp7paqotrsQeC0ZZnpvAeFjkPIYHv5NQO-euIdL3jo/edit) developed jointly by representatives of the Governments of BC, PROVINCE2 and PROVINCE3.

## The Canada Person Credential Schema

The Canada Person Credential Schema is defined to allow the issuance of a credential that provides the Holder with the core digital identity attributes held by an jurisdictional authority about the resident of the jurisdiction, such that the Holder can share those attributes with the verifiers of their choice.

The specific attributes in the credential about the subject include the following and are intended to come from the current digital identity record about the Holder. Technical details about each of the attributes follow in this section of the document.

An Issuer MAY choose to populate only a subset of the attributes in a verifiable credential based on this schema and SHOULD structure the content of populate attributes as described below, if at all possible. The Issuer MUST publish a document about how they use this schema that includes any attributes not populated and any attributes populated differently from what is described below.

### full_name

### given_names

A UTF-8 encoded string containing the names of the Subject, excluding the surname. If the Subject of the credential has only a single name (a mononym), the givenNames field will be an empty string (“”). If the person has multiple names, the names are in order (e.g. first name, first middle name, etc.), space-separated. No differentiation is made for a single name with or without spaces. For example, the value of giveNames is the same for a person having just a first name of “Jim Bob” and a person with a first name “Jim” and a single middle name “Bob”. 

### given_name

### surname

A UTF_8 encoded string containing the surname of the Subject. The attribute may not be blank in an issued credential.

### birthdate_dateint

An integer obtained by converting the date of birth of the credential subject into an integer of value “YYYYMMDD.” For example, the date June 12, 1993 is converted to the integer `19930712` (or `19,930,712`). This is the recommended format for dates to enable the use of AnonCreds predicates for proving (for example) the person is a given age based on the dob_dateint value without having to reveal the value. This reduces the possibility of correlation across verifiers that must know of the Subject is older than a given age. This format is described in the [Hyperledger Aries RFC 0441 Present Proof Best Practices](https://github.com/hyperledger/aries-rfcs/blob/main/concepts/0441-present-proof-best-practices/README.md).

### parent_1_full_name

### parent_2_full_name

### identification_level

The “Level of Assurance” (LOA) about the collection of the data included in the credential. The LOA is a number from 1-4 and is based on the LOA definition in the Pan Canadian Trust Framework, Public Sector Profile V1.1, which can be found [here](https://canada-ca.github.io/PCTF-CCP/Version1_1/).

### full_civic_address

### civic_address

### civic_number

### street_name

### city_name

### province_name

### postal_code

### photo

### issue_date_dateint

An integer obtained by converting the date the credential was issued into an integer of value “YYYYMMDD.” For example, the date June 12, 2022 is converted to the integer “20220712”. This is the recommended format for dates to enable the use of AnonCreds predicates for proving (for example) the credential has already been issued. This reduces the possibility of correlation across verifiers that require proof that the credential is past its issue date. This format is described in the [Hyperledger Aries RFC 0441 Present Proof Best Practices](https://github.com/hyperledger/aries-rfcs/blob/main/concepts/0441-present-proof-best-practices/README.md).

### expiry_date_dateint

### issuing_jurisdication


## Intended Use of the Canada Person Credential

The Canada Person credential is intended to allow a Holder to prove that they are a resident of the issuing jurisdiction (possession of the credential), and to provide authoritative demographic information about themselves to a verifier.

Note that all of the demographic information in the Person credential is Personally Identifiable Information (PII) and as such,

* The Holder should take care in deciding with whom they share the information, and for what purpose.
* Verifiers receiving the information MUST handle the data in a manner consistent with the Privacy Laws of the jurisdiction in which they operate, and the (if different) the jurisdiction of the issuer of the credential.

Example uses of this credential are plentiful:

* Collecting the name of a person opening a bank account.
* Collecting the name of a new hire joining a company.
* Providing the name of a person requesting a Criminal Records Check.
* Completing an online form requiring the entry of data in the credential.
* Verifying the person is a resident of a jurisdiction and is thus entitled to a discount on a product or service.
* Verifying a person is of age to, for example, purchase alcohol in a jurisdiction.

Verifiers MUST NOT request attributes from the credential for purposes where they are not needed. For example, when verifying the age of a person when purchasing alcohol, the credentials issued based onthe Canada Person Credential schema can be used to prove the person is over the age of 19 without sharing any other information from the credential. Sample presentation requests are provided in the 
[Technical Information](#sample-presentation-requests) section of this document.

## Contact for Additional Information

For more more information about the use this document please contact the publisher of this Schema, the BC Ministry of Citizen Services using this email address: [idiminfo@gov.bc.ca](mailto:idiminfo@gov.bc.ca)

## Sample Presentation Requests:

