---
title: "Passive SSH Key Compromise via Lattices"
authors: 'Keegan Ryan, <u>Kaiwen He</u>, George Arnold Sullivan, and Nadia Heninger.'
collection: publications
category: conferences
permalink: /publication/2023-ssh-lattice-attack
excerpt: 'We demonstrate that a **passive** network attacker can opportunistically obtain **private RSA host keys** from an SSH server that experiences a **naturally arising fault** during signature computation. In prior work, *this was not believed to be possible* for the SSH protocol because the signature included information like the shared Diffie-Hellman secret that would not be available to a passive network observer. We show that for the signature parameters commonly in use for SSH, there is an **efficient lattice attack** to recover the private key in case of a signature fault. We provide a security analysis of the SSH, IKEv1, and IKEv2 protocols in this scenario, and use our attack to discover **hundreds of compromised keys in the wild** from *several independently vulnerable* implementations.'
date: 2023-11-26
venue: 'ACM CCS'
paperurl: 'https://eprint.iacr.org/2023/1711.pdf'
slidesurl: '/files/slides/ssh-lattice-attack.pdf'
---

We demonstrate that a passive network attacker can opportunistically obtain private RSA host keys from an SSH server that experiences a naturally arising fault during signature computation. In prior work, this was not believed to be possible for the SSH protocol because the signature included information like the shared Diffie-Hellman secret that would not be available to a passive network observer. We show that for the signature parameters commonly in use for SSH, there is an efficient lattice attack to recover the private key in case of a signature fault. We provide a security analysis of the SSH, IKEv1, and IKEv2 protocols in this scenario, and use our attack to discover hundreds of compromised keys in the wild from several independently vulnerable implementations.

Joint work with: Keegan Ryan, George Arnold Sullivan, and Nadia Heninger.
