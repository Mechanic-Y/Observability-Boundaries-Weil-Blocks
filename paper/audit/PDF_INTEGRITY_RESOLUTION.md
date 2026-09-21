# Observability Boundaries V1.0 — PDF Integrity Resolution

**Status:** RESOLVED  
**Date:** 2026-09-21 (JST)

## Issue

The SHA-256 values originally reported from the typeset build directory did not match the PDF byte streams surfaced through the distribution path.

Original typeset-build hashes:

- JA: `ccefae16cf5ae8ec8582b34b28a672ac39812932be471966d1de4d1dcdf2d338`
- EN: `7b568e9b3a75449de8179a6471fdb78b8c5316703a2ee57f1b3b7db7023b9946`

Distributed PDF hashes:

- JA: `c259500bf9e33484d9cb6aec7cab1c2021fe53edc016a6b55b09277a4ae9bacc`
- EN: `1e64b93112e7faf3f1592092b340a8429d8ba3120baab6c6c01d8436b0a18152`

## Content-equivalence check

The two byte representations were compared before choosing the canonical files.

- JA extracted text: identical.
- EN extracted text: identical.
- JA rendered comparison: `0 / 26` changed pages.
- EN rendered comparison: `0 / 27` changed pages.
- PDF title, author, producer, CreationDate, page count, page size, and font inventory were consistent across each pair.

The mismatch is therefore a PDF byte-serialization difference, not a mathematical, textual, or visual typesetting difference.

## Canonicalization decision

The **distributed PDF byte streams** were canonical for that Publication Candidate stage because they were the actual artifacts delivered to the reader.

Canonical V1.0 Publication Candidate PDFs at that stage:

- JA SHA-256: `c259500bf9e33484d9cb6aec7cab1c2021fe53edc016a6b55b09277a4ae9bacc`
- EN SHA-256: `1e64b93112e7faf3f1592092b340a8429d8ba3120baab6c6c01d8436b0a18152`

The later accepted Design v2 PDFs were separately frozen byte-for-byte; their final release hashes are recorded in `releases/v1.0/SHA256SUMS.txt`.

## Frozen-package rule

1. Do not regenerate or replace canonical PDFs after the final MANIFEST is generated.
2. The final MANIFEST must hash the exact distributed/source files included in the Frozen package.
3. The MANIFEST does not include its own hash, avoiding self-reference.
4. Audit documents should refer to the MANIFEST for final artifact hashes rather than embedding a self-hash.

**Verdict: PDF byte integrity was resolved before final Design v2 freeze.**
