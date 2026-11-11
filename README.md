# Candidate approvals

This public repository contains only the generic approval workflow, opaque candidate digests and dates. Never upload application code, deployment scripts, business documents, server addresses or credentials.

A request branch is named `requests/<SHA-256>`. Its workflow waits for the configured reviewer. Only the human reviewer may approve or reject it. Agents must never approve on the reviewer's behalf.

An approved workflow is evidence for that exact frozen candidate, not a deployment itself. The production verifier independently reads GitHub review history, checks the repository and environment IDs, approver, workflow content, candidate digest, first attempt, successful completion and expiry. A completed run without a matching approval must be denied. Existing preflight, health, storage admission, backups and recovery requirements still apply.

Production access is not granted by this repository. No production keys or tokens belong here. On 2026-11-11 UTC, a synthetic approval, execution and recovery cycle was verified; detailed evidence remains private. This does not authorize any application release or grant unrestricted administrative access.
