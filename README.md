# Automating-Splunk-with-n8n

## Overview 
This project is an end-to-end SOC automation pipeline that demonstrates how modern security operations team automate triage, enrichment, and notification workflow using:

- Splunk (Detection)
- N8N (Orchestration)
- OpenAI (AI assisted triage)
- Slack (Alert delivery to analysts)

## Project Goal

**Build a fully automated workflow that:**

1. Detects security events in Splunk
2. Sends alerts to N8N through a webhook
3. Automatically triggers AI-powered triage using OpenAI
4. Enriches IOCs (IP / Hash) using AbuseIPDB & Virustotal
5. Sends a structured triage to a Slack channel which analysts can view

## Outcome

By completing this Proof of Concept, we demonstrate how SOC automation can:

- Reduce analyst time spent on repetitive enrichment
- Deliver consistent, structured triage reports
- Deliver alerts to Slack and instantly alert analysts

## Lab Enviroment 

| Component / Role             | Description                          | IP Address      |
| ---------------------------- | ------------------------------------ | --------------- |
| **Windows 10 Endpoint**      | Target machine sending Sysmon logs   | `192.168.1.100` |
| **Splunk Server**            | SIEM for log ingestion + alerts      | `192.168.1.9`   |
| **N8N Orchestration Server** | SOAR platform receiving webhooks     | `192.168.1.12`  |
