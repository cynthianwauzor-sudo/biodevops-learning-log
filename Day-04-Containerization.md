# Day 4: Containerization & Reproducibility
**Date:** January 16, 2026
**Focus:** Docker, Dockerfiles, and Volume Mounting

## 📝 Summary
Solved the "It works on my machine" problem by containerizing the `setup_lab.sh` script. Built a custom Docker image using Alpine Linux, debugged a cross-platform "Shebang" error (`exec format error`), and implemented Volume Mounting to ensure data generated inside the container persists on the host machine.

## 🛠 Technical Skills Acquired
* **Docker Architecture:** Understanding Images (Recipes) vs. Containers (Meals).
* **Dockerfile Syntax:** `FROM`, `WORKDIR`, `COPY`, `RUN`, `ENTRYPOINT`.
* **Build & Run:** `docker build -t lab-bot .` and `docker run`.
* **Debugging:** Identifying and fixing missing interpreter headers (`#!/bin/sh`).
* **Persistence:** Using volumes (`-v $(pwd):/app`) to drill a "hole" in the container for data retrieval.

## 💡 Key Takeaway
> "If the data stays in the container, it dies in the container. Volume mounting is essential for extracting results from a containerized pipeline."
