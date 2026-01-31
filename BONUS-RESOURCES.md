# Bonus Resources

## Quick Reference: STRIDE Cheat Sheet

### Spoofing Identity
**What**: Pretending to be something or someone else
**Questions to ask**:
- How do we authenticate users/services?
- Can authentication be bypassed?
- Can credentials be stolen or forged?
- Are there default credentials?

**Common examples**:
- Stolen credentials
- Session hijacking
- JWT token forgery
- IP spoofing
- Email spoofing

### Tampering with Data
**What**: Malicious modification of data
**Questions to ask**:
- Is data protected in transit?
- Is data protected at rest?
- Can users modify data they shouldn't?
- Are integrity checks in place?

**Common examples**:
- Man-in-the-middle attacks
- Database manipulation
- Configuration tampering
- Parameter manipulation
- Race conditions

### Repudiation
**What**: Denying that an action was performed
**Questions to ask**:
- Are user actions logged?
- Can logs be modified or deleted?
- Is there non-repudiation for critical actions?
- Can we prove who did what and when?

**Common examples**:
- Missing audit logs
- Modifiable logs
- Unsigned transactions
- No timestamp validation

### Information Disclosure
**What**: Exposing information to unauthorized parties
**Questions to ask**:
- Who can see what data?
- Is sensitive data encrypted?
- Are errors too verbose?
- Are debug endpoints exposed?

**Common examples**:
- SQL injection
- Path traversal
- Verbose error messages
- Exposed API keys
- Unencrypted data

### Denial of Service
**What**: Making a system unavailable
**Questions to ask**:
- Can services be overwhelmed?
- Are there rate limits?
- What are single points of failure?
- Is there resource exhaustion potential?

**Common examples**:
- DDoS attacks
- Resource exhaustion
- Algorithmic complexity attacks
- Database query bombs
- Infinite loops

### Elevation of Privilege
**What**: Gaining unauthorized capabilities
**Questions to ask**:
- How is authorization enforced?
- Can privilege checks be bypassed?
- Are there insecure defaults?
- Can users escalate privileges?

**Common examples**:
- SQL injection to admin
- Path traversal to system files
- Privilege escalation bugs
- Insecure direct object references
- Missing authorization checks

## Fintech-Specific Threat Patterns

### Payment Manipulation
- Amount tampering
- Currency manipulation
- Recipient swapping
- Double spending
- Negative amounts
- Integer overflow

### Account Takeover
- Credential stuffing
- Password spraying
- Session hijacking
- SIM swapping
- Social engineering
- Phishing

### Financial Fraud
- Card testing
- Chargeback fraud
- Refund abuse
- Synthetic identities
- Money laundering
- Transaction reversals

### Compliance Violations
- Insufficient KYC/AML
- Data residency issues
- Improper PII handling
- Missing consent
- Inadequate audit trails
- Report tampering

## Real-World Incident Examples

### Capital One (2019)
**What happened**: SSRF vulnerability + misconfigured S3 bucket
**Impact**: 100M+ records exposed
**Lesson**: Server-side request forgery + cloud misconfig = disaster
**Relevant to PayFlow**: AWS security, SSRF prevention, least privilege

### Equifax (2017)
**What happened**: Unpatched Apache Struts vulnerability
**Impact**: 147M+ records exposed
**Lesson**: Patch management is critical
**Relevant to PayFlow**: Dependency management, vulnerability scanning

### Twitter/X Bitcoin Scam (2020)
**What happened**: Social engineering + internal tools access
**Impact**: High-profile account compromise
**Lesson**: Insider threats and admin tool security
**Relevant to PayFlow**: Admin authentication, social engineering training

### Target (2013)
**What happened**: Third-party HVAC vendor compromise
**Impact**: 40M+ credit cards stolen
**Lesson**: Supply chain security matters
**Relevant to PayFlow**: Third-party risk management

### Colonial Pipeline (2021)
**What happened**: Ransomware via compromised credentials
**Impact**: Major fuel pipeline shutdown
**Lesson**: Credential protection and segmentation
**Relevant to PayFlow**: MFA, network segmentation

## Attack Tree Example

### Goal: Steal money from PayFlow user

```
                    [Steal Money]
                          |
        +----------------+----------------+
        |                                 |
   [Account              [Payment
   Takeover]            Manipulation]
        |                                 |
    +---+---+                        +----+----+
    |       |                        |         |
 [Steal  [Social               [Tamper    [Double
  Creds] Engineer]              Amount]    Spend]
    |       |                        |         |
  +-+-+   +-+-+                    +-+-+     +-+-+
  | | |   | | |                    | | |     | | |
 [P][C][K][Ph][V]                 [M][R][I] [C][T]

P = Phishing
C = Credential stuffing
K = Keylogger
Ph = Phone social engineering
V = Vishing
M = MITM
R = Race condition
I = Injection
C = Concurrent requests
T = Transaction replay
```

## Threat Modeling Anti-Patterns

### Don't Do This:
1. **Analysis paralysis**: Spending months without actionable output
2. **Security theater**: Focusing on easy but low-impact items
3. **One-and-done**: Treating threat modeling as a checkbox
4. **Expert-only**: Only security team does it
5. **No follow-up**: Great analysis, zero implementation
6. **Tool obsession**: Buying tools without doing the thinking
7. **Perfect is the enemy of good**: Waiting for perfect documentation

### Do This Instead:
1. **Time-box your analysis**: Set a deadline and ship it
2. **Risk-based prioritization**: Focus on what matters
3. **Continuous process**: Review regularly as system evolves
4. **Team activity**: Include developers, not just security
5. **Track mitigations**: Actually implement and measure
6. **Think first, tool second**: Tools amplify good process
7. **Iterate and improve**: Ship v1, then refine

## Useful Frameworks and Standards

### Security Frameworks
- **NIST Cybersecurity Framework**: Identify, Protect, Detect, Respond, Recover
- **OWASP ASVS**: Application Security Verification Standard
- **CIS Controls**: Critical Security Controls
- **MITRE ATT&CK**: Adversary tactics and techniques

### Compliance Standards
- **PCI-DSS**: Payment Card Industry Data Security Standard
- **SOC 2**: Service Organization Control 2
- **GDPR**: General Data Protection Regulation
- **CCPA**: California Consumer Privacy Act
- **ISO 27001**: Information Security Management

### Threat Modeling Methodologies
- **STRIDE**: Microsoft's threat classification (what you used)
- **PASTA**: Process for Attack Simulation and Threat Analysis
- **LINDDUN**: Privacy threat modeling
- **Attack Trees**: Hierarchical threat analysis
- **DREAD**: Risk assessment method (Damage, Reproducibility, Exploitability, Affected users, Discoverability)

## Security Testing Tools

### Static Analysis (SAST)
- Semgrep
- SonarQube
- Checkmarx
- Veracode

### Dynamic Analysis (DAST)
- OWASP ZAP
- Burp Suite
- Acunetix
- Nessus

### Dependency Scanning
- Snyk
- Dependabot
- WhiteSource
- npm audit

### API Security
- Postman
- REST-Assured
- OWASP API Security Top 10
- API Fuzzing tools

### Cloud Security
- AWS GuardDuty
- Azure Security Center
- Prowler
- ScoutSuite

## Learning Path

### Beginner
1. Complete this threat modeling exercise
2. Read OWASP Top 10
3. Learn about common vulnerabilities (SQL injection, XSS, CSRF)
4. Practice with deliberately vulnerable apps (WebGoat, DVWA)
5. Learn basic security concepts (authentication vs authorization, encryption)

### Intermediate
1. Study STRIDE in depth
2. Learn about specific attack techniques
3. Read incident reports and breach analyses
4. Practice on CTF challenges
5. Learn about secure coding practices
6. Study authentication and session management

### Advanced
1. Learn multiple threat modeling methodologies
2. Study cryptography and key management
3. Understand cloud security architectures
4. Learn about threat intelligence
5. Study incident response and forensics
6. Read academic security research
7. Contribute to security communities

## Books Worth Reading

### Threat Modeling
- "Threat Modeling: Designing for Security" by Adam Shostack
- "Threats: What Every Engineer Should Learn from Star Wars" by Adam Shostack

### Security
- "The Web Application Hacker's Handbook" by Stuttard & Pinto
- "Security Engineering" by Ross Anderson
- "Hacking: The Art of Exploitation" by Jon Erickson

### Fintech Security
- "Payments Systems in the U.S." by Carol Coye Benson
- "The PayTech Book" by Susanne Chishti & Tony Craddock

## Communities and Resources

### Online Communities
- OWASP Slack
- r/netsec
- Security Stack Exchange
- Hacker News
- Twitter #infosec

### Blogs and News
- Krebs on Security
- Schneier on Security
- Troy Hunt
- Dark Reading
- The Hacker News

### Conferences
- DEF CON
- Black Hat
- RSA Conference
- OWASP AppSec
- BSides events

### Practice Platforms
- HackTheBox
- TryHackMe
- PentesterLab
- PortSwigger Web Security Academy
- OWASP WebGoat

## Quick Start Guide

### If you have 30 minutes:
1. Read README.md
2. Skim 01-system-architecture.md
3. Fill out TODO 1 in 02-assets-and-trust-boundaries.md
4. Pick one component and do STRIDE analysis

### If you have 2 hours:
1. Complete files 01-03 thoroughly
2. Do STRIDE on 2-3 major components
3. Create 2-3 detailed threat scenarios
4. List top 5 risks

### If you have a full day:
1. Complete all files 01-07
2. Do comprehensive STRIDE analysis
3. Create 5+ detailed scenarios
4. Full risk assessment
5. Design mitigations for top 5 risks

### If you have a week:
1. Complete all 8 files thoroughly
2. Research real-world incidents
3. Create detailed implementation tickets
4. Draft incident response runbooks
5. Build monitoring dashboard design
6. Present findings to imaginary stakeholders

## Template: Quick Threat Model

For when you need a fast threat assessment:

```
System: __________
Date: __________
Analyst: __________

Top 3 Assets:
1. 
2. 
3. 

Top 3 Threats:
1. 
2. 
3. 

Top 3 Mitigations:
1. 
2. 
3. 

Risk Level: □ Critical □ High □ Medium □ Low

Next Review: __________
```

## Questions for Practice

Try answering these about PayFlow or your own systems:

1. If I could only fix ONE security issue, what would it be and why?
2. What would a sophisticated attacker target first?
3. Which component's compromise would be unrecoverable?
4. Where would we NOT detect a breach?
5. What keeps the CEO up at night?
6. Which threat is most likely in the next 6 months?
7. What would regulators care most about?
8. Where are we blindly trusting something we shouldn't?
9. What would make front-page news if it leaked?
10. Which control failure would cascade to others?

## Final Tips

1. **Start small**: Don't try to model everything at once
2. **Be specific**: "Attacker steals data" is too vague
3. **Think like an attacker**: What would you target?
4. **Involve the team**: Diverse perspectives find more threats
5. **Document decisions**: Why you chose to accept/mitigate risks
6. **Update regularly**: Systems change, so must threat models
7. **Measure effectiveness**: Track if controls actually work
8. **Learn from incidents**: Your own and others'
9. **Communicate clearly**: Translate security to business impact
10. **Take action**: A perfect threat model that sits on a shelf is worthless

Good luck with your security journey!
