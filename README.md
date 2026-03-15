# language-dictionary

A Java client–server dictionary and vocabulary learning application.

This repository combines the original **language-dictionary-client** and **language-dictionary-server** projects into a single codebase. Together they form a simple end‑to‑end system for storing vocabulary data, serving dictionary queries, and providing a user-facing client interface.

---

## Overview

The project demonstrates a classic **client–server architecture**:

1. The **server** stores vocabulary data and provides dictionary lookup functionality.
2. The **client** provides a user interface for searching and interacting with the vocabulary database.
3. Communication between the two components allows users to retrieve dictionary entries and manage vocabulary data.

This repository is useful as a learning example of building a small distributed Java application with a dedicated backend and frontend.

---

## Repository Structure

```
packages/
│
├─ language-dictionary-server/
│  ├─ src/              # Server source code
│  ├─ users.dat         # User data storage
│  └─ vocab.txt         # Vocabulary dataset
│
└─ language-dictionary-client/
   ├─ src/              # Client source code
   └─ assets/           # UI images and resources
```

---

## Server (packages/language-dictionary-server)

The server provides the backend logic and data layer for the application.

Responsibilities include:

- storing vocabulary entries
- managing user data
- serving dictionary lookup requests
- handling communication with the client application

Data files included:

- **`vocab.txt`** – vocabulary dataset
- **`users.dat`** – simple user storage

---

## Client (packages/language-dictionary-client)

The client provides the user-facing interface for interacting with the dictionary.

Capabilities include:

- searching for vocabulary entries
- displaying results returned by the server
- interacting with the dictionary dataset

The client is implemented as a Java desktop application.

---

## Technologies

- Java
- File-based data storage
- Client–server architecture

---

## Why this project is interesting

This project demonstrates several core software engineering concepts:

- separation of frontend and backend responsibilities
- communication between distributed components
- simple data persistence using flat files
- building user-facing tools on top of backend services

Although simple, it represents a complete small-scale application stack.

---

## Possible Improvements

Potential extensions could include:

- replacing flat-file storage with a relational database
- exposing the server as a REST API
- adding authentication and user management
- modernizing the client with a web or mobile interface
- adding automated tests and build tooling
