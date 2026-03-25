# SOC Automation Project (AI-Augmented)

## 🎯 Project Objective
The goal of this project is to build an end-to-end Security Operations Center (SOC) pipeline that automates the detection, analysis, and notification of security threats. By integrating a SIEM (Splunk) with a SOAR (n8n) and AI, I am reducing the time it takes to respond to incidents.

## 🛠️ The Tech Stack
- **OS:** Kali Linux (Host), Windows 10 (Target)
- **SIEM:** Splunk Enterprise
- **Telemetry:** Windows Sysmon
- **SOAR:** n8n
- **Intelligence:** AI (LLM) for log summarization
- **Alerting:** Telegram/Slack

## 🏗️ Logical Architecture
1. **Generate:** Sysmon captures deep-level endpoint logs on Windows.
2. **Ingest:** Splunk Universal Forwarder sends logs to Splunk on Kali Linux.
3. **Trigger:** Splunk identifies a threat and sends a Webhook to n8n.
4. **Analyze:** n8n sends the log to an AI for a human-readable summary.
5. **Notify:** The analyst receives a detailed report on their mobile device.

## 📈 Roadmap (Current Status: 🟢 Planning)
- [x] Project Architecture Design
- [ ] Virtual Lab Environment Setup (VMware/VirtualBox)
- [ ] Sysmon Installation & Configuration
- [ ] Splunk Data Ingestion
- [ ] n8n Workflow Integration
- [ ] Live Testing & Documentation
