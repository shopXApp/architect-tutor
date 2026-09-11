# ROLE

Act as a **Senior Technical Architect, Solution Architect, Principal Engineer, Technical Interviewer, and Interview Panel Lead** with extensive experience conducting senior-level software engineering interviews.

Your task is to create a **single, self-contained HTML interview assessment document** designed to conduct a **minimum 3-hour comprehensive technical interview**.

The candidate has approximately **12+ years of software development experience**, primarily in:

* C#
* .NET / ASP.NET Core
* REST APIs
* SQL Server
* JavaScript
* Microservices
* Redis
* RabbitMQ / messaging
* Background processing
* Cloud
* System design
* Software architecture
* Technical leadership

The interview must evaluate whether the candidate is genuinely ready for:

**Senior Software Engineer → Technical Lead → Technical Architect / Solution Architect**

Do NOT assume the candidate is Architect-ready.

The interview must identify the actual level based on evidence from answers.

---

# PRIMARY OBJECTIVE

Generate a **comprehensive interview guide and assessment system** capable of running for **at least 3 hours**.

The HTML must contain:

* Questions
* Follow-up questions
* Expected discussion areas
* Practical scenarios
* Coding exercises
* System design exercises
* Debugging exercises
* Architecture challenges
* Behavioral questions
* Leadership questions
* Evaluation criteria
* Scoring system
* Interviewer notes
* Final recommendation

The interviewer should be able to use the HTML directly during a live interview.

Do not create a simple question bank.

Create a **complete interview process**.

---

# IMPORTANT INTERVIEW RULE

The interviewer must NOT immediately show the candidate:

* Model answers
* Expected answers
* Evaluation notes
* Scoring guidance

Keep interviewer guidance visually separated or collapsible using HTML `<details>` and `<summary>`.

For example:

```html
<details>
    <summary>Interviewer Evaluation Guide</summary>
    ...
</details>
```

This allows the interviewer to reveal evaluation guidance only after the candidate answers.

---

# INTERVIEW DURATION

Design the interview for a minimum of **180 minutes**.

Target approximately:

| Section                 | Target Time |
| ----------------------- | ----------: |
| Introduction            |      10 min |
| Core Computer Science   |      20 min |
| C# / .NET               |      25 min |
| Database                |      20 min |
| OS Fundamentals         |      10 min |
| Networking              |      15 min |
| Coding                  |      25 min |
| Debugging               |      15 min |
| Testing                 |      10 min |
| Practical Engineering   |      10 min |
| System Design           |      25 min |
| Architecture            |      20 min |
| Leadership / Behavioral |      15 min |
| Final Discussion        |       5 min |
| **Total**               | **225 min** |

The interview should therefore support approximately **3 to 3.75 hours**.

The interviewer can shorten sections if required.

---

# HTML REQUIREMENTS

Generate exactly **ONE complete HTML file**.

The HTML must:

* Start with `<!DOCTYPE html>`
* Include `<html>`
* Include `<head>`
* Include `<meta charset="UTF-8">`
* Include a useful `<title>`
* Include `<style>`
* Include `<body>`
* Contain all content inside the HTML
* Require NO external CSS
* Require NO external JavaScript
* Require NO external libraries
* Work offline
* Be readable on desktop and mobile
* Use semantic HTML
* Use clear headings
* Use tables where appropriate
* Use `<code>` for code
* Use `<pre>` for larger code examples
* Use `<details>` for interviewer-only guidance

Add simple JavaScript only if useful for:

* Score calculation
* Timer
* Progress tracking
* Section navigation
* Expand/collapse controls

Do not make the HTML dependent on external resources.

---

# SECTION 1: INTERVIEW DASHBOARD

Create a professional dashboard at the top.

Include:

* Candidate name field
* Interviewer name field
* Date field
* Current role
* Target role
* Years of experience
* Interview start time
* Interview status

Include a section progress indicator.

Example:

```text
Overall Progress
[████████░░░░░░░░] 45%
```

Create buttons for:

* Start Interview
* Reset Interview
* Expand All
* Collapse All

If JavaScript is used, keep it simple and embedded inside the HTML.

---

# SECTION 2: INTERVIEWER INSTRUCTIONS

Explain:

## How to Conduct This Interview

The interviewer should:

1. Ask the primary question.
2. Allow the candidate to think.
3. Ask follow-up questions.
4. Challenge assumptions.
5. Ask "Why?"
6. Ask for real examples.
7. Ask for trade-offs.
8. Ask what could fail.
9. Ask how success would be measured.
10. Score only after sufficient discussion.

Explain that the interviewer should not reward:

* Buzzwords
* Technology name-dropping
* Memorized definitions
* Long answers without substance
* Fake experience

Reward:

* Clear reasoning
* Correct fundamentals
* Practical experience
* Trade-off thinking
* Ownership
* Business awareness
* Production thinking
* Communication

---

# SECTION 3: INTRODUCTION AND CAREER DISCUSSION

Target: **10 minutes**

Ask:

1. Tell me about yourself.
2. Walk me through your career.
3. What are you currently responsible for?
4. What percentage of your work involves architecture?
5. What technical decisions do you personally make?
6. What is the most complex system you have worked on?
7. What was your biggest technical contribution?
8. What was your biggest mistake?
9. Why are you targeting Technical Architect / Solution Architect roles?

For each question include:

* Main question
* 2 to 4 follow-ups
* What the interviewer is testing
* Strong answer indicators
* Warning signs
* Score field

---

# SECTION 4: COMPUTER SCIENCE FUNDAMENTALS

Target: **20 minutes**

Cover:

## Data Structures

Ask about:

* Array
* List
* Dictionary / HashMap
* Stack
* Queue
* Linked List
* Tree
* Graph
* Heap
* Set

Do not only ask definitions.

Use practical questions.

Example:

> You need to find whether a user ID already exists among 10 million records. What data structure would you choose and why?

Follow up with:

> What is the lookup complexity?

> What are the memory implications?

> What happens if the data changes frequently?

---

## Algorithms

Ask about:

* Searching
* Sorting
* Binary search
* Hashing
* Recursion
* Traversal
* Graph traversal
* Common algorithmic approaches

Include at least:

**10 conceptual questions**

**5 practical scenarios**

**5 complexity questions**

---

## Complexity

Test:

* Big O
* Time complexity
* Space complexity
* Average vs worst case

Give code snippets and ask the candidate to determine complexity.

Example:

```csharp
for (int i = 0; i < n; i++)
{
    for (int j = 0; j < n; j++)
    {
        Console.WriteLine(i + j);
    }
}
```

Ask:

> What is the time complexity?

Then provide progressively harder examples.

---

# SECTION 5: C# AND .NET

Target: **25 minutes**

Go beyond syntax.

Evaluate actual senior-level knowledge.

Cover:

## C# Fundamentals

* Classes
* Structs
* Interfaces
* Abstract classes
* Generics
* Delegates
* Events
* Exceptions
* Collections
* LINQ
* Extension methods

## Object-Oriented Programming

Ask:

* SOLID
* Encapsulation
* Abstraction
* Inheritance
* Polymorphism

Do not ask only definitions.

Use practical design scenarios.

---

## Advanced C#

Cover:

* async / await
* Task
* CancellationToken
* Thread safety
* Lock
* Concurrent collections
* IDisposable
* Garbage collection
* Memory management
* Dependency Injection
* Reflection
* Records
* Nullable reference types

---

## ASP.NET Core

Ask about:

* Middleware
* Dependency Injection
* Configuration
* Logging
* Authentication
* Authorization
* Filters
* Routing
* Model binding
* API versioning
* Exception handling
* Health checks
* Background services

---

## Performance

Ask:

> An ASP.NET Core API suddenly becomes slow. How do you investigate it?

Follow up with:

* CPU
* Memory
* Database
* External API
* Thread pool
* Network
* Logging
* Distributed tracing

---

# SECTION 6: DATABASE

Target: **20 minutes**

## SQL

Cover:

* SELECT
* JOIN
* GROUP BY
* HAVING
* Subqueries
* CTE
* Window functions
* Transactions
* Isolation levels
* Indexes
* Stored procedures

Ask practical questions.

---

## Database Design

Ask the candidate to design tables for:

* Users
* Companies
* Products
* Orders
* Order items
* Payments

Test:

* Primary keys
* Foreign keys
* Indexes
* Constraints
* Normalization
* Relationships

---

## Query Optimization

Scenario:

> A query that previously took 200 ms now takes 8 seconds.

Ask:

1. What do you check?
2. Execution plan?
3. Indexes?
4. Statistics?
5. Data growth?
6. Blocking?
7. Locking?
8. Query structure?
9. Server resources?

---

## NoSQL

Ask:

* When would you use NoSQL?
* When would you avoid it?
* Document vs relational data
* Consistency
* Scaling
* Query patterns

Compare SQL and NoSQL using practical scenarios.

---

# SECTION 7: OPERATING SYSTEMS

Target: **10 minutes**

Cover:

* Process
* Thread
* Thread pool
* Context switching
* Memory
* Stack
* Heap
* Garbage collection
* Deadlock
* Race condition
* CPU utilization
* Memory pressure

Ask practical scenarios.

Example:

> An API server has high CPU but low traffic. What would you investigate?

---

# SECTION 8: NETWORKING

Target: **15 minutes**

Cover:

## TCP/IP

* IP
* TCP
* UDP
* Ports
* Connections
* Handshake
* Timeouts

## HTTP

* GET
* POST
* PUT
* PATCH
* DELETE
* Status codes
* Headers
* Cookies
* Authentication

## HTTPS

Explain:

* TLS
* Certificates
* Encryption

## DNS

Ask:

> What happens when a user enters a URL into the browser?

Expect discussion covering:

DNS
→ connection
→ TLS
→ HTTP
→ server
→ response

Ask follow-up questions at every stage.

---

# SECTION 9: CODING ASSESSMENT

Target: **25 minutes**

Create **3 coding problems**.

### Problem 1: Easy/Medium

Test:

* Collections
* Logic
* Complexity

### Problem 2: Medium

Test:

* Algorithms
* Clean code
* Edge cases

### Problem 3: Senior Level

Test:

* Design
* Concurrency OR performance
* Error handling
* Maintainability

Use C#.

For each problem provide:

* Problem statement
* Input
* Output
* Constraints
* Example
* Expected discussion
* Follow-up questions
* Hidden edge cases
* Evaluation criteria

Do NOT immediately show the solution.

Put the solution inside:

```html
<details>
    <summary>Interviewer Only: Model Solution</summary>
</details>
```

Evaluate:

* Correctness
* Complexity
* Readability
* Naming
* Structure
* Error handling
* Edge cases
* Performance
* Communication

---

# SECTION 10: CODE REVIEW

Give the candidate a deliberately poor C# code sample.

The code should contain several issues such as:

* Poor naming
* Duplicate logic
* Bad exception handling
* Inefficient LINQ
* Unnecessary database calls
* Poor async usage
* Hard-coded values
* Tight coupling

Ask:

> Review this code as a Senior Engineer / Technical Lead.

Then ask:

> What would you change first?

> Which issue is most dangerous?

> Which issue affects performance?

> Which issue affects maintainability?

> How would you refactor it?

Provide interviewer-only evaluation guidance.

---

# SECTION 11: DEBUGGING AND TROUBLESHOOTING

Target: **15 minutes**

Create realistic production incidents.

Include:

### Scenario 1

API response time increases.

### Scenario 2

Database CPU reaches 100%.

### Scenario 3

Memory keeps increasing.

### Scenario 4

RabbitMQ queue backlog grows.

### Scenario 5

Redis becomes unavailable.

### Scenario 6

Users receive duplicate operations.

For each scenario ask:

1. What do you check first?
2. What evidence do you collect?
3. What is your hypothesis?
4. How do you confirm it?
5. What immediate action do you take?
6. What permanent fix would you make?
7. How would you prevent recurrence?

Evaluate whether the candidate uses:

* Logs
* Metrics
* Traces
* Alerts
* Profiling
* Database monitoring
* Distributed tracing

---

# SECTION 12: TESTING

Target: **10 minutes**

Cover:

* Unit testing
* Integration testing
* API testing
* End-to-end testing
* Mocking
* Test doubles
* Regression testing
* Performance testing
* Security testing

Ask practical questions.

Example:

> A payment API works locally but fails in production. What testing was probably missing?

Also ask:

> What should NOT be mocked?

---

# SECTION 13: DEVELOPMENT TOOLS AND ENGINEERING PRACTICES

Evaluate familiarity with:

* Visual Studio
* VS Code
* Git
* Pull requests
* Code reviews
* CI/CD
* NuGet
* Docker
* API testing tools
* SQL tools
* Logging tools
* Monitoring tools

Do not evaluate tool knowledge as memorization.

Ask how the candidate actually uses tools to solve problems.

---

# SECTION 14: SYSTEM DESIGN

Target: **25 minutes**

Give one completely new system design problem.

Do not use famous interview examples such as:

* Netflix
* Uber
* WhatsApp
* Twitter

Create a realistic enterprise system.

The candidate must:

1. Ask clarifying questions.
2. Define functional requirements.
3. Define non-functional requirements.
4. Estimate scale.
5. Identify major components.
6. Define APIs.
7. Design database.
8. Discuss caching.
9. Discuss messaging.
10. Discuss scaling.
11. Discuss failure handling.
12. Discuss security.
13. Discuss monitoring.
14. Discuss cost.
15. Discuss trade-offs.

Do NOT provide the architecture immediately.

Challenge every major decision.

Ask:

> Why?

> Why not the alternative?

> What happens if it fails?

> How does it scale?

> What does it cost?

---

# SECTION 15: SOFTWARE ARCHITECTURE

Target: **20 minutes**

Evaluate understanding of:

## Architecture Styles

* Monolith
* Modular monolith
* Microservices
* Event-driven architecture
* Serverless
* Layered architecture
* Clean architecture

Do not ask only definitions.

Ask:

> When would you NOT choose microservices?

---

## Architecture Patterns

Cover:

* API Gateway
* CQRS
* Event sourcing
* Saga
* Circuit breaker
* Retry
* Bulkhead
* Cache-aside
* Repository
* Outbox
* Strangler migration

For each ask:

* What problem does it solve?
* What new problem does it create?
* When would you use it?
* When would you avoid it?

---

# SECTION 16: SCALABILITY, RELIABILITY AND AVAILABILITY

Ask:

> Your system works correctly for 10,000 users. The business expects 10 million. What changes?

Cover:

* Horizontal scaling
* Vertical scaling
* Load balancing
* Caching
* Database scaling
* Read replicas
* Partitioning
* Sharding
* CDN
* Async processing
* Queue-based architecture

Then ask:

> What becomes the bottleneck first?

---

# SECTION 17: API DESIGN

Evaluate:

* REST
* HTTP methods
* Status codes
* Versioning
* Pagination
* Filtering
* Sorting
* Validation
* Error response
* Idempotency
* Rate limiting
* Authentication
* Authorization

Give a poorly designed API and ask the candidate to improve it.

---

# SECTION 18: SECURITY

Evaluate:

* Authentication
* Authorization
* JWT
* OAuth
* Identity
* Secrets
* Encryption
* HTTPS
* SQL injection
* XSS
* CSRF
* Rate limiting
* Audit logging
* Tenant isolation

Use real scenarios.

Example:

> Company A can see Company B's data.

Ask:

> How would you investigate?

> How would you prevent it?

> How would you prove tenant isolation?

---

# SECTION 19: CLOUD

Ask architecture-level questions about:

* Azure
* AWS
* Containers
* Managed services
* Databases
* Storage
* Networking
* Monitoring
* Scaling
* Disaster recovery

Do NOT test memorization of cloud product names.

Test whether the candidate understands:

> What problem does the cloud service solve?

---

# SECTION 20: PRACTICAL ARCHITECTURE DECISIONS

Create at least **15 decision scenarios**.

Examples:

### Scenario 1

SQL vs NoSQL

### Scenario 2

Microservices vs Modular Monolith

### Scenario 3

Redis vs Database

### Scenario 4

RabbitMQ vs direct API call

### Scenario 5

Synchronous vs asynchronous processing

### Scenario 6

Shared database vs separate databases

### Scenario 7

Build vs buy

### Scenario 8

Single region vs multi-region

### Scenario 9

Read replica vs reporting database

### Scenario 10

Cloud vs on-premise

For each ask:

* Requirements
* Options
* Decision
* Trade-offs
* Risks
* Cost
* When to revisit

---

# SECTION 21: LEADERSHIP

Target: **10 minutes**

Ask:

* How do you mentor developers?
* How do you handle a strong developer who disagrees?
* How do you conduct architecture reviews?
* How do you maintain standards?
* How do you delegate?
* How do you handle technical debt?
* How do you handle a missed deadline?
* How do you communicate risks to management?

Evaluate:

* Leadership
* Ownership
* Communication
* Emotional maturity
* Decision making

---

# SECTION 22: BEHAVIORAL INTERVIEW

Target: **15 minutes**

Ask at least 15 questions covering:

* Biggest achievement
* Biggest failure
* Difficult stakeholder
* Conflict
* Production incident
* Wrong decision
* Mentoring
* Pressure
* Deadline
* Technical disagreement
* Business disagreement
* Learning something difficult
* Adapting to change
* Handling criticism
* Taking ownership

Use real experience.

Do not reward fake or overly perfect stories.

---

# SECTION 23: ETHICS

Ask practical ethical questions.

Examples:

> You discover a serious security vulnerability one day before release. What do you do?

> Management asks you to hide a production defect.

> A developer copies code from an unknown source.

> Customer data is accidentally exposed.

> A team member manipulates performance numbers.

Evaluate:

* Integrity
* Responsibility
* Risk awareness
* Professional judgement

---

# SECTION 24: CULTURAL FIT

Evaluate:

* Collaboration
* Ownership
* Respect
* Learning mindset
* Adaptability
* Accountability
* Communication

Avoid discriminatory or personal questions.

Focus only on workplace behavior.

---

# SECTION 25: ARCHITECTURE LEADERSHIP CHALLENGE

Create one major scenario:

> A company has a large .NET monolithic application.

Problems:

* Slow releases
* Database bottleneck
* Poor monitoring
* High deployment risk
* Increasing traffic
* Multiple teams
* High technical debt

Management says:

> "Move everything to microservices within 3 months."

Ask the candidate:

1. Would you agree?
2. What questions would you ask?
3. What would you change first?
4. Would you recommend microservices?
5. How would you reduce risk?
6. How would you plan migration?
7. How would you measure success?

Challenge the answer aggressively.

---

# SECTION 26: FINAL ARCHITECTURE DEFENSE

Tell the candidate:

> "I disagree with your architecture."

Then generate objections such as:

* Too expensive
* Too complex
* Not scalable
* Too many services
* Security risk
* Operational burden
* Too slow to deliver

Ask the candidate to defend or change the architecture.

Evaluate whether they:

* Defend blindly
* Listen
* Ask questions
* Use evidence
* Understand trade-offs
* Change their decision when appropriate

---

# SECTION 27: RAPID-FIRE ROUND

Create **30 rapid-fire questions**.

Each should be answerable within 30 to 60 seconds.

Cover:

* C#
* .NET
* SQL
* APIs
* Redis
* Messaging
* Microservices
* Architecture
* Security
* Cloud
* Scalability
* Production

Do not allow long theoretical answers.

---

# SECTION 28: FINAL SCORING

Create a detailed scoring system.

Score every major area from:

**1 to 10**

Use:

### 1 to 3

Weak

### 4 to 5

Below expected level

### 6

Acceptable

### 7

Good

### 8

Strong

### 9

Very strong

### 10

Architect-level / exceptional

Final score should be weighted.

Use:

| Category                   |   Weight |
| -------------------------- | -------: |
| C# / .NET                  |      10% |
| Computer Science           |       5% |
| Database                   |      10% |
| OS / Networking            |       5% |
| Coding                     |      10% |
| Debugging                  |      10% |
| Testing                    |       5% |
| System Design              |      15% |
| Architecture               |      15% |
| Security / Reliability     |       5% |
| Leadership                 |       5% |
| Behavioral / Communication |       5% |
| **Total**                  | **100%** |

---

# SECTION 29: CAREER LEVEL DECISION

Based on the interview, classify the candidate:

### Senior Software Engineer

### Technical Lead

### Technical Architect

### Solution Architect

### Enterprise Architect

Provide a percentage fit for each.

Example:

```text
Senior Software Engineer: 95%
Technical Lead: 90%
Technical Architect: 78%
Solution Architect: 65%
Enterprise Architect: 40%
```

Do not use arbitrary scores.

Explain the evidence behind each score.

---

# SECTION 30: FINAL VERDICT

Answer:

> Would you hire this candidate as a Technical Architect today?

Choose:

### YES

### NO

### BORDERLINE

Then explain:

1. Why
2. Strongest evidence
3. Biggest weakness
4. Biggest technical gap
5. Biggest leadership gap
6. Biggest communication gap
7. What would make you change the decision

---

# SECTION 31: TOP STRENGTHS

Identify the candidate's:

## Top 10 strengths

Only use strengths demonstrated during the interview.

---

# SECTION 32: TOP WEAKNESSES

Identify:

## Top 10 weaknesses

For every weakness provide:

* Evidence
* Impact
* Severity
* Improvement action

Prioritize:

**Critical / High / Medium / Low**

---

# SECTION 33: ARCHITECT GAP ANALYSIS

Create:

| Skill | Current Level | Architect Expected | Gap | Priority | Action |
| ----- | ------------: | -----------------: | --: | -------- | ------ |

Include:

* System design
* Architecture
* Cloud
* Security
* Scalability
* Reliability
* Database
* Distributed systems
* Leadership
* Communication
* Business thinking

---

# SECTION 34: 90-DAY IMPROVEMENT PLAN

Based ONLY on weaknesses identified during the interview.

Create:

## Month 1

Focus on biggest technical gap.

## Month 2

Focus on architecture and real-world application.

## Month 3

Focus on interviews and leadership.

For each month include:

* Weekly objectives
* Practical assignment
* Expected output
* Measurement

---

# SECTION 35: FINAL REPORT

Generate a professional report titled:

# Technical Architect Interview Assessment Report

Include:

## Candidate Profile

## Interview Duration

## Overall Score

## Technical Score

## Architecture Score

## Leadership Score

## Communication Score

## Strongest Skills

## Weakest Skills

## Architecture Readiness

## Career Level

## Hiring Recommendation

## Key Risks

## 90-Day Improvement Plan

## Final Verdict

---

# IMPORTANT: FINAL ASSESSMENT PHILOSOPHY

The interview must distinguish between:

### Knowing

The candidate can explain a concept.

### Applying

The candidate can use the concept in a real situation.

### Designing

The candidate can build a solution using the concept.

### Defending

The candidate can explain why the solution is appropriate.

### Leading

The candidate can convince others, manage trade-offs, handle disagreement, and own the outcome.

A Technical Architect must demonstrate all five.

Do not classify someone as Architect-ready simply because they know many technologies.

---

# HTML DESIGN

Create a professional interview dashboard.

Use:

* Clean typography
* Cards
* Tables
* Section numbering
* Score badges
* Progress indicators
* Expandable interviewer notes
* Question numbering
* Clearly separated candidate questions and interviewer guidance

Use a professional neutral visual style.

Do not use external fonts, images, CSS, JavaScript libraries, CDN links, or frameworks.

The final HTML must work completely offline.

---

# FINAL OUTPUT RULE

Return **ONLY the complete HTML source code**.

Do not provide:

* Markdown explanation
* Introduction outside HTML
* Explanation after the HTML
* Multiple files
* Separate CSS
* Separate JavaScript
* External resources

The output must be directly saveable as:

`technical-architect-3-hour-interview.html`

and open directly in a browser.
