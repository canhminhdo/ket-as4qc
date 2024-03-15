### An Algebraic Specification for Quantum Computation in Maude
---
This repository presents an <u>A</u>lgebraic <u>S</u>pecification for <u>Q</u>uantum <u>C</u>omputation called |AS4QC> which was developed in Maude.

## Dependencies
- Maude is a programming/specification language based on rewriting logic. How to download and install Maude can be found at [here](http://maude.cs.illinois.edu/w/index.php/The_Maude_System).

## How to install
- Clone the source code to your computer and go to the source code directory.

- Feed a Maude file that is the formal specification of a protocol of interest into Maude.

For example, we can type the following command in CLI in order to see how Quantum Teleportation works:

```console
maude teleport.maude
```

- For testing, we can test the algebraic speicfication with some test cases provided as follows:

```console
cd test && ./tester
```

## Repository structure
- `cpx.maude` for complex number reasoning.

- `qc.maude` for quantum computation reasoning.

- `teleport.maude` for reasoning about Quantum Teleportation.
