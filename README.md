# SOC Home Lab – Wazuh SIEM

## Overview
This project demonstrates a Security Operations Center (SOC) home lab using **Wazuh SIEM** to collect, analyze, and monitor Linux security telemetry. The lab simulates real-world SOC workflows including log ingestion, audit monitoring, and agent-manager communication.

## Technologies Used
- Wazuh SIEM (Manager, Indexer, Dashboard)
- Docker & Docker Compose
- Linux (Ubuntu)
- auditd
- journald & syslog
- TCP-based agent communication

## Architecture
- Wazuh Manager, Indexer, and Dashboard deployed via Docker
- Linux endpoint configured as a Wazuh agent
- Logs collected from:
  - journald
  - syslog
  - dpkg package manager
  - authentication and sudo activity
- auditd rules enabled for identity and privilege monitoring

## Key Skills Demonstrated
- SIEM deployment and configuration
- Linux security monitoring
- Log ingestion and normalization
- Agent-based telemetry collection
- Troubleshooting configuration and connectivity issues
- Security auditing with auditd

## Validation
- Agent successfully connected and reporting to Wazuh Manager
- Logcollector confirmed ingestion of system and audit logs
- Security events visible in Wazuh Dashboard

## Notes
Sensitive information (IPs, certificates, credentials) has been intentionally excluded.
