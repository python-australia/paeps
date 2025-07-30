---
PAEP: 1
Title: PAEP Purpose and Guidelines

Authors: Alyssa Coghlan, Elena Williams

Created: 2025-03-16
# Resolved: TBD

State: Draft
---

# What is a “PAEP”?

PAEP is the acronym for a Python Australia Enhancement Proposal.
This model is based on the "Enhancement Proposal" models used by
the [Python core development team](https://github.com/python/peps/) (and associated groups)
and the [Django Software Foundation](https://github.com/django/deps).

A PAEP is a document or small group of artefacts in this repository intended to contain the
concise, specific rationale and technical specifications for
governance, standards, processes, and information for Python Australia.

This format is adopted to:
* encourage transparency
* allow input and ideas to be explored
* formalise consensus gathering

Each PAEP will be designated a positive integer number in consecutive order, per the PAEP register.

# PAEP Approval Processes

The approval processes described in this section may be used for the following purposes:

* directly approving (or rejecting) a submitted PAEP
* nominating a decision making delegate (or delegates) for a given PAEP
* making decisions which do require some level of consensus, but not the full complexity of a PAEP

A specific example of the last category would be the decision to switch the PAEPs repository
from being a private GitHub repository to being a public one.

## Prior to the establishment of a formal organisation

In the absence of a formal Python Australia organisation, an interim approval process is
required to support making the collective decisions needed to establish a cohesive formal
organisation in the first place.

To serve that purpose, we define the concept of "Potential Founding Members". These are
individuals that will be offered the opportunity to become the actual founding members of
the formal organisation when it is established.

### Potential Founding Members

Potential Founding Members are those individuals that have received (and accepted) an invitation
to one of the following communications platforms:

* the "PyAU" Discord server;
* the "python-australia" GitHub organization;
* any other shared communication channel that is established prior to setting up the formal organisation
  (preferably this will include a more free-software compatible platform, such as a Zulip or Discourse instance).

New Potential Founding Members are added via nomination by an existing Potential Founding Member,
with that nomination then being supported by at least one other Potential Founding Member.

The initial set of Potential Founding Members was established following PyCon Australia 2024,
when Elena Williams, Nic Crouch, and Jack Skinner brought together a group of existing organisers and
open source contributors in the Australian Python community to discuss the possibility of establishing
a formal Python Australia organisation.

### Approval by polling the Potential Founding Members

Polls of the potential founding members will use the polling mechanisms of the available communication platforms.

Initially, this will mean the use of *open* ballots in the "PyAU" Discord server.
A dedicated `#approval-polls` channel will be established for this purpose.

Approval polls must be yes/no polls, decided by a simple majority. PAEP authors are free to publish
more complex non-binding polls in other channels to help inform the PAEP development process.

Approval polls MUST remain open for at least 7 days, and MAY remain open for up to 14 days.

For PAEP approval ballots, the poll question should provide the PAEP title and link to the PAEP text
for details.

For other decision approval ballots, the question should be simple enough that it can be included
directly in the poll definition. If more background is required than can be reasonably included in
the poll question, it indicates that using the full PAEP process may be more appropriate.

If an alternative communications platform is set up, this section may be amended via the PAEP process to
switch the approval polls to that platform.

### Approval by delegation

Rather than requesting that a PAEP be approved directly, an approval poll may instead propose that
the final decision on the PAEP be delegated to an individual or a small group of individuals. This
is most appropriate when there is broad consensus in favour of the general *idea* behind a PAEP,
but also several fiddly implementation details which need to be resolved before the PAEP can be
finalised.

In these cases, the poll question should provide the PAEP title, the names of proposed delegates,
while still linking to the PAEP text for details. The poll should also provide some rationale
for why the delegation is considered appropriate for the affected PAEP.

## After the establishment of a formal organisation

Once a formal Python Australia organisation has been established, formal approval authority
for PAEPs will rest with the governance structure established in the constitution and
by-laws of that organisation.

Most notably, the governing Board of the formal organisation is likely to take over the
role filled by the full roster of Potential Founding Members in the interim approval process.

# Additional Process Details

## Proposal metadata

```
PAEP number: `int` (per PAEP register)
Title: short text

Author(s): person/people
Approval Delegate(s) (optional): person/people

Created: `date`
Resolution: `date` (with URL reference) | None

State: `state`

Requires (optional): `int` (per PAEP register)
Replaces (optional): `int` (per PAEP register)
Superseded-by (optional): `int` (per PAEP register)
```

`state` is process PAEP state, see section: PAEP states.

The authors of a PAEP are responsible for building consensus within the community and documenting dissenting opinions.
If one or more approval delegates are nominated, their role is recorded in the PAEP metadata.

When a PAEP is resolved (whether via approval or rejection), the resolution date will be added to the PAEP metadata,
with a link to the details of the resolution. If the PAEP is resolved in a forum which does not support URL references
(such as Discord), then the resolution will be recorded in an issue on the PAEPs repository, and the PAEP metadata
will link to that issue.

## Proposal states

**Open**
* Draft
* Submitted

**Approved**
* Active (approved, used directly as a reference document)
* Accepted (approved, proposed changes are in process)
* Final (approved, proposed changes have been completed)

**Closed**
* Rejected (submitted for approval, but was not approved)
* Withdrawn (authors chose not to submit for approval)
* Deferred (authors chose not to submit for approval *yet*, but may submit later)
* Superseded (replaced by another PAEP)

These states largely match those defined in [PEP 1](https://peps.python.org/pep-0001/),
with the addition of the "Submitted" state for PAEPs which have been submitted
for approval.

There is no prescribed timeline for PAEP processing, *except* that the "Submitted"
state is expected to last no less than 7 days and no more than 14 days
(as described for approval ballots above).
