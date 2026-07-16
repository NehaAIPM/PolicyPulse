# PolicyPulse
PolicyPulse POC

## AI-Powered HR Policy Change Detection & Employee Impact Analysis

PolicyPulse is an AI-powered HR policy intelligence agent designed to help organizations identify changes between policy versions and understand how those changes impact employees.

HR policies evolve frequently due to regulatory updates, organizational changes, and business requirements. Manually reviewing policy documents and determining affected employee groups can be time-consuming and error-prone. PolicyPulse automates this process by analyzing policy documents, detecting meaningful changes, and generating targeted employee impact insights.

## Key Capabilities

- **Automated Policy Comparison**
  - Upload multiple versions of HR policy documents and automatically identify changes.
  - Detect updates in areas such as eligibility rules, accrual calculations, benefits, timelines, and policy limits.

- **AI-Powered Change Analysis**
  - Uses Large Language Models (LLMs) to understand policy context rather than relying only on text differences.
  - Highlights meaningful business changes while ignoring formatting or insignificant edits.

- **Employee Impact Detection**
  - Maps policy changes against employee attributes such as tenure, location, employment type, and eligibility criteria.
  - Identifies which employees or employee groups may be affected by policy updates.

- **Actionable Notifications**
  - Generates employee-specific summaries explaining relevant policy changes.
  - Helps HR teams proactively communicate updates to impacted employees.

- **Structured AI Output**
  - Produces consistent JSON-based insights that can be consumed by HR applications, workflows, or notification systems.

## Example Use Case

An organization updates its Annual PTO Policy:

**Previous Policy**
- Employees accrue 15 PTO days annually.
- PTO requests require 5 days advance notice.
- Carryover limit is 20 days.

**Updated Policy**
- Employees with 3+ years tenure accrue 20 PTO days.
- PTO requests require 10 days advance notice.
- Carryover limit increases to 30 days.

PolicyPulse identifies:
- What changed
- Who is impacted
- How employees are affected
- Recommended communication messages


## Architecture Overview

PolicyPulse combines document processing, AI reasoning, and employee data analysis.

High-level workflow:

1. HR uploads policy documents.
2. Policy documents are extracted and processed.
3. AI analyzes differences between policy versions.
4. Employee data is evaluated against policy rules.
5. Impacted employees receive targeted insights.

## Technology Stack

- **AI/LLM:** Large Language Models for policy understanding and reasoning
- **Workflow Automation:** n8n
- **Frontend:** React / Next.js
- **Backend Integration:** Webhooks and API-based communication
- **Data Storage:** Supabase
- **Document Processing:** PDF extraction and structured analysis

## Project Goals

PolicyPulse aims to reduce manual HR operations by transforming static policy documents into actionable employee intelligence. It enables HR teams to move from reactive policy communication to proactive, personalized employee engagement.

## Future Enhancements

- Integration with HRIS platforms such as Workday
- Automated policy ingestion from document repositories
- Multi-language policy analysis
- Compliance risk detection
- HR chatbot interface for policy questions

