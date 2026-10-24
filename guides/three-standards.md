# Three NIST standards at a glance

NIST published these three post-quantum cryptography standards on August 13, 2024. Check the linked standard pages for current errata and updates.

| Name | Standard | Use |
| --- | --- | --- |
| **ML-KEM** | [FIPS 203](https://csrc.nist.gov/pubs/fips/203/final) | A key-encapsulation mechanism used to establish a shared secret |
| **ML-DSA** | [FIPS 204](https://csrc.nist.gov/pubs/fips/204/final) | A digital signature scheme: generate signatures and verify them |
| **SLH-DSA** | [FIPS 205](https://csrc.nist.gov/pubs/fips/205/final) | A stateless hash-based digital signature scheme |

## Easy mix-ups

- **ML-KEM is not a signature scheme.** It is for key establishment.
- **ML-DSA and SLH-DSA are signatures.** They do not encrypt a message for confidentiality.
- **A KEM is not a complete messaging protocol.** An application still needs to use the established key material correctly and handle authentication and other protocol needs.
- **A standard name does not guarantee an implementation is correct.** Use maintained, reviewed software and follow its documentation.
