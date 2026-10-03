# Changelog

## 0.1.0-draft.2 — 2026-10-03

Documentation cleanup after the first public draft: removed obsolete references to
the former parent repository from onboarding text and uses `famfamfam` as the sole
public contributor identity. Protocol messages and schemas are unchanged.

## 0.1.0-draft.1 — 2026-10-03

Initial experimental specification package. Defines role-specific contracts for
catalog publication, independent indexing, agent-assisted transactions, evidence,
reputation, communities and infrastructure accounting. The registry and service
token are mandatory network concepts; a concrete blockchain binding is not selected.

Includes JSON schemas, reproducible examples, cryptographic fixtures and document
checks. Does not include running network services or a production checkout binding.

Pre-publication review adds explicit currency exponents, network and destination
bindings, cumulative permission limits, snapshot tombstones and rollback checks,
issuance-time checks, and bounded delta validation with regression fixtures.
