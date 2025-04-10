# Microsoft Sentinel Lab - Day 1

This repository contains my hands-on labs and detection projects using Microsoft Sentinel as part of my 11-day Sentinel training series.

## 🧠 Key Concepts
- Microsoft Sentinel as a cloud-native SIEM and SOAR platform
- Sentinel's role in a modern Security Operations Center (SOC)
- Integration with Microsoft Defender XDR for threat detection and response

## 🧪 Lab Activities
- Deployed Microsoft Sentinel
- Connected Azure Activity Logs as data source
- Ran KQL queries to investigate sign-in patterns

## 🔍 Sample KQL Query
```kql
SigninLogs
| summarize SignInCount = count() by UserPrincipalName
| order by SignInCount desc
