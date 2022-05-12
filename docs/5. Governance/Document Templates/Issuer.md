# Issuer

## Introduction

Describe the issuance of the credential in the context of the issuer. Remember that the reader should also be looking at the schema as a reference.

## Technical Information

### Ledger Information

* Ledger: Link to Ledger
* Issuer DID for the SCHEMA verifiable credential: &lt;DID with Link to Ledger Txn>
* Credential Definition ID: &lt;CRED_DEF ID with Link to Ledger Txn>
* &lt;Link to Overlays Capture Architecture: Source>
* &lt;Link to Overlays Capture Architecture: Published>

## Authority to Issue

Why is the issuer an authority?  From where is the authority delegated?

## The Issued Verifiable Credential

Provide an overview of what data from the issuer is provided to the holder.

### Issuer-Specific Credential Information

The following sections describes the differences between the [Schema documentation](../README.md) and the verifiable credentials issued by ISSUER.

#### Attributes Not Published

List attributes that are NEVER published and what is put into the credential in their place (usually ""). 

* photo_id: The value `""` is issued in all cases.

#### Attributes Handled Differently

List the attributes of the SCHEMA that are published but in a manner different from what is defined in the SCHEMA document.

* All name-related items (full_name, given_name, given_names and surname) are in CAPITAL letters.

### Holders

Describes the set of Holders that could receive this Verifiable Credential.

#### Pre-Issuance Verification

Prior to issuing the ISSUER SCHEMA credential, the Issuer does the following verification of the Holder:

* List the pre-issuance verification process performed

### Revocation

Revocable: Yes/No

If yes, provide details, a list of the circumstances under which a credential would be revoked.

* The credential was issued in error.

## Intended Use of the ISSUER SCHEMA Credential

Describe where the credential from this specific issuer is likely to be used.

## Contact for Additional Information

For more more information about the use this document please contact the Ministry of Citizens’ Services using this email address: [me@example.com](mailto:mme@example.com)

## Sample Presentation Requests

### Use Case: NAME OF USE CASE

Describe the use case and details about the presentation request.

```jsonc
"requested_attributes" : [
	{
		"names": ["full_name", "birthdate_dateint"]
		"restrictions": [
			{ "creddef_id" : "id_of_the_creddef" }
		]
	},
],
"requested_predicates" : []

```
