# RCA-002 Repository Registry

**Release:** RCA-002 — Production Normalization and Release Hardening  
**Status:** Initial inventory; verification in progress  
**Authority:** Operation Runway Evidence Command Center

## Purpose

This registry records the known GitHub estate, each repository's intended role, visibility, lifecycle state, canonicality, and current production recommendation. It prevents duplicate repositories, legacy code, public evidence, and private implementation from being treated as interchangeable.

## Registry

| Repository | Visibility | Intended role | Initial lifecycle classification | Canonical status | Initial release recommendation |
|---|---|---|---|---|---|
| `Ziontyler7/ai-systems-portfolio` | Public | Professional evidence hub for recruiters, hiring managers, collaborators, and technical reviewers | Active | Canonical public evidence repository | Revision Required |
| `Ziontyler7/gmais-framework` | Public | Public authorship and citation anchor for governed multi-agent intelligence concepts | Active | Canonical public framework record, pending content verification | Revision Required |
| `Ziontyler7/Ziontyler7` | Public | GitHub profile repository and professional entry point | Active | Canonical profile surface | Revision Required |
| `Ziontyler7/Edios` | Private | Private Edios repository; exact operational role not yet verified | Undetermined | Not yet assigned | Blocked pending inspection |
| `Ziontyler7/edios-core-clean` | Private | Large private implementation repository and probable current core | Active candidate | Canonical implementation candidate | Blocked pending build, security, branch, and architecture verification |
| `Ziontyler7/edios-rig-library` | Private | Supporting rig or library assets | Active candidate | Supporting repository candidate | Blocked pending dependency and licensing review |
| `Ziontyler7/EdiosV1` | Private | Earlier Edios implementation | Legacy candidate | Non-canonical unless evidence proves otherwise | Archive candidate pending comparison |
| `Ziontyler7/Initial-authorship-and-IP-record-for-Edios-documents` | Private | Authorship and intellectual-property provenance record | Record repository | Canonical provenance candidate | Approved with Conditions pending integrity review |

## Immediate risks

1. `edios-core-clean` uses `clean-post-cutover-hardening-2026-05-11` as its default branch rather than a stable conventional production branch. This may be intentional, but it must be verified and documented before release.
2. `Edios`, `EdiosV1`, and `edios-core-clean` have overlapping names and potentially overlapping scope. Their canonical relationships must be proven, not inferred.
3. The public evidence repositories currently demonstrate narrative and architectural documentation, but production readiness requires claim-to-evidence mappings and independent verification.
4. Repository visibility boundaries must be checked before any private implementation evidence is surfaced publicly.
5. No repository receives an Approved production recommendation solely because it exists or has recent commits.

## Canonicality rules

- Exactly one repository may be designated canonical for any deployable application or authoritative evidence function.
- Legacy repositories must identify their successor and must not appear active without an explicit reason.
- Public repositories may contain professional evidence, sanitized architecture, and authorship records, but not secrets, private prompts, personal records, or unpublished implementation details.
- Private repositories may support public claims only through reviewed evidence references that do not expose protected material.
- A branch name, repository name, or recent commit is not evidence of production status.

## Required verification pass

For each repository, RCA-002 must verify:

- ownership and permission level;
- repository description and declared purpose;
- default branch and active branches;
- current README accuracy;
- architecture and dependency documentation;
- recent commits, open issues, and pull requests;
- CI/CD and test evidence;
- secret, privacy, and licensing posture;
- deployment or artifact evidence where applicable;
- relationship to resume, LinkedIn, portfolio, and other public claims;
- final lifecycle and release recommendation.

## Recommendation vocabulary

- **Approved:** All applicable production gates passed.
- **Approved with Conditions:** Safe for the declared purpose with explicit residual conditions.
- **Revision Required:** Viable, but material corrections are required before production release.
- **Blocked:** Verification cannot proceed or critical risks remain unresolved.
- **Archive:** Repository should be preserved as history but removed from active operational positioning.

## Change control

Changes to repository roles, canonicality, public/private boundaries, or release recommendations must be made through a traceable issue and pull request under RCA-002 or a successor release.