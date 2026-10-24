# PQC in a Pocket

A compact, plain-language introduction to post-quantum cryptography (PQC): what it is, what the first NIST standards do, and how key establishment differs from digital signatures.

This is an educational overview, not an implementation guide or a claim that any system is secure. It links to NIST's standards for exact requirements. The NIST overview currently identifies three finalized standards: ML-KEM (FIPS 203), ML-DSA (FIPS 204), and SLH-DSA (FIPS 205).

## Read in a few minutes

- [What PQC changes](guides/what-pqc-changes.md)
- [Three standards at a glance](guides/three-standards.md)
- [How a KEM fits into hybrid encryption](guides/kem-and-hybrid-encryption.md)
- [Sources](sources.md)

## The pocket summary

| Standard | Main job | Quick reminder |
| --- | --- | --- |
| **ML-KEM (FIPS 203)** | Establish a shared secret using a key encapsulation mechanism | It is a key-establishment building block, not a bulk-data cipher |
| **ML-DSA (FIPS 204)** | Create and verify digital signatures | Signatures help detect changes and verify a signer |
| **SLH-DSA (FIPS 205)** | Create and verify digital signatures | A separate hash-based signature standard |

The names and roles above follow the current [NIST PQC standards overview](https://csrc.nist.gov/projects/post-quantum-cryptography).

## What makes this guide different

It is intentionally small: one key-establishment standard, two signature standards, and one diagram showing how a KEM can feed a symmetric encryption scheme. It does not try to list every candidate algorithm or teach implementation details.
