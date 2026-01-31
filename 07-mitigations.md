# 07 - Mitigations

## Objective
Design security controls to reduce risk. For each high-priority threat, define specific, actionable mitigations.

## Defense in Depth

Good security uses multiple layers:
1. **Prevent** - Stop attacks before they start
2. **Detect** - Identify attacks in progress
3. **Respond** - Contain and remediate attacks
4. **Recover** - Restore normal operations

## TODO: Design Mitigations

### TODO 1: Credential Stuffing Mitigation

Based on your risk assessment, design controls to address credential stuffing:

**Your Answer:**
```
PREVENTIVE CONTROLS:

Technical:
1. Control: 
   How it works: 
   Implementation complexity: □ High □ Medium □ Low
   Cost: □ High □ Medium □ Low

2. Control: 
   How it works: 
   Implementation complexity: □ High □ Medium □ Low
   Cost: □ High □ Medium □ Low

3. Control: 
   How it works: 
   Implementation complexity: □ High □ Medium □ Low
   Cost: □ High □ Medium □ Low

Process/Policy:
1. 
2. 
3. 


DETECTIVE CONTROLS:

Monitoring:
1. What to monitor: 
   Alert threshold: 
   Response time: 

2. What to monitor: 
   Alert threshold: 
   Response time: 

Logging:
1. What to log: 
   Retention: 
   Analysis method: 


RESPONSIVE CONTROLS:

Automated Response:
1. Trigger: 
   Action: 
   Duration: 

2. Trigger: 
   Action: 
   Duration: 

Manual Response Procedures:
1. 
2. 
3. 


RECOVERY CONTROLS:

User Notification:
Method: 
Timeline: 
Content: 

Account Recovery:
Process: 
Timeline: 
Verification: 


EFFECTIVENESS ASSESSMENT:
How much does this reduce risk?
Likelihood reduction: ___% → ___%
Impact reduction: ___% → ___%
Residual risk: □ Critical □ High □ Medium □ Low


IMPLEMENTATION PRIORITY:
□ P0 - Immediate (this week)
□ P1 - Urgent (this month)
□ P2 - Important (this quarter)
□ P3 - Nice to have (backlog)
```

### TODO 2: Payment Fraud Mitigation

Design controls for race condition and payment manipulation:

**Your Answer:**
```
PREVENTIVE CONTROLS:

Technical:
1. Control: 
   How it works: 
   Implementation complexity: □ High □ Medium □ Low
   Cost: □ High □ Medium □ Low

2. Control: 
   How it works: 
   Implementation complexity: □ High □ Medium □ Low
   Cost: □ High □ Medium □ Low

3. Control: 
   How it works: 
   Implementation complexity: □ High □ Medium □ Low
   Cost: □ High □ Medium □ Low


DETECTIVE CONTROLS:

Fraud Detection:
1. Signal: 
   Detection method: 
   False positive rate: 

2. Signal: 
   Detection method: 
   False positive rate: 

Transaction Monitoring:
1. What to monitor: 
   Analysis: 
   Alert on: 


RESPONSIVE CONTROLS:

Real-time Response:
1. Trigger: 
   Action: 

2. Trigger: 
   Action: 

Post-transaction Review:
Process: 
Timeline: 
Escalation: 


RECOVERY CONTROLS:

Reversal Process:
When: 
Who approves: 
Timeline: 

User Communication:
When: 
Method: 
Content: 


EFFECTIVENESS ASSESSMENT:
Likelihood reduction: ___% → ___%
Impact reduction: ___% → ___%
Residual risk: □ Critical □ High □ Medium □ Low


IMPLEMENTATION PRIORITY:
□ P0 - Immediate
□ P1 - Urgent
□ P2 - Important
□ P3 - Nice to have
```

### TODO 3: Insider Threat Mitigation

Design controls for malicious or compromised employees:

**Your Answer:**
```
PREVENTIVE CONTROLS:

Access Control:
1. Control: 
   How it works: 
   Implementation: 

2. Control: 
   How it works: 
   Implementation: 

Separation of Duties:
1. What's separated: 
   Why: 

2. What's separated: 
   Why: 


DETECTIVE CONTROLS:

User Behavior Analytics:
1. Behavior monitored: 
   Baseline: 
   Alert on: 

2. Behavior monitored: 
   Baseline: 
   Alert on: 

Audit Logging:
1. What's logged: 
   Who reviews: 
   Frequency: 


RESPONSIVE CONTROLS:

Alert Response:
1. Alert type: 
   Response: 
   Timeline: 

Investigation Process:
Trigger: 
Steps: 
Escalation: 


RECOVERY CONTROLS:

Access Revocation:
When: 
How: 
Verification: 

Incident Response:
Process: 
Key stakeholders: 


EFFECTIVENESS ASSESSMENT:
Likelihood reduction: ___% → ___%
Impact reduction: ___% → ___%
Residual risk: □ Critical □ High □ Medium □ Low


IMPLEMENTATION PRIORITY:
□ P0 - Immediate
□ P1 - Urgent
□ P2 - Important
□ P3 - Nice to have
```

### TODO 4: API Security Mitigation

Design controls for API abuse and rate limiting:

**Your Answer:**
```
PREVENTIVE CONTROLS:

Rate Limiting:
1. Endpoint: 
   Limit: 
   Window: 
   Scope: 

2. Endpoint: 
   Limit: 
   Window: 
   Scope: 

Authentication/Authorization:
1. Method: 
   Tokens: 
   Expiration: 

Input Validation:
1. What's validated: 
   How: 
   Rejection handling: 


DETECTIVE CONTROLS:

API Monitoring:
1. Metric: 
   Threshold: 
   Alert: 

2. Metric: 
   Threshold: 
   Alert: 

Anomaly Detection:
Pattern: 
Detection method: 
Response: 


RESPONSIVE CONTROLS:

Automated Throttling:
Trigger: 
Action: 
Duration: 

IP Blocking:
Criteria: 
Duration: 
Whitelist process: 


RECOVERY CONTROLS:

Service Recovery:
Process: 
Verification: 

Customer Communication:
When: 
Method: 


EFFECTIVENESS ASSESSMENT:
Likelihood reduction: ___% → ___%
Impact reduction: ___% → ___%
Residual risk: □ Critical □ High □ Medium □ Low


IMPLEMENTATION PRIORITY:
□ P0 - Immediate
□ P1 - Urgent
□ P2 - Important
□ P3 - Nice to have
```

### TODO 5: Supply Chain Security Mitigation

Design controls for dependency and third-party risks:

**Your Answer:**
```
PREVENTIVE CONTROLS:

Dependency Management:
1. Control: 
   How: 
   Frequency: 

2. Control: 
   How: 
   Frequency: 

Vendor Security:
1. Assessment: 
   Frequency: 
   Criteria: 

Code Integrity:
1. Verification: 
   How: 
   When: 


DETECTIVE CONTROLS:

Vulnerability Scanning:
1. What's scanned: 
   Tool: 
   Frequency: 
   Action on finding: 

2. What's scanned: 
   Tool: 
   Frequency: 
   Action on finding: 

Behavior Monitoring:
What: 
How: 
Alert on: 


RESPONSIVE CONTROLS:

Incident Response:
Trigger: 
Steps: 
Timeline: 

Vendor Notification:
When: 
How: 
Requirements: 


RECOVERY CONTROLS:

Rollback Process:
When: 
How: 
Testing: 

Alternative Vendor:
Criteria: 
Preparation: 


EFFECTIVENESS ASSESSMENT:
Likelihood reduction: ___% → ___%
Impact reduction: ___% → ___%
Residual risk: □ Critical □ High □ Medium □ Low


IMPLEMENTATION PRIORITY:
□ P0 - Immediate
□ P1 - Urgent
□ P2 - Important
□ P3 - Nice to have
```

## TODO: Design Your Own Mitigations

### TODO 6: Custom Threat Mitigation 1

For your first custom threat from file 05:

**Threat:** 

**Your Answer:**
```
PREVENTIVE CONTROLS:






DETECTIVE CONTROLS:






RESPONSIVE CONTROLS:






RECOVERY CONTROLS:






EFFECTIVENESS ASSESSMENT:
Likelihood reduction: ___% → ___%
Impact reduction: ___% → ___%
Residual risk: □ Critical □ High □ Medium □ Low
```

### TODO 7: Custom Threat Mitigation 2

**Threat:** 

**Your Answer:**
```
[Same structure as above]






```

## TODO: Cross-Cutting Security Controls

### TODO 8: Foundational Security Measures

Design baseline security that protects against multiple threats:

**Your Answer:**
```
ENCRYPTION:

Data in Transit:
- Protocol: 
- Cipher suites: 
- Certificate management: 

Data at Rest:
- Method: 
- Key management: 
- Encryption scope: 

Data in Use:
- Sensitive fields: 
- Protection method: 


AUTHENTICATION:

User Authentication:
- Primary method: 
- MFA: 
- Password policy: 
- Session management: 

Service Authentication:
- Method: 
- Key rotation: 
- Scope: 


AUTHORIZATION:

Access Control Model:
- Model: 
- Granularity: 
- Default policy: 

Role Definition:
Role 1: 
  Permissions: 
  
Role 2: 
  Permissions: 


LOGGING & MONITORING:

Security Events Logged:
1. 
2. 
3. 
4. 
5. 

Log Storage:
- Location: 
- Retention: 
- Access control: 

Monitoring Strategy:
- Real-time alerts: 
- Periodic review: 
- Automated analysis: 


NETWORK SECURITY:

Segmentation:
- Segments: 
- Communication rules: 

Perimeter Defense:
- WAF rules: 
- DDoS protection: 
- Geographic restrictions: 


INCIDENT RESPONSE:

Detection:
- Methods: 
- Responsibility: 

Response Team:
- Members: 
- Escalation: 

Response Process:
1. 
2. 
3. 
4. 
5. 

Communication Plan:
- Internal: 
- External: 
- Regulatory: 
```

## TODO: Mitigation Roadmap

### TODO 9: Implementation Plan

Prioritize and sequence your mitigations:

**Your Answer:**
```
PHASE 1 - IMMEDIATE (Week 1-2):
Critical gaps that must be addressed now

1. Mitigation: 
   Effort: 
   Owner: 
   Dependencies: 

2. Mitigation: 
   Effort: 
   Owner: 
   Dependencies: 

3. Mitigation: 
   Effort: 
   Owner: 
   Dependencies: 


PHASE 2 - SHORT TERM (Month 1-3):
High-priority improvements

1. Mitigation: 
   Effort: 
   Owner: 
   Dependencies: 

2. Mitigation: 
   Effort: 
   Owner: 
   Dependencies: 


PHASE 3 - MEDIUM TERM (Quarter 2-3):
Important enhancements

1. Mitigation: 
   Effort: 
   Owner: 
   Dependencies: 


PHASE 4 - LONG TERM (Quarter 4+):
Strategic improvements

1. Mitigation: 
   Effort: 
   Owner: 
   Dependencies: 
```

### TODO 10: Resource Requirements

Estimate resources needed:

**Your Answer:**
```
PERSONNEL:
Engineering: ___ FTEs for ___ months
Security: ___ FTEs for ___ months
Operations: ___ FTEs for ___ months

Key skills needed:
1. 
2. 
3. 


BUDGET:
Tools/Services: $___________
Infrastructure: $___________
Training: $___________
Consulting: $___________
Total: $___________


TIMELINE:
Start date: 
Critical milestones:
1. 
2. 
3. 

Completion target: 
```

## Mitigation Checklist

Verify your mitigations:
- ✓ Address root cause, not just symptoms
- ✓ Include prevent, detect, respond, recover
- ✓ Consider implementation complexity
- ✓ Account for false positives
- ✓ Include monitoring and metrics
- ✓ Define ownership and responsibilities
- ✓ Prioritized based on risk reduction

## Reflection Questions

- Have you addressed your highest risks?
- Are your controls practical to implement?
- Do you have defense in depth?
- Can you measure control effectiveness?
- What's your residual risk after mitigations?

## Next Steps

Proceed to `08-action-plan.md` to create your final remediation roadmap.
