# 06 - Risk Assessment

## Objective
Prioritize threats based on likelihood and impact. You can't fix everything at once, so risk assessment helps you focus on what matters most.

## Risk Assessment Formula

**Risk = Likelihood × Impact**

Where:
- **Likelihood**: How probable is this threat? (Rare, Unlikely, Possible, Likely, Almost Certain)
- **Impact**: How bad would it be? (Minimal, Minor, Moderate, Major, Catastrophic)

## Risk Rating Matrix

```
                    IMPACT
              Min  Minor Mod  Major Cata
        AC    Low  Med   High High  Crit
L   Likely    Low  Med   Med  High  Crit
I   Possible  Low  Low   Med  Med   High
K   Unlikely  Low  Low   Low  Med   Med
E   Rare      Low  Low   Low  Low   Med

AC = Almost Certain
```

## TODO: Assess Threat Likelihood

### TODO 1: Likelihood Factors

For each scenario, consider these factors:

**Your Answer:**
```
Credential Stuffing Account Takeover:

Attacker skill required: 
  □ Advanced  □ Intermediate  □ Basic  □ None
  
Attacker resources needed:
  □ Significant  □ Moderate  □ Minimal  □ None
  
Attack complexity:
  □ Very Complex  □ Complex  □ Moderate  □ Simple
  
Existing controls:
  □ Strong  □ Adequate  □ Weak  □ None
  
Known exploit availability:
  □ Public tools  □ Some tools  □ Rare  □ None

Past incidents of this type:
  □ Frequent  □ Regular  □ Occasional  □ Rare

Overall Likelihood Rating: 
  □ Almost Certain  □ Likely  □ Possible  □ Unlikely  □ Rare

Reasoning:




---

Race Condition Double-Spend:

Attacker skill required: 
  □ Advanced  □ Intermediate  □ Basic  □ None
  
Attacker resources needed:
  □ Significant  □ Moderate  □ Minimal  □ None
  
Attack complexity:
  □ Very Complex  □ Complex  □ Moderate  □ Simple
  
Existing controls:
  □ Strong  □ Adequate  □ Weak  □ None
  
Known exploit availability:
  □ Public tools  □ Some tools  □ Rare  □ None

Past incidents of this type:
  □ Frequent  □ Regular  □ Occasional  □ Rare

Overall Likelihood Rating: 
  □ Almost Certain  □ Likely  □ Possible  □ Unlikely  □ Rare

Reasoning:




---

[Continue for other scenarios from file 05]
Insider Data Exfiltration:

Overall Likelihood Rating: 


Reasoning:




---

API Rate Limit Bypass:

Overall Likelihood Rating: 


Reasoning:




---

Supply Chain Attack:

Overall Likelihood Rating: 


Reasoning:




```

## TODO: Assess Threat Impact

### TODO 2: Impact Factors

Rate the impact across multiple dimensions:

**Your Answer:**
```
Credential Stuffing Account Takeover:

Financial Impact:
  Direct losses: $___________
  Indirect costs: $___________
  Rating: □ Catastrophic □ Major □ Moderate □ Minor □ Minimal

Reputational Impact:
  User trust: 
  Media coverage: 
  Rating: □ Catastrophic □ Major □ Moderate □ Minor □ Minimal

Regulatory Impact:
  Violations: 
  Potential fines: $___________
  Rating: □ Catastrophic □ Major □ Moderate □ Minor □ Minimal

Operational Impact:
  Service downtime: 
  Recovery time: 
  Rating: □ Catastrophic □ Major □ Moderate □ Minor □ Minimal

Customer Impact:
  Users affected: 
  Data compromised: 
  Rating: □ Catastrophic □ Major □ Moderate □ Minor □ Minimal

Overall Impact Rating: 
  □ Catastrophic  □ Major  □ Moderate  □ Minor  □ Minimal

Justification:




---

Race Condition Double-Spend:

Financial Impact:
  Direct losses: $___________
  Indirect costs: $___________
  Rating: □ Catastrophic □ Major □ Moderate □ Minor □ Minimal

Reputational Impact:
  User trust: 
  Media coverage: 
  Rating: □ Catastrophic □ Major □ Moderate □ Minor □ Minimal

Regulatory Impact:
  Violations: 
  Potential fines: $___________
  Rating: □ Catastrophic □ Major □ Moderate □ Minor □ Minimal

Operational Impact:
  Service downtime: 
  Recovery time: 
  Rating: □ Catastrophic □ Major □ Moderate □ Minor □ Minimal

Customer Impact:
  Users affected: 
  Data compromised: 
  Rating: □ Catastrophic □ Major □ Moderate □ Minor □ Minimal

Overall Impact Rating: 
  □ Catastrophic  □ Major  □ Moderate  □ Minor  □ Minimal

Justification:




---

[Continue for other scenarios]
Insider Data Exfiltration:

Overall Impact Rating: 


Justification:




---

API Rate Limit Bypass:

Overall Impact Rating: 


Justification:




---

Supply Chain Attack:

Overall Impact Rating: 


Justification:




```

## TODO: Calculate Risk Scores

### TODO 3: Risk Matrix

Fill in your risk matrix:

**Your Answer:**
```
Threat                              | Likelihood    | Impact        | Risk Level
------------------------------------|---------------|---------------|------------
Credential Stuffing Account Takeover|               |               |
Race Condition Double-Spend         |               |               |
Insider Data Exfiltration          |               |               |
API Rate Limit Bypass              |               |               |
Supply Chain Attack                |               |               |
[Your Custom Scenario 1]           |               |               |
[Your Custom Scenario 2]           |               |               |
[Your Custom Scenario 3]           |               |               |
```

### TODO 4: Priority Rankings

Rank your threats from highest to lowest risk:

**Your Answer:**
```
CRITICAL RISK (Address Immediately):
1. 
   Likelihood:  Impact:  
   Why critical: 

2. 
   Likelihood:  Impact:  
   Why critical: 


HIGH RISK (Address Soon):
1. 
   Likelihood:  Impact:  

2. 
   Likelihood:  Impact:  

3. 
   Likelihood:  Impact:  


MEDIUM RISK (Address in Planning):
1. 
   Likelihood:  Impact:  

2. 
   Likelihood:  Impact:  

3. 
   Likelihood:  Impact:  


LOW RISK (Monitor/Accept):
1. 
   Likelihood:  Impact:  

2. 
   Likelihood:  Impact:  
```

## TODO: Risk Treatment Strategy

### TODO 5: Choose Risk Responses

For each high and critical risk, choose a response:
- **Mitigate**: Reduce likelihood or impact
- **Accept**: Risk is acceptable as-is
- **Transfer**: Insurance, vendor liability
- **Avoid**: Don't do the risky activity

**Your Answer:**
```
Risk: 
Response: □ Mitigate  □ Accept  □ Transfer  □ Avoid
Reasoning:



Risk: 
Response: □ Mitigate  □ Accept  □ Transfer  □ Avoid
Reasoning:



Risk: 
Response: □ Mitigate  □ Accept  □ Transfer  □ Avoid
Reasoning:



Risk: 
Response: □ Mitigate  □ Accept  □ Transfer  □ Avoid
Reasoning:



[Continue for all critical and high risks]




```

## TODO: Risk Acceptance Criteria

### TODO 6: Define What You'll Accept

Set thresholds for acceptable risk:

**Your Answer:**
```
Financial Risk Tolerance:
- Maximum acceptable loss per incident: $___________
- Maximum acceptable annual losses: $___________

Reputational Risk Tolerance:
- Acceptable PR incidents per year: ___________
- Acceptable user churn rate: ___________%

Regulatory Risk Tolerance:
- Acceptable compliance violations: ___________
- Maximum acceptable fine: $___________

Operational Risk Tolerance:
- Maximum acceptable downtime: ___________ hours/month
- Acceptable MTTR (Mean Time To Recovery): ___________ hours

Data Breach Risk Tolerance:
- Maximum acceptable records exposed: ___________
- Acceptable breach frequency: ___________ per year

Justification for these tolerances:




```

## TODO: Worst-Case Scenario Planning

### TODO 7: Nightmare Scenario

Describe your absolute worst-case scenario:

**Your Answer:**
```
The Nightmare Scenario:
What happens: 




Impact assessment:
- Financial: 
- Users affected: 
- Data compromised: 
- Recovery time: 
- Company survival: 


Likelihood this could actually happen:
□ Extremely unlikely but possible
□ Unlikely but we should prepare
□ More likely than we'd like to admit
□ We need to act NOW

Warning signs we'd see:
1. 
2. 
3. 


If this happened tomorrow, our response would be:
Immediate (0-24 hours):


Short-term (1-7 days):


Medium-term (1-4 weeks):


Long-term recovery:


Gaps in our response capability:
1. 
2. 
3. 
```

## Risk Assessment Checklist

Before moving on, verify:
- ✓ All scenarios have likelihood ratings
- ✓ All scenarios have impact ratings
- ✓ Risk levels are calculated using the matrix
- ✓ Top risks are clearly identified
- ✓ Risk response strategies are chosen
- ✓ Acceptance criteria are defined

## Common Risk Assessment Pitfalls

Watch out for:
- Overestimating your existing controls
- Underestimating attacker capabilities
- Focusing only on technical impact (ignoring business/regulatory)
- Assuming low likelihood means ignore it
- Not considering attack chains (multiple vulnerabilities combined)

## Reflection Questions

- Are you surprised by any of your risk ratings?
- Do your priorities align with business priorities?
- Which risks would keep executives up at night?
- Are there any "unknown unknowns" you're worried about?

## Next Steps

Proceed to `07-mitigations.md` to design security controls for your high-priority risks.
