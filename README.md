# hackpert-forge

Prolog code-security expert system: ZeroForge ported onto
[prolog-rlm](https://github.com/lost-rob0t/prolog-rlm), with a vulnerability
knowledge base and CVE List v5 ([cvelistV5](https://github.com/CVEProject/cvelistV5))
ingestion.

## Purpose

- Reimplement the ZeroForge evidence -> generate -> validate -> repair
  exploit-engineering pipeline as a Prolog expert system embedding prolog-rlm.
  The model proposes strategy; Prolog owns execution semantics, validation,
  and promotion.
- Maintain a vulnerability KB as queryable Prolog facts with provenance,
  ingesting the CVEProject/cvelistV5 corpus (CVE JSON 5.x) and bounded
  advisory sources (OSV, GHSA, CISA KEV).
- Generate security artifacts (Metasploit modules, ZAP scan rules, Nuclei
  templates) only through hard deterministic validators and bounded repair.

## Ownership and lineage

- Source of truth: https://github.com/lost-rob0t/hackpert-forge
- Port lineage: https://github.com/lost-rob0t/zero-forge (Python original)
- Embedded runtime: https://github.com/lost-rob0t/prolog-rlm

Status: bootstrap. Scope and port-mapping milestones live in the issue
tracker; no implementation is implied by this repository existing yet.
