# Paxos Algorithm C++ Benchmark | 1.0.0 Simple 

## Description

This project will simulate the three core object relationships in the Paxos algorithm: Proposers, Acceptors, and Learners.

This project will reveal exactly *why* these components talk to one other.

Note: Proposers, Acceptors, and Learners are typically communicating over a distributed communication network. This version of the project will simulate this communication through
simple function calls.

For ease and scalability, main initializations will be handled by parsing a JSON config file, structured as follows for each of Learners, Acceptors, and Proposers, NOTE: this is a minimal version, further iterations will find the optimal number of communications for simulating interactions in production codebases.

```JSON
{
  "proposers": [
    {"id": 1, "name": "Proposer1"},
    {"id": 2, "name": "Proposer2"}
  ],
  "acceptors": [
    {"id": 1, "name": "Acceptor1"},
    {"id": 2, "name": "Acceptor2"}
  ],
  "learners": [
    {"id": 1, "name": "Learner1"},
    {"id": 2, "name": "Learner2"}
  ]
}


```

## Structure

This project is part of a larger series to benchmark implementations of the Paxos algorithm in vanilla C++ and Java. 


 **Directory tree**
```text
project-root/
├── src/
│   ├── main.cpp
│   ├── proposer.cpp
│   ├── acceptor.cpp
│   └── learner.cpp
├── include/
│   ├── proposer.h
│   ├── acceptor.h
│   └── learner.h
├── tests/
│   └── test_main.cpp
├── configs/
│   └── paxos_config.json
├── lib/
├── build/
├── .gitignore
└── README.md
```

## Usage

To be written by 09/24/23


## Implementation Overview

To be written by 09/29/23


## Benchmarking tests

Comparing the space, time and overall performance complexity between programming languages is not an easy process. However, because meeting complex problem domains with equally complex solutions just creates, most of the time, endless abstractions, the benchmark tests employed in this project will be farily simple. 

There is a key distinction being made here- between an "easy" solution and a "simple" one. 

Sure, it may be "easier" to use pre-written dependencies to minmize time to production, but the boilerplate required for setting up substantial projects using abstract frameworks or libraries in C++ and Java become a barrier to answering the fundamental question here:

### When is C++ or Java the *preferrable* solution in implementing the Paxos algorithm?




*This README is a work in progress*