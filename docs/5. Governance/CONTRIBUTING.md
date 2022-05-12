# Contribution Policy

This document provides the contribution policy for managing the contents of this
ToIP Layer 4 Pan-Canadian Verifiable Credential Ecosystem Governance Framework repository.

## Contribution Guidelines

Contributions to this governance framework must be made via pull requests to the
GF's GitHub repository
[https://github.com/cloudcompass/demo-pancdn-toip-gf](https://github.com/cloudcompass/demo-pancdn-toip-gf).
The following section outlines the process for merging contributions ot this
Repository.

### Issues/Pull Requests

Issues and pull requests are used as the primary method for tracking anything to
do with the documentation and governance of this ecosystem. A pull request is
treated exactly the same as an issue with a specific proposed change to
documents within the ecosystem governance GitHub repository. An issue may be
created that later spawns a related pull request.

#### Issue/Pull Request Types

There are three types of issues/pull requests (each with their own corresponding label):

##### Discussions

Discussions are support or functionality inquiries that we want to have a record of
for future reference. Depending on the discussion, these can turn into "Layer X
GF Change" issues, where "X" is 1, 2, 3 or 4.

##### Proposals

Proposals are for new ideas that impact the ToIP Layer 4 GF itself, and for
ToIP Layer 1 and 2 updates that may impact all participants in the ecosystem.
Changes at Layers 1, 2 and 4 require a larger discussion amongst all of the
authorities within the eco-system, as they impact the policies of the ecosystem.
Example of such issues include:

* Changes to this Contributing document, or the overview of how the ecosystem
  governance framework operates or should be used.
* The addition of new ToIP Layer 1 utility ledgers to be used by verifiable
  credential Issuers in the ecosystem, and hence required by Holders and
  Verifiers interested in consuming those verifiable credentials.
* An update to the set of ToIP Layer 2 protocols used by the ecosystem participants.
* Updates to the template documents used at the ToIP Layer 3 level, especially
  if they impact existing ToIP Layer 3 governance documents.

Such issues/pull requests allow for feedback from the relevant ecosystem
authorities before changes are made to the Governance Framework itself or the
underlying ToIP Layers of the ecosystem that impact all participants. All issues
and pull requests that are proposals should both have the "Proposal" label and
title of "Proposal: [the rest of the title]." A proposal can become a "Layer X
GF Change".

Proposal pull requests are merged when consensus has been reached amongst the relevant ecosystem authorities.

##### ToIP Layer 3 Document Changes

ToIP Layer 3 documents are "owned" by one participant in the ecosystem and being
shared with other participants. Owner, in this context means

* The publisher of a given Schema
* The Issuer for a given credential type
* The Verifier requesting data from a given set of credential types

The contents of a given ToIP Layer 3 document is primarily the concern of the owner of
the document. The role of the repository Editors/Maintainers in merging such
pull requests is one of facilitator rather than editor. Specifically, the review
process for such pull requests must cover only:

* Confirming that the contributor has a role within the organization of the
  document owner, or the pull request has been approved by a contributor that
  has a role within the organization of the document owner.
  * This is to prevent others altering the documents without authorization by
    the document owner's organization.
* Ensuring that the content of the document is appropriate to the purpose, such
  as making sure the appropriate Layer 3 template has been used as intended and
  is complete.
  * This is to ensure that there is consistency in what is being published by
    the participants.

All participants, including editors and maintainers, may make comments and
suggestions about the pull request contents, but merging is ultimately up to the
document owner, beyond the editorial facilitation described above.

## Issue/Pull Request Lifecycle

The issue and pull request lifecycle is mainly driven by the Editors and
Maintainer(s) as defined by the  All issue types follow the same general lifecycle. Differences
are noted below.

### Issue/Pull Request Creation

An issue or pull request is created.

### Triage

One of the Editors triages the contribution and applies the proper labels for
the issue. This includes labels for priority, type, and metadata, and (if
needed) cleans up the title to include the type and to succinctly and clearly
state the issue.

If a pull request is to a Layer 3 document, is submitted by a person known to
have a role in the document owner's organization and the content is deemed
appropriate by the Editor, the pull request can be both approved and merged
immediately.

If not, the editor processing the issue/pull request publicizes the contribution
appropriately, such as tagging interested parties or adding the topic for
discussion at an upcoming meeting. 

### Discussion

Interested parties review the issue/pull request and contribute in the
issue/pull request to the discussion. As appropriate, the topic is covered in
meetings, with notes about the discussion added to the topic.

A contributor may volunteer or be assigned to create a pull request for an
issue, to make concrete the action to be taken.

The issue/pull request should remain open until consensus is reached that it is
resolved, with the Editors working to close the topic as soon as possible.

The contributor of a pull request is expected to be responsive to the discussion
around the pull request, submitting updates or replying with comments to address
feedback provided by both the Editors and other contributors.

### Closure

When the consensus is reached on an issue/pull request, the issue is closed.  A
contributor that disagrees with the consensus may re-open the issue/pull request
to restart the discussion.
