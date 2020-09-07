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

## Cardinality (count) of Functions

How many functions of type n map to a function of type m. Each row corresponds to a possible input

<img src="/res/discreteex.png">

## One-to-One Functions

One-to-one functions are permutations. Can be seen as a table with 2^n entries where each row is unique.

## Pseudo Random Functions

Cryptographic functions usually have hundreds or thousands of bits.

- SHA-2 maps 512bit strings to 256bit strings.

- AES is a one-to-one function that maps 128bit strings to 128bit strings.

These functions are enormous so we need a key that conveys the chosen function.

## PRFs, PRPs, PRGs

Keyed functions used in cryptography are pseudo-random functions, pseudo-random permutations, and pseudo-random generators.

- PRF: *F:{0,1}^l✕{0,1}^m →{0,1}^n* Bits are mapped from m-bit input to n-bit output. Mapping is determined by the i-bit key. PRFs with n < m are used as compression functions.

- PRP: *E:{0,1}l✕{0,1}n →{0,1}n* A specific permutation of the 2^n possible n-bit values. PRPs are used as block ciphers

- PRG: A PRF can be used to construct a PRG. If F(k,x)  is a secure PRF, then  G(k)=F(k,0)||F(k,1)||F(k,2)... is a secure PRG.

## Symmetric vs Asymmetric Cryptography

### Symmetric

- PRGs are used for realizing stream ciphers
- PRPs are used for realizing block ciphers
- PRFs are used for realizing hash functions

### Asymmetric

In asymmetric cryptography it is easier to think of functions as operations performed in a finite group.

- It is asymmetric because of the use of key-pairs instead of a shared key
- A key-pair includes a private secret key and a public key

## Finite Groups in Asymmetric Cryptography

*A finite group is a set with a group operation that maps two elements to a third element of the same set*
