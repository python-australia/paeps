---
PAEP: 1
Title: PAEP Purpose and Guidelines

Authors: Alyssa Coghlan, Elena Williams

Created: 2025-03-16
Resolved: [2025-08-31](https://github.com/python-australia/paeps/pull/7#issuecomment-3241276245)

State: Active
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

## Pronunciation

Discussing the PAEP process at PyCon Australian 2025 made it clear that some level of consensus on
how to pronounce "PAEP" would be helpful. The suggested pronunciation is "pay-ep", but we're mostly
Australians, so it's inevitable it will frequently be shortened to the single syllable "pape".

# When is a formal process needed?

Many decisions relating to Python Australia may be made without needing a formal PAEP or approval
vote. For example, if someone wants to talk at their local user group about the efforts
that are being made to establish Python Australia and some of the hoped for benefits of getting
such an organisation in place, that's not something that needs anyone else's permission.
Similarly, editorial updates to the Python Australia website, or even the explanatory portions of
process PAEPs, may take place through regular source update review tools.

Instead, the PAEP and approval vote mechanisms exist to allow decisions to be made in situations
that members feel they *can't* reasonably resolve as individuals, rather than requiring that
*everything* use these processes.

If we're thinking "It would be good if X happened, I'm willing to spend time on X, but I don't
think I have the right to do X on Python Australia's behalf", then that's the kind of situation
these processes are designed to help resolve.

And if we're not sure, we can just ask other members if they feel a particular question should be
escalated before we follow through on doing anything about it.

# PAEP Approval Processes

The approval processes described in this section may be used for the following purposes:

* directly approving (or rejecting) a submitted PAEP
* nominating a decision making delegate (or delegates) for a given PAEP
* making decisions which do require some level of consensus, but not the full complexity of a PAEP

Specific examples of the last category would be the decision to switch the PAEPs repository
from being a private GitHub repository to being a public one, as well as the acceptance of
`pythonaustralia.org` as the domain for Python Australia's initial web presence.

## Prior to the establishment of a formal organisation

In the absence of a formal Python Australia organisation, an interim approval process is
required to support making the collective decisions needed to establish a cohesive formal
organisation in the first place.

To serve that purpose, we define the concept of "Potential Founding Members". These are
individuals that will be offered the opportunity to become the actual founding members of
the formal organisation when it is established.

### Potential Founding Members

The roster of Potential Founding Members aims to include those individuals that are already
actively involved in organising the Australian Python community, as these are the folks the
proposed organisation primarily aims to support. This group includes Python user group
organisers, community workshop organisers, conference organisers, and other individuals that
have been invited to actively participate in the development and establishment of a formal
Python Australia organisation.

The initial set of Potential Founding Members was established following PyCon Australia 2024,
when Elena Williams, Nic Crouch, and Jack Skinner brought together a group of existing organisers
and open source contributors in the Australian Python community to discuss the possibility of
establishing a formal Python Australia organisation.

New Potential Founding Members are added via nomination by an existing Potential Founding Member,
with that nomination then being supported by at least one other Potential Founding Member.

The roster of Potential Founding Members is maintained as the list of individuals that have
received (and accepted) an invitation to the "PyAU" Discord server. This is likely to be
transferred to a platform independent format at a later date, but this mechanism is considered
sufficient as a pragmatic starting point. It is also plausible that Discord may be replaced
with a more open, locally controlled communications platform. Future approval for either of
those changes will use the mechanisms described in this PAEP.

Note: separately from the Potential Founding Members, a more open invitation has been issued to
folks that are interested in signing up as members of the new organisation once it exists, without
necessarily being directly involved in the details of establishing that organisation. Folks
accepting that broader invitation are free to comment on PAEPs and other aspects of the proposed
formal organisation, but aren't able to directly participate in approval polls.

### Approval by polling the Potential Founding Members

Polls of the Potential Founding Members use the polling mechanisms of the chosen communication
platforms.

Initially, this means the use of *open* ballots in the "PyAU" Discord server.
A dedicated `#votes` channel has been established for this purpose, together with a dedicated
`#votes-discussion` channel for any related questions and clarifications.

PAEP authors are free to publish non-binding polls in other channels to help inform the
PAEP development process.

Approval polls use a "threshold with veto" voting mechanism inspired by the +1/+0/-0/-1 style
Apache voting process:

* Approve (+1)
* Abstain, mildly in favour (+0)
* Abstain, not in favour (-0)
* Veto (-1)
* Abstain, not expressing a perspective

In order to pass, an approval poll must receive at least 5 votes for approval, and NO
vetoes. Allowing vetoes is intended to be the equivalent of an "Emergency Stop" button on an
industrial site: each Potential Founding Member is trusted with the authority to say
"We're about to make a serious mistake here, let's stop and consider this further".

Abstentions (whether explicit votes to abstain, or implicitly abstaining by failing to vote)
do not affect the outcome of the ballot. When explicitly abstaining, members may still indicate
whether or not they favour the proposal, even if they don't feel strongly enough about it to
either assist in meeting the approval threshold or to invoke their veto.

Rejection of a proposal may occur either via a "collective 'Meh'" (failing to reach the
approval threshold), or by a Potential Founding Member invoking their veto.

If a Potential Founding Member invokes their veto, they are expected to provide the
rationale for their veto, and indicate if they consider the proposal irredeemably flawed,
or if their concern is with specific details of the proposal that could be amended without
having to discard the overall proposal.

Based on the details of the feedback associated with a failed approval vote, PAEP Authors may
either choose to accept the rejection as final, or else revert the proposal to a Draft state and
then resubmit it for approval after making suitable amendments.

Approval polls MUST remain open for at least 7 days, and MAY remain open for up to 14 days.

For PAEP approval ballots, the poll question should provide the PAEP title and link to the PAEP text
for details.

For other decision approval ballots, the question should be simple enough that it can be included
directly in the poll definition. If more background is required than can be reasonably included in
the poll question, it indicates that using the full PAEP process may be more appropriate.

If an alternative communications platform is set up, the approval polls may be switched to that
platform using the mechanisms described in this PAEP.

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

The authors of a PAEP are responsible for building consensus within the community and documenting
dissenting opinions.

If one or more approval delegates are nominated, their role is recorded in the PAEP metadata.

When a PAEP is resolved (whether via approval or rejection), the resolution date will be added to
the PAEP metadata, with a link to the details of the resolution. If the PAEP is resolved in a forum
which does not support public URL references (such as a private Discord server), then the resolution
will be recorded in an issue or PR comment on the PAEPs repository, and the PAEP metadata will link
to the relevant issue/PR.

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
