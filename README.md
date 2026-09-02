# enterprise-semantics-spec

> Normative semantic and conformance specifications: identifier scheme, relationship vocabulary, lifecycle model, serialization formats.

This repository holds the **implementation-neutral** specifications that the [enterprise-semantics](https://github.com/Enterprise-Semantics/enterprise-semantics) source must satisfy, and the conformance requirements that [enterprise-semantics-test-probe](https://github.com/Enterprise-Semantics/enterprise-semantics-test-probe) enforces.

Specifications live in `docs/spec/` as Markdown documents with normative requirements. Each requirement carries a stable ID (for example `ES-SPEC-IDENT-001`) and is referenced by the test-probe.

## Status

**Skeleton (v0.0.1).** The founding specifications (identifier scheme, lifecycle model, relationship vocabulary) land after ADR-ES-001 in Phase 3 per the [program plan](https://github.com/Enterprise-Semantics/enterprise-semantics-governance/blob/main/docs/plan/PLAN.md).

## What this repository is for

- Identifier scheme (`ES:<KIND>:<NAME>` and variants).
- Relationship vocabulary (predicates, inverses, qualifications).
- Lifecycle model (Candidate ;;; Investigating ;;; Proposed ;;; Established ;;; Canonical ;;; Mapped ;;; Deprecated ;;; Retired).
- Provenance schema.
- Mapping schema (delegated to [enterprise-semantics-mappings](https://github.com/Enterprise-Semantics/enterprise-semantics-mappings)).
- Serialization formats (YAML, JSON, JSON Schema).
- Conformance levels.

## Relationship to other repositories

| Repository | Relationship |
|------------|--------------|
| [`enterprise-semantics`](https://github.com/Enterprise-Semantics/enterprise-semantics) | Downstream: this repository specifies what that source must satisfy. |
| [`enterprise-semantics-test-probe`](https://github.com/Enterprise-Semantics/enterprise-semantics-test-probe) | Downstream: this repository defines the conformance checks that the test-probe implements. |
| [`enterprise-semantics-governance`](https://github.com/Enterprise-Semantics/enterprise-semantics-governance) | Side: ADRs and CRs that ratify or modify specifications. |

## Contributing

See [CONTRIBUTING.md](https://github.com/Enterprise-Semantics/.github/blob/main/CONTRIBUTING.md). Spec changes require an ADR.

## License

Apache License 2.0. See [LICENSE](https://github.com/Enterprise-Semantics/enterprise-semantics-spec/blob/main/LICENSE).