# VitaSDK Governance

VitaSDK is a volunteer-driven project. This document defines the minimum process needed to keep important decisions transparent and reviewable without adding unnecessary bureaucracy.

Technical judgment, relevant expertise, and discussion are preferred over formal voting. Voting is used when maintainers cannot otherwise resolve a disagreement.

## Maintainers

The VitaSDK GitHub organization membership is the source of truth for current maintainer status.

Maintainers may have different areas of expertise and involvement. Maintainer status does not imply equal expertise or responsibility across every repository. Technical decisions should, whenever possible, involve maintainers familiar with the affected area.

For governance purposes, an **active maintainer** is a maintainer who has meaningfully participated in VitaSDK during the preceding six months. Participation may happen on GitHub or through the project's usual communication channels and may include development, review, technical discussion, releases, infrastructure, coordination, or other maintenance work.

There is no numerical activity threshold.

A **historical maintainer** is a former VitaSDK maintainer who remains in good standing with the project. A maintainer who becomes inactive remains a maintainer unless they resign or are removed under this governance.

### Becoming a Maintainer

New maintainers are generally selected from contributors who have demonstrated sustained involvement, technical judgment, and familiarity with VitaSDK or the broader Vita development ecosystem.

Relevant experience may include repeated technical contributions, constructive reviews and discussions, maintenance of Vita-related projects, or other established work in the Vita community.

Any active maintainer may propose a new maintainer through the project's usual communication channels. In normal circumstances, appointment requires:

- explicit support from at least one other active maintainer; and
- no unresolved substantive objection.

If only one maintainer is currently active, the appointment must instead receive support from at least one historical maintainer in good standing.

There is no public application or nomination requirement. Once agreed, an appointment should be publicly recorded or announced.

A maintainer may resign at any time without approval.

## Pull Requests

Significant changes should be submitted through a pull request, including changes made by maintainers.

Direct pushes are acceptable for trivial changes and for repositories that are experimental, temporary, or otherwise not yet relied upon by the VitaSDK community.

The origin of a pull request does not affect its review requirements.

In normal circumstances, approval from one maintainer is sufficient to merge a pull request.

Maintainers should not merge their own pull requests without independent maintainer approval.

Previous approval is sufficient when a pull request faithfully implements an accepted RFC or another clearly documented decision that already received independent maintainer approval. If the implementation introduces material decisions outside the approved scope, normal review or the RFC process applies.

Contributor reviews are welcome and should be considered according to their relevance and expertise, but they do not replace maintainer approval where this governance requires it.

Any maintainer may require a proposed change to go through the RFC process before it is merged. The maintainer requesting an RFC should explain why broader review is warranted.

A substantive disagreement between maintainers therefore moves the proposed change to the RFC process.

Rebase-and-merge should normally be used when integrating pull requests in order to preserve a linear project history.

## RFCs

An RFC is a GitHub issue marked with the `rfc` label. Anyone may propose one.

Opening an RFC does not imply endorsement.

An RFC should describe the problem, proposed change, expected impact, and relevant alternatives or tradeoffs clearly enough for maintainers to make a decision.

### When an RFC Is Required

RFCs are required for:

- breaking changes to a public API or ABI;
- significant architectural changes;
- significant reductions in existing compatibility or support;
- changes to licensing or contribution policy;
- organization-wide project policy;
- any modification to this governance document; and
- any other change that a maintainer reasonably determines needs broader project review.

Routine maintenance, dependency updates, internal refactoring, and other changes that preserve existing behavior normally do not require an RFC.

### Discussion and Final Objection Period

RFC discussion is public. Anyone may provide feedback, technical advice, or context.

Only maintainers may raise a **formal objection** that blocks acceptance. A concern raised by another community member may become a formal objection if a maintainer adopts it.

Maintainer objections should be reasoned.

An RFC enters a **three-day final objection period** after receiving explicit approval from a maintainer other than the proposer. This approval means the RFC is mature enough to finalize; it does not require enthusiastic support.

If no formal objection remains unresolved when the period expires, the proposer may mark the RFC as accepted.

If an objection is raised, the RFC returns to discussion. After the concern is resolved or the proposal is revised, a new approval from a maintainer other than the proposer starts a fresh three-day final objection period.

### Deadlocks and Voting

Maintainers should first try to resolve disagreements through discussion and revision.

If an objection cannot be resolved, a strict majority of maintainers active during the preceding six months may override it. All active maintainers may participate, including the proposer and the maintainer who raised the objection.

Once the required majority is reached, a new three-day final objection period begins.

An objection that has already been explicitly overridden by the required majority does not block the RFC again unless new information or new grounds are raised.

A strict majority of active maintainers may also reject an RFC.

Maintainer positions may be recorded using 👍 or 👎 reactions on the RFC issue. Votes expressed through Discord or another usual project communication channel are also valid if they are recorded on the RFC issue with the maintainer and position identified.

Only maintainer votes count for governance decisions. The latest recorded position of each maintainer counts.

### Withdrawal and Inactivity

The proposer may withdraw an RFC at any time before acceptance.

An RFC that has not been accepted and has had no meaningful activity for six months may be closed as inactive by any maintainer.

Closing an RFC as inactive is not rejection and does not prevent it from being reopened or proposed again later.

### Implementation

An accepted RFC remains open while it is being implemented.

Implementation pull requests should reference the RFC. Once all required implementation work has been merged, the proposer or any maintainer may close it.

Implementation must remain within the scope of the accepted decision. A material change outside that scope requires its own RFC.

Materially changing, reversing, or superseding an accepted RFC decision also requires a new RFC.

An accepted RFC is not closed merely because implementation is taking a long time while the accepted work remains ongoing.

## Repository Lifecycle

Maintainers may freely create or remove repositories used for experiments, prototypes, migrations, testing, or other temporary project work.

When such work relates to an issue or RFC, that issue or RFC should reference the repository. A proposal does not need to be accepted before experimental development begins.

Creating an experimental repository does not imply adoption by VitaSDK.

Once a repository has been adopted or is relied upon by the VitaSDK community, archiving or deleting it should normally result from an accepted RFC or another previously approved change that makes the repository obsolete.

Archiving or deleting such a repository is implementation of the underlying decision and does not require a separate governance decision.

## Licensing

New original VitaSDK projects use the MIT License by default.

Projects based on, derived from, or incorporating third-party software must use licensing compatible with the applicable upstream terms and preserve required notices and attribution.

When those constraints do not determine otherwise, MIT remains the default.

Choosing a different license for new original VitaSDK software, changing the license of an existing project, or materially changing project-wide contribution or licensing rules requires an RFC.

Contributors and maintainers are responsible for ensuring that externally sourced material may be legally incorporated and distributed under the applicable project terms.

Existing repositories retain their current licensing unless changed through the RFC process.

## Maintainer Removal

A maintainer may be removed for serious or repeated violations of project rules, abuse of project access, conduct that materially harms the project or its community, or another serious breach of project trust.

Inactivity alone is not grounds for removal, and removal must not be used to settle ordinary technical or personal disagreements.

Removal requires the support of a strict majority of maintainers active during the preceding six months.

The maintainer whose removal is being considered does not participate in the decision and is not counted when determining the required majority.

### Temporary Suspension

When there is a credible risk of immediate harm to the project, repositories, or organization, a maintainer's access may be temporarily suspended while the situation is reviewed.

The suspension must be carried out or explicitly approved by an active maintainer other than the person raising the concern. The maintainer whose conduct is under review does not participate in approving their own suspension.

A temporary suspension may last for no more than seven days and may not be extended.

Before that period expires, the normal maintainer removal process must reach a decision. If the required majority for removal is not reached, the suspension automatically ends and access must be restored.

Temporary suspension is precautionary and does not itself constitute removal.

## Changes to This Governance

Any modification to this governance document, including minor changes, requires an accepted RFC.

Once the RFC is accepted, the corresponding governance change is implementation of that decision and may be merged under the normal pull request rules.
