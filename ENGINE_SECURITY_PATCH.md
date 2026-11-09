# Engine compatibility branch

Base: alloy-rs/core v1.7.3 (`87080853083c909b34f8c8cff3622570c114985d`).

Use upstream k256 0.14 and rename the SEC1 point trait, following the relevant
change in alloy-rs/core PR #1147. This selects fixed upstream crypto-bigint;
no cryptographic arithmetic or transaction encoding is changed here.
Engine pins this branch by commit and tests published EIP-155 wires, hash
boundaries, signer recovery, retained-wire replay and cross-binary recovery.
Replace the fork when maintained compatible upstream releases contain the fix.
