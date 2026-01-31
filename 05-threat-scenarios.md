# 05 - Threat Scenarios

## Objective
Develop detailed, realistic attack scenarios. Moving from abstract threats to concrete scenarios helps prioritize risks and design effective mitigations.

## What is a Threat Scenario?

A threat scenario describes:
- **Who**: The attacker (skill level, motivation, resources)
- **What**: Their goal (steal money, steal data, disrupt service)
- **How**: Step-by-step attack method
- **Impact**: What happens if they succeed

## TODO: Develop Attack Scenarios

### TODO 1: Account Takeover Scenario

**Scenario Name**: Credential Stuffing Account Takeover

**Your Answer:**
```
Attacker Profile:
- Skill level: 
- Resources: 
- Motivation: 


Attack Goal:
What they want to achieve: 


Attack Prerequisites:
What the attacker needs first:
1. 
2. 
3. 


Attack Steps:
Step 1: 

Step 2: 

Step 3: 

Step 4: 

Step 5: 


Success Indicators (from attacker's POV):
- 
- 


Impact if Successful:
Financial: 
Reputational: 
Regulatory: 
User trust: 


Current Defenses (if any):
- 
- 


Defense Gaps:
What would make this attack easier:
1. 
2. 
3. 
```

### TODO 2: Payment Fraud Scenario

**Scenario Name**: Race Condition Double-Spend Attack

**Your Answer:**
```
Attacker Profile:
- Skill level: 
- Resources: 
- Motivation: 


Attack Goal:


Attack Prerequisites:
1. 
2. 
3. 


Attack Steps:
Step 1: 

Step 2: 

Step 3: 

Step 4: 

Step 5: 


Success Indicators:


Impact if Successful:
Financial: 
Reputational: 
Regulatory: 
User trust: 


Current Defenses:


Defense Gaps:
1. 
2. 
3. 
```

### TODO 3: Insider Threat Scenario

**Scenario Name**: Malicious Employee Data Exfiltration

**Your Answer:**
```
Attacker Profile:
- Role: 
- Access level: 
- Motivation: 


Attack Goal:


Attack Prerequisites:


Attack Steps:
Step 1: 

Step 2: 

Step 3: 

Step 4: 

Step 5: 


Success Indicators:


Impact if Successful:
Financial: 
Reputational: 
Regulatory: 
User trust: 


Current Defenses:


Defense Gaps:
1. 
2. 
3. 
```

### TODO 4: API Abuse Scenario

**Scenario Name**: API Rate Limit Bypass for Enumeration

**Your Answer:**
```
Attacker Profile:
- Skill level: 
- Resources: 
- Motivation: 


Attack Goal:


Attack Prerequisites:


Attack Steps:
Step 1: 

Step 2: 

Step 3: 

Step 4: 

Step 5: 


Success Indicators:


Impact if Successful:
Financial: 
Reputational: 
Regulatory: 
User trust: 


Current Defenses:


Defense Gaps:
1. 
2. 
3. 
```

### TODO 5: Supply Chain Attack Scenario

**Scenario Name**: Compromised NPM Dependency

**Your Answer:**
```
Attacker Profile:
- Skill level: 
- Resources: 
- Motivation: 


Attack Goal:


Attack Prerequisites:


Attack Steps:
Step 1: 

Step 2: 

Step 3: 

Step 4: 

Step 5: 


Success Indicators:


Impact if Successful:
Financial: 
Reputational: 
Regulatory: 
User trust: 


Current Defenses:


Defense Gaps:
1. 
2. 
3. 
```

### TODO 6: Social Engineering Scenario

**Scenario Name**: Customer Service Impersonation

**Your Answer:**
```
Attacker Profile:
- Skill level: 
- Resources: 
- Motivation: 


Attack Goal:


Attack Prerequisites:


Attack Steps:
Step 1: 

Step 2: 

Step 3: 

Step 4: 

Step 5: 


Success Indicators:


Impact if Successful:
Financial: 
Reputational: 
Regulatory: 
User trust: 


Current Defenses:


Defense Gaps:
1. 
2. 
3. 
```

## TODO: Create Your Own Scenarios

### TODO 7: Custom Scenario 1

Pick a threat from your STRIDE analysis and develop it into a full scenario:

**Scenario Name**: 

**Your Answer:**
```
Attacker Profile:


Attack Goal:


Attack Prerequisites:


Attack Steps:







Success Indicators:


Impact if Successful:


Current Defenses:


Defense Gaps:


```

### TODO 8: Custom Scenario 2

**Scenario Name**: 

**Your Answer:**
```
Attacker Profile:


Attack Goal:


Attack Prerequisites:


Attack Steps:







Success Indicators:


Impact if Successful:


Current Defenses:


Defense Gaps:


```

### TODO 9: Custom Scenario 3

**Scenario Name**: 

**Your Answer:**
```
Attacker Profile:


Attack Goal:


Attack Prerequisites:


Attack Steps:







Success Indicators:


Impact if Successful:


Current Defenses:


Defense Gaps:


```

## TODO: Attack Chain Analysis

### TODO 10: Multi-Stage Attack
Describe an attack that combines multiple vulnerabilities:

**Your Answer:**
```
Attack Chain Name: 


Stage 1: Initial Access
- Vulnerability exploited: 
- What attacker gains: 


Stage 2: Lateral Movement
- Vulnerability exploited: 
- What attacker gains: 


Stage 3: Privilege Escalation
- Vulnerability exploited: 
- What attacker gains: 


Stage 4: Objective Completion
- Final action: 
- Impact: 


Why this chain is dangerous:
1. 
2. 
3. 


Critical points where this could be stopped:
1. 
2. 
3. 
```

## Real-World Examples to Research

To make your scenarios more realistic, research these actual fintech incidents:
- Capital One breach (2019) - SSRF and misconfigured S3
- Equifax breach (2017) - Unpatched vulnerability
- Cash App breach (2022) - Insider access
- PayPal 2FA bypass incidents
- Plaid security issues

### TODO 11: Research Notes

Pick one real incident and analyze it:

**Your Answer:**
```
Incident: 


What happened:


How it relates to PayFlow:


Lessons learned:
1. 
2. 
3. 


How PayFlow could be vulnerable:


How to prevent in PayFlow:


```

## Scenario Evaluation Checklist

For each scenario, ask:
- ✓ Is this technically feasible?
- ✓ Does the attacker motivation make sense?
- ✓ Have I considered detection opportunities?
- ✓ Is the impact assessment realistic?
- ✓ Are there similar real-world examples?

## Reflection Questions

- Which scenarios keep you up at night?
- Which are most likely vs. most impactful?
- Where are your biggest blind spots?
- Which scenarios would be hardest to detect?

## Next Steps

Proceed to `06-risk-assessment.md` to prioritize these threats based on likelihood and impact.
