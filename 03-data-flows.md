# 03 - Data Flows

## Objective
Map how data moves through PayFlow. Data flow diagrams help identify where data is vulnerable as it crosses trust boundaries.

## Why Data Flows Matter

Threats often occur during data transit:
- When data crosses trust boundaries
- When data format changes (serialization/deserialization)
- When data is transformed or validated
- When data moves between security contexts

## TODO: Map Critical Data Flows

### TODO 1: User Registration Flow
Trace the complete flow when a new user registers:

**Your Answer:**
```
Step 1: User enters information
- Where: 
- Data: 
- Validation: 
- Trust boundary crossed: 

Step 2: 
- Where: 
- Data: 
- Processing: 
- Trust boundary crossed: 

Step 3:
- Where: 
- Data: 
- Processing: 
- Trust boundary crossed: 

[Continue until user is fully registered]




Security questions to consider:
- Where is password hashed? 
- How is email verified? 
- What happens to failed registrations? 
```

### TODO 2: Login/Authentication Flow
Map the authentication process:

**Your Answer:**
```
Step 1: User submits credentials
- Where: 
- Data transmitted: 
- Transport security: 
- Trust boundary: 

Step 2: Credential verification
- Where: 
- How validated: 
- Password storage format: 
- Failed attempt handling: 

Step 3: Session creation
- Where: 
- Session data: 
- Storage location: 
- Expiration: 

Step 4: Token issuance
- Token type: 
- Contents: 
- Signing method: 
- Lifetime: 

[Add MFA steps if applicable]




Security questions:
- Can credentials be intercepted? 
- How are sessions invalidated? 
- What rate limiting exists? 
```

### TODO 3: Payment Initiation Flow
Trace a payment from initiation to completion:

**Your Answer:**
```
Step 1: User initiates payment
- Where: 
- Data input: 
- Client-side validation: 

Step 2: Request reaches backend
- Entry point: 
- Authentication check: 
- Authorization check: 

Step 3: Payment validation
- Service: 
- Checks performed:
  - 
  - 
  - 
- Data retrieved: 

Step 4: Balance/fraud checks
- Where: 
- What's checked: 
- What happens if fails: 

Step 5: External payment processing
- Provider: 
- Data sent: 
- Data received: 
- How secured: 

Step 6: Ledger recording
- Service: 
- Records created: 
- Transaction guarantees: 

Step 7: Notifications
- Methods: 
- What info included: 
- Delivery confirmation: 

Step 8: UI update
- How user sees confirmation: 
- What details shown: 


Security questions:
- Can amounts be manipulated? 
- What if payment fails midway? 
- How is double-spending prevented? 
- Can user see others' transactions? 
```

### TODO 4: Bank Account Linking Flow
Map how users link their bank accounts:

**Your Answer:**
```
Step 1: User initiates bank linking
- UI component: 
- What triggers Plaid: 

Step 2: Plaid authentication
- Where does auth happen: 
- What data is shared: 
- How is it secured: 

Step 3: Account verification
- Who verifies: 
- What's verified: 
- Where stored: 

Step 4: Microdeposit verification (if used)
- Process: 
- Timing: 
- Failure handling: 

Step 5: Account activation
- Final checks: 
- Data stored in PayFlow: 
- Access tokens stored: 


Security questions:
- Can attacker link someone else's bank account? 
- What prevents account number tampering? 
- How long are Plaid tokens valid? 
- Can linked accounts be changed? 
```

### TODO 5: Data at Rest Flow
Describe how data moves into storage:

**Your Answer:**
```
User Profile Data:
- Created when: 
- Flows through: 
- Stored in: 
- Encryption: 
- Backup process: 

Transaction Records:
- Created when: 
- Flows through: 
- Stored in: 
- Encryption: 
- Retention period: 

Authentication Credentials:
- Created when: 
- Hashing algorithm: 
- Salt strategy: 
- Stored where: 

Session Data:
- Created when: 
- Stored where: 
- TTL: 
- Cleanup process: 

Audit Logs:
- What's logged: 
- Stored where: 
- Retention: 
- Who can access: 
```

### TODO 6: Admin Operations Flow
Map how admins perform sensitive operations:

**Your Answer:**
```
Admin Authentication:
- How admins log in: 
- Additional verification: 
- Access granted to: 

User Account Management:
- Actions allowed:
  - 
  - 
- Audit trail: 
- Approval process: 

Transaction Investigation:
- What data accessible: 
- Audit trail: 
- PII access restrictions: 

System Configuration:
- What can be changed: 
- Change approval: 
- Rollback capability: 


Security questions:
- Can admin access be abused? 
- How are admin actions logged? 
- Can admins modify their own audit logs? 
```

## Data Flow Diagram Exercise

### TODO 7: Create a DFD
Draw a simple data flow diagram for the payment flow. Use this notation:
- [Entity] = External entity (user, system)
- (Process) = Process/service
- [Data Store] = Database/storage
- → = Data flow with label

**Your Answer:**
```
[Create your diagram here - can be ASCII art or describe it]

Example format:
[User] --amount, recipient--> (API Gateway) --validated data--> (Payment Service)








```

## Common Data Flow Vulnerabilities

As you review your flows, watch for:
- Unencrypted sensitive data in transit
- Data crossing trust boundaries without validation
- Sensitive data in logs or error messages
- Data accessible by unauthorized services
- Missing or weak input validation
- Improper error handling that leaks information

### TODO 8: Vulnerability Spotting
Review each flow you mapped. List potential vulnerabilities:

**Your Answer:**
```
Registration Flow Vulnerabilities:
1. 
2. 
3. 

Login Flow Vulnerabilities:
1. 
2. 
3. 

Payment Flow Vulnerabilities:
1. 
2. 
3. 

[Continue for other flows]


```

## Reflection Questions

- Do you understand how money moves through the system?
- Can you identify where sensitive data is most vulnerable?
- Do you see any flows that lack proper validation?
- Are there any unnecessary data exposures?

## Next Steps

Proceed to `04-threat-identification.md` to systematically identify threats using STRIDE.
