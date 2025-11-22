[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/vhoKWTLf)
# assignment-2

Generate legacy addresses, bech32 addresses and bech32m addresses
 Answer: Find the output.txt file. They're all in there

What is the difference between hardened and non hardened keys
Answer: 

Non-hardened keys

Child keys can be derived from parent public key + chain code.

Less secure: if a child private key leaks, the parent can be compromised.

Convenient for watch-only wallets.

Hardened keys

Child keys can only be derived with parent private key + chain code.

More secure: parent cannot be derived from child keys.

Ideal for hardware wallets or extra-secure setups.


Why should a wallet developer prefer deterministic wallets over non deterministic wallets
Answer:

Deterministic wallets (HD wallets / BIP32): generate all keys from a single seed phrase.

Easier to back up (just one seed).

Can generate unlimited addresses deterministically.

Allows hierarchical structure (multiple accounts and addresses).

Non-deterministic wallets: generate random keys individually.

Harder to back up.

Losing the wallet means losing all funds.

 Conclusion: deterministic wallets are safer, easier to manage, and recoverable from a single backup.
