# Security maintenance — 2026-10-15

External links explicitly isolate the opened tab; the page sends no referrer.

## Validation

Static HTML reviewed; no build pipeline.

No package-manager dependency tree in this repository.

## Limits and deployment

This is a source/dependency maintenance review, not a security certification or a penetration test. npm audit counts vulnerable packages, not distinct exploitable defects. Legacy build tooling still has known advisories and requires a future migration; a successful build does not resolve those advisories. Audit suggestions to replace react-scripts with a nonfunctional package must not be applied automatically.

Local builds used Node 24.19.0 and npm 11.21.0 with installation lifecycle scripts disabled. Existing lint warnings are not treated as a successful lint audit. Browser permissions, live hosting configuration, account MFA, branch protections, cloud IAM, and full Git history were not comprehensively verified.

