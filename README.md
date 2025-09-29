# Kikkoman Project v1.0

**Kikkoman** is a standalone, horizontally scalable server/service for managing requests in the Kikkoman AI project. It is designed as a back-end AI service and is not intended for direct web client-server interactions.

---

## Table of Contents

- [Docker Image](#docker-image)
- [API Documentation](#api-documentation)
- [Docker Run](#docker-run)
- [Todo](#todo)
- [Update History](#update-history)

---

## Docker Image

The Docker image for Kikkoman project is downloaded from "Github releases"
using this URL:

https://github.com/ahard-elife/project_kikkoman/releases

### Loading

gunzip -c kikkoman-latest.tar.gz | docker load

---

## API Documentation

API specifications and usage guides are in the `/docs` directory.
 

## Docker Run

Download the Docker image from  or the /image directory.
(can put it in GitHub Releases later on or via AWS ECR)

**Load**:

gunzip -c kikkoman-latest.tar.gz | docker load

**Run the container**:

docker run -d -p 5000:5000 --name kikkoman-server kikkoman:latest

(Adjust tag and port mapping as needed)

---

## Todo

- Pre-built archive via GitHub Releases or that I push directly to AWS ECR
- Data provisioning is currently bulk-load/batch


## Update History
| Version | Date       | Notes                        |
|---------|------------|------------------------------|
| v1.0.0  | 2025-09-18 | Self-containing JSON-service |

---

Arthur (arthur.hard@elife.co.jp)

Questions? Mail me or open an issue.


