# ARTEMIS Geometric Alignment Service API

OpenAPI 3.0 specification for the Geometric Alignment service of the
[ARTEMIS](https://www.artemis-twin.eu/) project, developed within **WP9**.

📖 **[Browse the interactive documentation →](https://artemis-twin.github.io/artemis-simulation-geometric-alignment-api/)**

## What this is

A REST API providing a mechanism to invoke algorithms for the automatic alignment of 3D models remotely, without requiring to run the alignment itself on the client platform. Alignment is a core operation on many digitization and virtual restoration tasks, particularly when the 3D data involved is very detailed and too large to handle locally on a client device.

This repository publishes the **19 endpoints** of the Geometric Alignment service categories:

| Category | Endpoints | Purpose |
|---|---:|---|
| **Session & Lock Management** | 6 | Initialize, validate, and end alignment sessions, as well as handle exclusive project locks. |
| **Parameter & Part Management** | 5 | Add/remove 3D models, check model readiness, update global transforms, and configure algorithmic parameters. |
| **Groups & Anchors** | 4 | Combine multiple parts into unified groups and establish anchor point pairs to enforce alignment constraints. |
| **Simulations & Status Checking** | 4 | Trigger local/global registration between parts or bundle adjustments for groups, and retrieve the cached operation status. |

## Files

| File | Contents |
|---|---|
| `openapi.yaml` | The OpenAPI 3.0 specification |
| `index.html` | Swagger UI page, served by GitHub Pages |
