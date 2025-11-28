# Deployment Guide

## Overview

This guide covers deployment procedures for NexaFlow applications.

## Environments

- **Development:** Auto-deployed from feature branches
- **Staging:** Deployed from main branch
- **Production:** Deployed from tagged releases

## Deployment Process

### Prerequisites
- Docker installed
- Kubernetes cluster access
- CI/CD pipeline configured

### Steps
1. Create release tag
2. Run test suite
3. Build Docker image
4. Push to container registry
5. Deploy to Kubernetes

## Rollback Procedure

In case of issues, rollback to previous version using:
```bash
kubectl rollout undo deployment/nexaflow-app
```

---

**Maintained by:** DevOps Team