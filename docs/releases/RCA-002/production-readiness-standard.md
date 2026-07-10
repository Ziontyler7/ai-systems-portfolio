# RCA-002 Production-Readiness Standard

**Release:** RCA-002 — Production Normalization and Release Hardening  
**Status:** Proposed control standard  
**Applies to:** All active Operation Runway repositories

## Governing principle

A repository is production-ready only when its declared purpose, implementation or evidence, security posture, operational controls, and public representation are consistent and independently verifiable.

Existence is not completion. A successful commit is not a release. A passing build is not proof that public claims are accurate.

## Gate 1 — Identity and ownership

Required:

- Repository owner and maintainers are known.
- The repository has a single declared purpose.
- Visibility is intentional.
- Canonical, supporting, legacy, experimental, or record status is declared.
- Overlap with other repositories is resolved.

Failure condition: Ambiguous purpose, duplicate canonical claims, or unclear ownership.

## Gate 2 — Branch and change control

Required:

- The default branch is intentional and documented.
- Production branches are protected from uncontrolled direct changes where platform capabilities allow.
- Material work is traceable to issues and pull requests.
- Merge strategy is declared.
- Stale or abandoned branches are reviewed.

Failure condition: A temporary hardening or migration branch functions as the default without an explicit operational decision.

## Gate 3 — Documentation fidelity

Required as applicable:

- `README.md`
- `ARCHITECTURE.md` or equivalent architecture documentation
- `CHANGELOG.md` or release history
- `SECURITY.md`
- contribution and review guidance
- deployment, rollback, and recovery notes for deployable systems
- public-boundary documentation for evidence repositories

Documentation must describe current reality and distinguish implemented, experimental, planned, deprecated, and removed capabilities.

Failure condition: Documentation overstates implementation or contradicts the repository.

## Gate 4 — Build, test, and artifact integrity

Required for software repositories:

- Reproducible dependency installation.
- Successful build or startup validation.
- Automated tests appropriate to the risk profile.
- Linting or static checks where appropriate.
- Versioned deployable artifacts or reproducible build instructions.
- Test evidence tied to a commit SHA.

Required for evidence or record repositories:

- Link validation.
- Source and citation validation.
- File-integrity and chronology review where provenance matters.

Failure condition: Results cannot be reproduced or tied to a specific revision.

## Gate 5 — Security, privacy, and licensing

Required:

- No committed secrets or credentials.
- Sensitive personal, operational, and proprietary material remains within approved boundaries.
- Dependencies and included assets have an understood licensing posture.
- Security reporting guidance exists where appropriate.
- Public repositories have completed exposure review.

Failure condition: Exposed credentials, private records, unclear asset rights, or an unresolved critical vulnerability.

## Gate 6 — Runtime and deployment readiness

Required for deployable systems:

- Declared environment and deployment target.
- Configuration and secret-management procedure.
- Health checks and observability appropriate to the system.
- Failure, degradation, and recovery behavior documented.
- Rollback path tested or credibly demonstrated.
- Production endpoint or artifact evidence captured without exposing protected information.

Failure condition: The application can only be demonstrated through an undocumented local or manual state.

## Gate 7 — Evidence Command Center alignment

Every material professional claim must map to:

- repository and revision;
- relevant implementation or document path;
- issue or pull request where appropriate;
- test, artifact, screenshot, or deployment evidence;
- resume, LinkedIn, and portfolio wording;
- verification status and reviewer.

Failure condition: Public language exceeds or cannot be traced to available evidence.

## Gate 8 — Recruiter and reviewer readability

Required for public-facing repositories:

- Purpose is understandable within the opening section.
- Navigation is clear.
- Technical depth is accessible without exposing private implementation.
- Claims use specific, defensible language.
- Links work and contact information is current.
- The repository has no abandoned scaffolding presented as a completed product.

Failure condition: A serious reviewer cannot determine what was built, what role Michael played, or what evidence supports the claim.

## Gate 9 — Independent fidelity verification

A reviewer other than the primary producer must examine:

- evidence sufficiency;
- contradictions and unsupported claims;
- security and public-boundary risks;
- branch and release integrity;
- documentation accuracy;
- recruiter readability;
- residual risks.

Failure condition: The same producer is the sole authority declaring the work complete.

## Gate 10 — Release decision

Every repository receives one explicit decision:

- **Approved**
- **Approved with Conditions**
- **Revision Required**
- **Blocked**
- **Archive**

The decision must include:

- reviewed revision;
- passed and failed gates;
- known residual risks;
- required corrective actions;
- approving reviewer and date.

## Minimum pull-request evidence

Every production-normalization pull request should include:

1. Problem and scope.
2. Files and systems affected.
3. Acceptance criteria.
4. Verification performed.
5. Security and public-boundary impact.
6. Evidence links or paths.
7. Known limitations and rollback plan.
8. Release recommendation.

## RCA-002 exit criteria

RCA-002 is complete only when:

- the full repository registry is verified;
- every repository has a lifecycle and canonicality decision;
- corrective issues are created and prioritized;
- critical public and private boundary risks are resolved;
- public evidence claims are mapped;
- production candidates pass their applicable gates;
- legacy repositories are clearly archived or justified;
- an independent fidelity review is recorded;
- the final RCA-002 release report is merged.