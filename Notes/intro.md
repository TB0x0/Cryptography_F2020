# Introduction

## What is Cryptography

Literal meaning is secret writing. Involves *encryption* of plain text and then *decryption* of cipher text using cryptographic algorithms (also called cryptographic primitives). These are well defined functions with inputs and outputs. Functions can be cascaded to construct cryptographic protocols.

## The Need for Information Security

Everything of value is information:

- Money
- Property
- Voting
- Bills

## What is Security

1. Being free from danger
2. Ensuring all desired assurances are met (things happen the way we expect them to)

Cryptographic tools and protocols provide specific types of assurances regarding digital data.
 - They do not care what the bits represent.


## Claims of Security

- Extraordinary claims require extraordinary evidence
- The claims made by cryptographic primitives must be backed up by evidence. This is difficult because **proving a negative** is generally very hard (such-and-such encryption is unbreakable)

- We have very good evidence that some things are actually impractical. Such as factoring a large number, solving large degree highly nonlinear equation, reversing "one-way" problems

## What to expect in the course

- Probability, random events, random variables
- Discrete Math (groups, fields, discrete functions)
- Number theory (primes, gcd, divisibility, factorization)
- Cryptographic algorithms (and the math required to understand them)

## Symmetric and Asymmetric Algorithms

<ol>
  <li>Symmetric Cryptography Algorithms</li>
    <ul>
      <li>Encryption/Decryption</li>
      <li>Hash functions</li>
      <li>Message authentication codes</li>
      <li>PRF/PRP (Pseudo random function/permutation)</li>
    </ul>
  <li>Asymmetric Cryptography Algorithms</li>
    <ul>
      <li>Encryption/Decryption</li>
      <li>Digital Signatures</li>
      <li>Key-pair generation</li>
    </ul>
</ol>
