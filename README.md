# ZKM-Proof-Verification - SHA256 Hash Verification
a project overview for a Zero-Knowledge Proof (ZKP) playground using ZKM (Zero-Knowledge Machine) for SHA256 hash verification. This project demonstrates the lifecycle of a ZKP generation process, showcasing a simple program that verifies a SHA256 hash without revealing the original input.

To summarize, the project consists of the following components:

A Rust program that performs SHA256 hash verification
A proof generation process using ZKM
A verifier contract (to be generated)
The proof generation process involves six main steps:

Writing the program (already provided in Rust)
Compiling the program using MIPS
Running the program through a prover with inputs
Receiving the proof as output
Generating a verifier contract from the ImageID of the program
Posting the proof to the verifier contract
The Rust program at the core of this project accepts two inputs: a public SHA256 hash and a private input value. It computes the SHA256 hash of the private input, verifies that the computed hash matches the public input, and commits the result to the proof.

You've also provided an example test case using the word "BUILDH3R" with a corresponding SHA256 hash.

To use this project, one needs to review the Rust code in HelloWorld.rs, input values through the provided interface, and click "Generate Proof" to run the proof generation process.