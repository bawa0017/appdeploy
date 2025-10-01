# Kubernetes Deployment Project

This repository contains Kubernetes manifests for deploying a simple microservices application, including a frontend, backend, and MongoDB database, along with persistent storage and secrets management.

---

## Repository Structure

| File | Description |
|------|-------------|
| `frontend.yml` | Deployment manifest for the frontend application. |
| `frontend-service.yml` | Service manifest exposing the frontend. |
| `backend.yml` | Deployment manifest for the backend application. |
| `backend-service.yml` | Service manifest exposing the backend. |
| `mongodb.yml` | Deployment manifest for MongoDB database. |
| `mongodb-service.yml` | Service manifest exposing MongoDB. |
| `pvc.yml` | PersistentVolumeClaim manifest for storing MongoDB data. |
| `pv.yml` | PersistentVolume manifest (if using static provisioning). |
| `secret.yml` | Kubernetes Secret manifest for storing sensitive information like database credentials. |

---

## Prerequisites

- Kubernetes cluster (Minikube, Kind, EKS, GKE, etc.)
- `kubectl` configured to access your cluster
- Docker images for frontend and backend already built and pushed to a container registry
