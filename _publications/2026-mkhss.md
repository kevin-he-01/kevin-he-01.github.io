---
title: "Concretely-Efficient Multi-Key Homomorphic Secret Sharing and Applications"
authors: '<u>Kaiwen He</u>, Sacha Servan-Schreiber, Geoffroy Couteau, and Srinivas Devadas.'
collection: publications
category: conferences
permalink: /publication/2026-mkhss
excerpt: 'We construct and implement the **first**, **concretely-efficient** *Multi-Key Homomorphic Secret Sharing (MKHSS)* scheme. A powerful application of MKHSS is to realize *attribute-based non-interactive key exchange (ANIKE)*, which **generalizes** password-authenticated key exchange (PAKE) to **arbitrary** attribute policies. ANIKE is currently only known from MKHSS and in this paper we show the **first practical instantiation of ANIKE** for two **concrete** predicate types with applications to geolocation-based key exchange and fuzzy PAKE.'
date: 2026-05-18
venue: 'IEEE S&P'
addinfo: ' (to appear)'
codeurl: 'https://github.com/kevin-he-01/mkhss'
---

Homomorphic secret sharing (HSS) is a powerful cryptographic primitive that enables efficient, low-communication secure computation without the use of fully homomorphic encryption. Public-key HSS is a well-known variant that supports inputs from multiple parties, but all parties must agree on a joint public key before any party can encode their inputs, requiring extra rounds of communication in applications. Recently, Couteau et al. (EUROCRYPT 2025) constructed multi-key HSS (MKHSS)—a new primitive which allows parties to encode their inputs under independent keys—under the DCR assumption. MKHSS assumes only a reusable common reference string, without the need for prior interactions between parties or a public-key infrastructure.

In this paper, we construct and implement the first concretely-efficient MKHSS scheme under the same assumptions used by Couteau et al.
Using an algorithmic insight that reduces the largest modulus in Couteau et al. from $$N^4$$ to $$N^2$$, our optimized implementation can homomorphically multiply inputs in 5.0 milliseconds—while an implementation of Couteau et al. requires 224.6 milliseconds—thereby achieving a $$45\times$$ speedup.

A powerful application of MKHSS is to realize attribute-based non-interactive key exchange (ANIKE), which generalizes password-authenticated key exchange (PAKE) to arbitrary attribute policies. ANIKE is currently only known from MKHSS and in this paper we show the first practical instantiation of ANIKE for two concrete predicate types with applications to geolocation-based key exchange and fuzzy PAKE.

We use our implementation to evaluate the first concretely-efficient ANIKE schemes for a range of practically useful policies. Using our implementation, two parties can perform a geolocation-based key exchange in under one second and a fuzzy PAKE on an 8-word passphrase in a few seconds for realistic parameters, on a single core, achieving a roughly $$30 \times$$ speedup over Couteau et al. for both applications.

Joint work with: Sacha Servan-Schreiber, Geoffroy Couteau, and Srinivas Devadas.

<!-- Using [MathJax](https://www.mathjax.org/) in the description is supported - $$E=mc^2$$ - however, the use must be mindful that the default delimiters are `$$...$$` and `\\[...\\]` which differs from the `$...$` that is typically expected. -->
