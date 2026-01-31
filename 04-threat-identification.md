# 04 - Threat Identification (STRIDE)

## Objective
Systematically identify threats using the STRIDE framework. STRIDE helps ensure you don't miss major threat categories.

## What is STRIDE?

STRIDE is a mnemonic for six threat categories:

- **S**poofing - Pretending to be someone/something else
- **T**ampering - Modifying data or code
- **R**epudiation - Denying an action was taken
- **I**nformation Disclosure - Exposing information inappropriately
- **D**enial of Service - Making systems unavailable
- **E**levation of Privilege - Gaining unauthorized access

## How to Use STRIDE

For each component, data flow, or trust boundary, ask "What STRIDE threats apply here?"

## TODO: Apply STRIDE to PayFlow Components

### TODO 1: API Gateway Threats

**Spoofing Threats:**
```
S1: 

S2: 

S3: 
```

**Tampering Threats:**
```
T1: 

T2: 

T3: 
```

**Repudiation Threats:**
```
R1: 

R2: 
```

**Information Disclosure Threats:**
```
I1: 

I2: 

I3: 
```

**Denial of Service Threats:**
```
D1: 

D2: 

D3: 
```

**Elevation of Privilege Threats:**
```
E1: 

E2: 
```

### TODO 2: Authentication Service Threats

**Spoofing Threats:**
```
S1: Attacker steals user credentials and logs in as victim

S2: 

S3: 
```

**Tampering Threats:**
```
T1: 

T2: 

T3: 
```

**Repudiation Threats:**
```
R1: 

R2: 
```

**Information Disclosure Threats:**
```
I1: 

I2: 

I3: 
```

**Denial of Service Threats:**
```
D1: 

D2: 
```

**Elevation of Privilege Threats:**
```
E1: 

E2: 

E3: 
```

### TODO 3: Payment Service Threats

**Spoofing Threats:**
```
S1: 

S2: 

S3: 
```

**Tampering Threats:**
```
T1: Attacker modifies payment amount before processing

T2: 

T3: 

T4: 
```

**Repudiation Threats:**
```
R1: 

R2: 

R3: 
```

**Information Disclosure Threats:**
```
I1: 

I2: 

I3: 
```

**Denial of Service Threats:**
```
D1: 

D2: 
```

**Elevation of Privilege Threats:**
```
E1: 

E2: 
```

### TODO 4: Database Threats

**Spoofing Threats:**
```
S1: 

S2: 
```

**Tampering Threats:**
```
T1: 

T2: 

T3: 
```

**Repudiation Threats:**
```
R1: 

R2: 
```

**Information Disclosure Threats:**
```
I1: SQL injection exposes all user data

I2: 

I3: 

I4: 
```

**Denial of Service Threats:**
```
D1: 

D2: 
```

**Elevation of Privilege Threats:**
```
E1: 

E2: 
```

### TODO 5: External API Integration Threats (Plaid/Stripe)

**Spoofing Threats:**
```
S1: 

S2: 

S3: 
```

**Tampering Threats:**
```
T1: 

T2: 

T3: 
```

**Repudiation Threats:**
```
R1: 

R2: 
```

**Information Disclosure Threats:**
```
I1: 

I2: 

I3: 
```

**Denial of Service Threats:**
```
D1: 

D2: 
```

**Elevation of Privilege Threats:**
```
E1: 

E2: 
```

### TODO 6: Mobile/Web Client Threats

**Spoofing Threats:**
```
S1: 

S2: 

S3: 
```

**Tampering Threats:**
```
T1: 

T2: 

T3: 
```

**Repudiation Threats:**
```
R1: 

R2: 
```

**Information Disclosure Threats:**
```
I1: 

I2: 

I3: 
```

**Denial of Service Threats:**
```
D1: 

D2: 
```

**Elevation of Privilege Threats:**
```
E1: 

E2: 
```

## TODO: Apply STRIDE to Data Flows

### TODO 7: User Login Flow Threats

For each step in the login flow you mapped earlier, identify STRIDE threats:

**Your Answer:**
```
Step: User enters credentials on client

Spoofing: 
Tampering: 
Repudiation: 
Info Disclosure: 
DoS: 
Elevation: 

---

Step: Credentials transmitted to API Gateway

Spoofing: 
Tampering: 
Repudiation: 
Info Disclosure: 
DoS: 
Elevation: 

---

[Continue for each step]








```

### TODO 8: Payment Transaction Flow Threats

Identify threats in the payment flow:

**Your Answer:**
```
Step: User initiates payment

Spoofing: 
Tampering: 
Repudiation: 
Info Disclosure: 
DoS: 
Elevation: 

---

Step: Payment validation

Spoofing: 
Tampering: 
Repudiation: 
Info Disclosure: 
DoS: 
Elevation: 

---

[Continue for each step]








```

## TODO: Cross-Cutting Threats

### TODO 9: Identify System-Wide Threats

Some threats affect multiple components:

**Your Answer:**
```
Supply Chain / Dependencies:
- Threat: 
- Affected components: 
- Impact: 

- Threat: 
- Affected components: 
- Impact: 


Insider Threats:
- Threat: 
- Affected components: 
- Impact: 

- Threat: 
- Affected components: 
- Impact: 


Configuration Issues:
- Threat: 
- Affected components: 
- Impact: 

- Threat: 
- Affected components: 
- Impact: 


Cryptographic Failures:
- Threat: 
- Affected components: 
- Impact: 

- Threat: 
- Affected components: 
- Impact: 


Logging/Monitoring Blind Spots:
- Threat: 
- Affected components: 
- Impact: 

- Threat: 
- Affected components: 
- Impact: 
```

## STRIDE Quick Reference Card

When stuck, use these prompting questions:

**Spoofing**: Can someone pretend to be someone/something else?
- Weak authentication?
- Missing authentication?
- Token theft possible?

**Tampering**: Can data or code be maliciously modified?
- Unencrypted transport?
- No integrity checks?
- Unsigned code/configs?

**Repudiation**: Can someone deny they did something?
- Missing audit logs?
- Logs can be modified?
- No non-repudiation mechanism?

**Information Disclosure**: Can someone see data they shouldn't?
- Excessive permissions?
- Data in logs/errors?
- Weak encryption?

**Denial of Service**: Can someone make the system unavailable?
- No rate limiting?
- Resource exhaustion possible?
- Single point of failure?

**Elevation of Privilege**: Can someone gain unauthorized access?
- Privilege escalation bugs?
- Insecure defaults?
- Missing authorization checks?

## Reflection Questions

- Did you find at least 3-5 threats per component?
- Are you thinking like an attacker?
- Did you consider both technical and business logic threats?
- Have you covered all major data flows?

## Next Steps

Proceed to `05-threat-scenarios.md` to develop detailed attack scenarios.
