# History and Foundations

Cryptography offers a foundation for assuring digital data

## History of Cryptography

Cryptography was historicaly considered an ad-hoc science of creating ciphers for message encryption. They were usually in the form of text and cipher-text.

Early cipher construction depended on 2 fundamental operations

- Substitution - Replacing one character with another.
- Permutation - Switching characters around.

Modern ciphers are not different from this except they use both operations repeatedly.

These ciphers are trivial to break and with a single plaintext-ciphertext pair the whole cryptographic function is broken.

**A cipher satisfies the requirement of perfect secrecy if it can withstand attacks by an attacker with unlimited computational ability.**

## Vernam Cipher (One Time Pad - OTP)

An OTP is perfectly secure as long as the key is never reused.

*Disadvantages:*

- Setting up a shared key is the most difficult part of secret communication. Ideally it can be reused once set.

- OTP does not guarantee the integrity of received data. Bits can be flipped.

## Semantic Security

Perfect secrecy is overkill. As long as the key size is large enough it is computationally infeasible to try to brute force it.

Thus, in practice cryptographic functions settle for semantic security.

**A cipher is semantically secure if there is no algorithm that has lower complexity than brute forcing the key.**

## Discrete functions

Any function that maps a bit-string of length m to a bit string of length n can be represented with one row corresponding to each possible input.

<img src="/res/discreteex.png">
