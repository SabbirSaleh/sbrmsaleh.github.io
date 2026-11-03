---
layout: hybrid-project
title: "DevSecLogs"
subtitle: "Stage-aware CI/CD security evidence modelling and verification"
permalink: "/projects/devseclogs/"
status: "Research prototype and demonstration"
demo_url: "https://devseclogs.sbrmsaleh.com/"
capabilities:
  - "Stage-aware analysis of CI/CD logs and observations across source, build, test, package, deploy and runtime"
  - "Deterministic reason codes connecting findings to inspection-ready observations"
  - "Run-level triage, alerts and evidence-related records"
  - "Local evidence digest verification and tamper simulation"
  - "Research-oriented IBM Cloud deployments and demonstration scenarios"
limitations:
  - "Not a production-managed security service"
  - "Triage priorities and risk scores do not establish confirmed attacks"
  - "The public demonstration may use browser-local state and local digest commitments; backend integrations and external anchoring are separately scoped"
---

DevSecLogs is an analyst-facing research prototype that reconstructs, interprets and verifies security-relevant evidence across the software delivery pipeline. It is designed to complement scanners and policy engines, not replace them or assert incident attribution.
