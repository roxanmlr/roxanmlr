# Loïc MILANDOU
**Industrial Systems Engineer · Student at 42 Paris · Transitioning into software**

I'm building a spreadsheet engine from scratch as a personal capstone project

---
## Spreadsheet Engine
### Why this project?
This project interests me particularly because of its ubiquity in professional environments and its engineering complexity.
My goal is to build a high-performance spreadsheet (low memory footprint, fast response times) with native support for concurrent use.
Building it from scratch will let me get familiar with compiler theory, graph algorithms, distributed systems, and cybersecurity within a single, coherent, hands-on project.
### Key deliverables
**Expression language and interpreter**

This is the main channel of communication between the user and the software. In particular, it must be data-oriented and provide clear error messages.

**Dependency graph and cycle detection**

The engine must be able to _present_ the dependency graph to the user and detect circular references.

**Distributed Systems and Cybersecurity**

The engine will be distributed as a server and able to support concurrent access from multiple users while enforcing access and modification rights.

## Tech stack
The engine will be developed in C / C++.
