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

# Cardinality (count) of Functions

How many functions of type n map to a function of type m. Each row corresponds to a possible input

<img src="/res/discreteex.png">

## Count of One-to-One Functions

One-to-one functions are permutations. Can be seen as a table with 2^n entries where each row is unique.


## Vernam Cipher (One Time Pad - OTP)

An OTP is perfectly secure as long as the key is never reused.

*Disadvantages:*

- Setting up a shared key is the most difficult part of secret communication. Ideally it can be reused once set.

- OTP does not guarantee the integrity of received data. Bits can be flipped.

## Semantic Security

Perfect secrecy is overkill. As long as the key size is large enough it is computationally infeasible to try to brute force it.

Thus, in practice cryptographic functions settle for semantic security.

**A cipher is semantically secure if there is no algorithm that has lower complexity than brute forcing the key.**

#
