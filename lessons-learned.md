# Lessons Learned

## Auth Service vs API Gateway

**Question:** Do you still need an Auth Service even with an API Gateway?

**Answer:** Yes, they serve different purposes:

### API Gateway's Role
- Validates incoming requests
- Enforces rate limiting
- Routes requests to backend services
- Acts as a security perimeter

### Auth Service's Role
- Issues and manages tokens (JWT)
- Handles user registration/login logic
- Manages MFA workflows
- Maintains session state
- Validates credentials against stored data

### Key Difference
The API Gateway typically does **stateless token validation** (checking if a JWT is valid/not expired), while the Auth Service does **stateful authentication** (verifying credentials, issuing new tokens, handling MFA challenges).

### In Practice
1. User logs in → **Auth Service** verifies username/password, returns JWT
2. User makes request with JWT → **API Gateway** validates token signature/expiry
3. If token invalid → request rejected at gateway
4. If token valid → routed to backend service

### Analogy
- **API Gateway** = Security checkpoint (checks your boarding pass is real)
- **Auth Service** = Ticket counter (issues the boarding pass in the first place)

### Architecture Benefit
Separating concerns makes the system more scalable and maintainable, though you could theoretically combine them.
