# 02 - Assets and Trust Boundaries

## Objective
Identify what you're protecting (assets) and where trust changes (boundaries). Threats occur when untrusted entities cross boundaries to access assets.

## What Are Assets?

Assets are anything of value that needs protection:
- Data (customer PII, financial records)
- Services (payment processing capability)
- Reputation (brand trust)
- Compliance (regulatory standing)

## What Are Trust Boundaries?

Trust boundaries are where the level of trust changes:
- Internet → Your network
- User device → Backend servers
- One microservice → Another microservice
- Application code → Database
- Your infrastructure → Third-party API

## TODO: Asset Identification

### TODO 1: List Critical Assets
Identify and categorize PayFlow's critical assets:

**Your Answer:**
```
DATA ASSETS:
1. 

2. 

3. 

4. 

5. 


SYSTEM ASSETS:
1. 

2. 

3. 


BUSINESS ASSETS:
1. 

2. 

3. 


```

### TODO 2: Asset Valuation
For each asset category, answer:
- What happens if it's stolen?
- What happens if it's modified?
- What happens if it's unavailable?

**Your Answer:**
```
Customer PII (names, addresses, SSN):
- If stolen: 



- If modified: 



- If unavailable: 




Transaction Records:
- If stolen: 



- If modified: 



- If unavailable: 




User Credentials:
- If stolen: 



- If modified: 



- If unavailable: 




[Continue for other critical assets]


```

### TODO 3: Draw Trust Boundaries

Map out the trust boundaries in PayFlow. Use this template:

**Your Answer:**
```
Trust Boundary 1: Internet ←→ API Gateway
- Trust Level Changes From: Completely untrusted
- Trust Level Changes To: 
- What crosses this boundary: 
- Authentication method: 


Trust Boundary 2: API Gateway ←→ Backend Services
- Trust Level Changes From: 
- Trust Level Changes To: 
- What crosses this boundary: 
- Authentication method: 


Trust Boundary 3: Backend Services ←→ Database
- Trust Level Changes From: 
- Trust Level Changes To: 
- What crosses this boundary: 
- Authentication method: 


Trust Boundary 4: PayFlow ←→ External APIs (Plaid, Stripe)
- Trust Level Changes From: 
- Trust Level Changes To: 
- What crosses this boundary: 
- Authentication method: 


Trust Boundary 5: [Add more as you identify them]





```

### TODO 4: Identify Data Stores
List where sensitive data is stored and its protection level:

**Your Answer:**
```
Data Store 1:
- Location: PostgreSQL - User Table
- Data Stored: 
- Encryption at rest: 
- Access controls: 
- Backup location: 


Data Store 2:
- Location: Redis Cache
- Data Stored: 
- Encryption at rest: 
- Access controls: 
- Backup location: 


Data Store 3:
- Location: 
- Data Stored: 
- Encryption at rest: 
- Access controls: 
- Backup location: 


[Continue for S3, logs, etc.]


```

### TODO 5: External Trust Assumptions
What are you trusting external parties to do? What could go wrong?

**Your Answer:**
```
Plaid API:
- We trust them to: 
- Risk if they're compromised: 
- Risk if they have downtime: 


Stripe:
- We trust them to: 
- Risk if they're compromised: 
- Risk if they have downtime: 


AWS Infrastructure:
- We trust them to: 
- Risk if they're compromised: 
- Risk if they have downtime: 


[Continue for other external dependencies]


```

### TODO 6: Privilege Levels
Define different privilege levels in your system:

**Your Answer:**
```
Anonymous User:
- Can access: 
- Cannot access: 


Authenticated User:
- Can access: 
- Cannot access: 


Admin User:
- Can access: 
- Cannot access: 


Service Account:
- Can access: 
- Cannot access: 


Database Admin:
- Can access: 
- Cannot access: 


```

## Key Concepts to Remember

**Trust but Verify**: Even within your system, don't trust blindly. Validate at boundaries.

**Least Privilege**: Each component should have only the minimum access needed.

**Defense in Depth**: Multiple layers of security controls protect assets.

## Reflection Questions

Before moving on, consider:
- Have you identified all sensitive data?
- Do you understand where trust changes in your system?
- Can you explain who can access what and why?
- What would an attacker want to steal or manipulate?

## Next Steps

Proceed to `03-data-flows.md` to map how data moves through these boundaries.
