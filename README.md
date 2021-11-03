# Asilomar massive random access challenge
The purpose of this repository is to identify a set of *practically relevant* scenarios for the massive random access problem as defined 
in the seminal paper by Polyanskiy (2017)[^1]  and to challenge the members of our community to propose accurate information-theoretic bounds and low-complexity
bound-approaching channel-coding schemes for such scenarios.

The purpose of this repository is also to gather numerical routines (e.g., implementation of channel models) that are useful to
tackle such challenges.

The idea behind this challenge originated from a virtual discussion at [Asilomar 2021](https://www.asilomarsscconf.org), which took place during the invited session on *massive random access*, organized by Maxime Guillaud (Huawei Technologies) and Giuseppe Caire (Technical University of Berlin, Germany).

## Status of this document
This document is still in a work-in-progress status.

## A rough classification of massive random access systems
In this section, we present a rough classification of massive random access systems for the internet of things (IoT), which will turn out useful to define the scenarios in this challenge.

One way to classify massive random access systems is by considering the complexity of the IoT devices that 
a given system intends to serve.

- **Expensive IoT devices:**
Such devices are typically equipped with both a transmitter and a receiver, which enable them to acquire synchronization and 
perform power adaptation. They are also equipped with good enough power amplifiers to be able to support transmission schemes such as orthogonal frequency-division multiplexing (OFDM).
[*Provide examples*]

- **Cheap IoT devices:**
These devices are equipped only with a transmitter, they have cheap power amplifiers, which prevent the use of OFDM, and inaccurate oscillators, which result in significant phase noise. 
[*Provide examples*]


Another useful classification is in terms of the location of the receiver.

- **Satellite-based IoT receivers:**
In such systems, the receiver is mounted on a satellite, which results in good coverage over a large geographical area.
For the case of cheap IoT devices, the propagation channel can be modeled as an AWGN channel with unknown path loss and multiplicative phase noise. The challenge for such systems is to solve the link-budget problem and to compensate for phase noise.
*[Provide some examples]*

- **Ground IoT receivers:**
In such systems, one needs to account also for small-scale fading, and for multipath propagation, which, for the case of cheap IoT devices, cannot be addressed by the use of OFDM.
*[Provide some examples]*





## Proponents of the challenge (alphabetical order)
- Giuseppe Durisi (Chalmers, Sweden)
- Maxime Guillaud (Huawei Technologies)
- Gianluigi Liva (DLR, Germany)
- Krishna Narayanan (Texas A&M University)

Interested in contributing? Please let us know and we will be happy to add you to the list. 

***	

[^1]: Y. Polyanskiy, "A perspective on massive random access," in Proc. IEEE Int. Symp. Inf. Theory (ISIT), Jan. 2017.
