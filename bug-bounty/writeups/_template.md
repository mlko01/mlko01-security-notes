---
title: "[Vuln Type] on [Target Type / Redacted Scope]"
description: "Vulnerability analysis, exploitation proof of concept, and business impact."
---

# [Vulnerability Type] - [Target / Scope]

| Metadata | Value |
| :--- | :--- |
| **Vulnerability Class** | (e.g. IDOR, SSRF, BAC, Logic Flaw) |
| **Platform / Program** | (e.g. HackerOne / Bugcrowd / Private Program) |
| **Severity** | Critical / High / Medium / Low |
| **Status** | Resolved & Disclosed / Accepted Impact |
| **Date** | YYYY-MM-DD |

---

## 1. Summary
Brief non-technical overview explaining what the vulnerability was and the core asset affected.

## 2. Technical Breakdown & Reproduction
Step-by-step reproduction guide with minimal noise.

1. Navigate to endpoint...
2. Intercept and modify the following parameter:

```http
POST /api/v2/resource/update HTTP/1.1
Host: target.example.com
Authorization: Bearer <USER_B_TOKEN>
Content-Type: application/json

{
  "account_id": "VICTIM_ID",
  "role": "admin"
}
