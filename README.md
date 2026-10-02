# AI Chatbot Security Assessment

## Overview

A hands-on security assessment of an intentionally vulnerable AI customer-support chatbot in an authorized, isolated lab environment.

The project focused on identifying AI application security weaknesses, reproducing them, implementing mitigations, retesting the application, and documenting residual risk.

> **Transparency:** This is a self-directed learning project completed with guidance from Claude AI. It is not employment, commercial client work, or production security experience.

## Security Findings

The assessment focused on:

- Direct Prompt Injection
- System Prompt Leakage
- Sensitive information exposure through model context
- Output-control weaknesses
- Mitigation bypass and residual-risk analysis

### Security Mapping

- OWASP LLM01 – Prompt Injection
- OWASP LLM07 – System Prompt Leakage
- CWE-1427 – Improper Neutralization of Input Used for LLM Prompting
- CWE-200 – Exposure of Sensitive Information

## Hands-On Workflow

1. Deployed and tested the vulnerable chatbot locally
2. Established baseline application behavior
3. Reproduced prompt-injection attacks
4. Confirmed system-prompt information leakage
5. Validated the finding through the lab verification workflow
6. Applied a mitigation to keep credential-style secrets outside the model context
7. Rebuilt and retested the application
8. Added an output-side leak check
9. Tested multiple attack variants
10. Identified a character-spacing bypass and documented the remaining residual risk

## Tools & Environment

- Docker Desktop
- Docker Compose
- Windows PowerShell
- Git
- Local Browser
- AI-assisted learning and troubleshooting with Claude AI

## Key Learning

This project helped me understand that AI security testing is not limited to discovering prompt-injection vulnerabilities.

The complete workflow included:

**Attack → Evidence → Root Cause → Mitigation → Retest → Bypass Testing → Residual Risk → Reporting**

A key lesson was that simple output filtering can reduce obvious leakage but should not be treated as a complete security boundary.

## Security Report

A detailed security assessment report was prepared covering:

- Executive Summary
- Scope and Methodology
- Findings Register
- Technical Evidence
- OWASP LLM and CWE Mapping
- Root-Cause Analysis
- Remediation
- Retest Results
- Residual Risk
- Security / GRC Roadmap
- Limitations and Assumptions

## Ethical Scope

All testing was performed against a deliberately vulnerable application in an authorized local lab environment.

No third-party or production systems were tested.

## Author

**Harshit Ojha**  
Cybersecurity Fresher | VAPT | Web Application Security | AI Application Security

LinkedIn: https://www.linkedin.com/in/harshit-ojha-717503211/
