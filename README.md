# GitOps Security Observability

This project implements a low-cost, cloud-native pipeline to detect,
store, and visualize GitOps security and compliance violations.

## High-level Architecture
- GitHub Actions runs Gitleaks on PRs and pushes
- Scan results are stored in GCS
- Cloud Composer (Airflow) ingests findings into BigQuery
- Grafana visualizes security and compliance metrics

## Tech Stack
- GCP: Cloud Composer, BigQuery, Cloud Storage
- CI/CD: GitHub Actions
- Security: Gitleaks
- Observability: Grafana
