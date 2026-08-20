# Contributing to VitaSDK

Thank you for contributing to VitaSDK.

These guidelines define the common contribution requirements across VitaSDK repositories. Individual repositories may have additional build, testing, formatting, or development requirements.

## Pull Requests

A separate issue is not required before opening a pull request.

Changes requiring broader project approval must follow the RFC process defined in VitaSDK Governance.

### Pull Request Description

Pull requests must explain:

- what the change does;
- why the change is needed; and
- how the change was tested.

Relevant compatibility considerations and related issues or RFCs should also be included when applicable.

## Scope

Pull requests should focus on a coherent change.

Unrelated refactoring, formatting, cleanup, or functional changes should not be mixed into the same pull request unless directly required.

Large changes may be split when doing so makes review or testing easier.

## Draft Pull Requests

Work-in-progress contributions may be opened as draft pull requests for early feedback, testing, or coordination.

Draft pull requests are not ready for final review or acceptance until marked as ready for review.

## Testing

Changes must be tested in an environment appropriate for the behavior being modified.

Real PlayStation Vita hardware may be required when the relevant behavior depends on hardware. Vita3K may be sufficient when the change can be meaningfully validated there.

Host-side changes, documentation, CI, and similar changes do not require Vita hardware testing when it is not relevant.

Testing may be performed by the contributor, a maintainer, or another community member, provided the result is recorded in the pull request.

When a repository has an existing test suite, contributors may be required to add or update tests when appropriate.

## Continuous Integration

Pull requests should pass required CI checks before they are merged.

A failing check may be disregarded when it is clearly unrelated to the change or otherwise not applicable. The reason should be documented in the pull request.

## Compatibility

Contributions should preserve existing public APIs, ABIs, supported behavior, and compatibility whenever reasonably possible.

Intentional breaking changes must follow the RFC process defined in VitaSDK Governance.

## Commit History

Contributions should have a clean, linear commit history.

Pull request branches must not contain merge commits. Contributors should rebase onto the target branch when necessary rather than merging the target branch into their branch.

A pull request does not need to be rebased solely because the target branch has advanced. Rebase may be required when there are conflicts or the branch has become materially outdated.

Commits should be logically organized and use clear, descriptive messages.

VitaSDK does not require Conventional Commits or another fixed commit message format.

Maintainers may ask contributors to rebase, squash, split, or otherwise clean up commits before merge.

## Code Style

Contributions should follow the existing style and conventions of the repository and surrounding code.

Repository-specific formatting, linting, or development tools should be used when available.

VitaSDK does not impose a single organization-wide code style.

## Third-Party Material

Contributions incorporating or adapting external code, data, headers, NIDs, documentation, patches, or other material must identify the original source in the pull request.

The license of the external material must also be stated, including the specific version when applicable. SPDX identifiers should be used when possible.

Third-party material must not be incorporated when its license is incompatible with the target repository or would impose additional licensing requirements that VitaSDK has not explicitly agreed to accept.

Material with an unknown, unclear, or missing license must not be copied or adapted unless permission to use and distribute it can be demonstrated.

Required copyright notices, attribution, license text, and other conditions must be preserved in the repository or distribution when required. Attribution only in the pull request is not sufficient in such cases.

Changes that would require relicensing a VitaSDK project or introduce broader licensing obligations must first follow the RFC process.

Sources should also be identified when material comes from reverse engineering, public documentation, another open-source project, or similar technical research.

## AI-Assisted Contributions

AI-assisted development tools may be used when contributing to VitaSDK.

If AI tools or models were used to prepare a contribution, the pull request must identify the model or models used, including the version when known.

For example:

    AI assistance:
    - <model and version>
    - <model and version>

The contributor remains responsible for understanding, reviewing, testing, and describing the submitted changes.

AI-assisted material is subject to the same testing, licensing, provenance, compatibility, and review requirements as any other contribution.

AI tools and models must not be listed as authors or co-authors, including through `Co-authored-by` commit trailers.

`Co-authored-by` may continue to be used for human contributors who materially participated in the contribution.

## Review Feedback

Substantive review comments should be addressed before a pull request is merged.

This may mean updating the contribution, providing an explanation, or reaching agreement that no change is required.

## Governance

Pull request acceptance and decisions requiring broader project approval are governed by VitaSDK Governance.
