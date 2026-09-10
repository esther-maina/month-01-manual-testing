# week 1 - QA Fundamentals

## What is Testing

Testing is a corrective and execution-focused process used to identify bugs
and evaluate the software work product.

## Necessity of Testing

1. The real value of testing is making a release decision with confidence.
   Finding bugs is the mechanism; the goal is informed decision-making.

2. Why do bugs cost more later? Because:
   - At the requirements stage, the change is just a requirement update.
   - At the development stage, it means rewriting code.
   - At production stage, it can cause emergency patches, customer refunds,
     reputational damage, and regulatory fines.

3. It ensures the software product works as expected and meets user and
   stakeholder needs in its operational environment.

4. It ensures the software product complies with regulatory standards.

## What is QA

QA is a planned, process-focused approach to improve the overall process and
prevent defects before, during, and after software development.

## Testing vs Debugging

- Testing: executing the software to find defects.
- Debugging: analyzing the root cause of the bug and fixing it.

## Prevention vs Detection

- Prevention: identifying defects before code is written, such as
  requirements review, design review, and static testing.
- Detection: finding bugs by executing the software.

NOTE: Prevention is always cheaper.

## The 1-10-100 Rule

1. Fix at the requirement stage: costs 1 unit
2. Fix at the testing stage: costs 10 units
3. Fix at production stage: costs 100 units

## Question

A bank releases a mobile app update. The update has a bug that charges
customers twice for transactions. It was not caught in testing. Walk me
through what the cost of that bug looks like — to the bank, the customers,
and the QA team that missed it.

## Answer based on each stage

**To the bank:**

- Reverse all duplicate transactions (operational cost)
- Customer service surge to handle complaints
- CBK regulatory scrutiny and potential fines
- Legal claims from affected customers
- Reputational damage and customer churn to competitors

**To the customer:**

- Money missing from their account
- Loss of trust in the institution
- Time spent resolving the issue

**To the QA team:**

- The failure was not in test execution.
- It was in test design — nobody asked:
  "What happens if this request is sent twice?"
- That question should have been asked at the requirements stage, not after
  release.

## What surprised me today

I was surprised by the 1-10-100 rule. It shows that the cost of fixing a
bug increases at each stage, and production is the most expensive.

I also wondered about the purpose of QA, since developers and project leads
can test too. I learned that QA brings a different mindset: developers and
product leads often test the happy path, while QA explores failure paths to
find defects.

Dynamic: executing the software product to find bugs using different testing
approaches and techniques.

Static: finding bugs without running the software, mostly before product
development begins. Examples include requirements review, code review, design
review, and static analysis.

## Static vs Dynamic Testing

**Dynamic:** Execute the software to find bugs.
Uses testing techniques and approaches against running code.

**Static:** Find bugs without running the software.
Reviews happen before or during development — requirements,
design, code review, static analysis tools.

**Why static is underrated:**

- No visible output — no dashboard, no pass/fail report
- Requires thinking, not just tool execution
- Catches the most expensive bugs earliest
- Some code paths can never be reached by running the software
  (dead code paths) — only code review finds these
- Teams under deadline pressure always skip it and always
  regret it later

**Key insight:**
The bugs static testing catches are requirement ambiguities
and design flaws. At that stage, fixing costs almost nothing.
The same bug in production costs 100x more.

## What is the difference between severity  and priority when logging defect?

## Answer

Severity is how much the bug impacts the software. Priority is how urgently it needs to be fixed. A cosmetic bug on the login page might be low severity but high priority because everyone sees it.
