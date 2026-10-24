# What post-quantum cryptography changes

Post-quantum cryptography (PQC) is cryptography designed to run on ordinary computers and resist attacks from both classical and quantum computers. It does not require a quantum computer to use.

A sufficiently capable quantum computer could threaten some widely used public-key systems. PQC gives software and protocols new public-key tools intended to withstand those attacks. The practical work is identifying where vulnerable algorithms are used and migrating systems carefully; replacing one algorithm name in code is not the whole job.

## A useful distinction

PQC standards include different kinds of tools:

- **Key establishment:** helps parties establish shared secret key material. NIST's ML-KEM standard is in this category.
- **Digital signatures:** let a signer create a signature that others can verify. ML-DSA and SLH-DSA are in this category.

These tools do different jobs. A key-encapsulation mechanism is not itself the symmetric algorithm that encrypts a large file, and a digital signature does not hide the signed message.

## Keep the claim modest

“Post-quantum” describes the intended security against known quantum-computing attacks; it does not mean unbreakable. Implementations, protocols, key handling, and future cryptanalysis still matter. For real deployments, follow current standards, vendor guidance, and expert migration advice rather than selecting algorithms from this introductory page.
