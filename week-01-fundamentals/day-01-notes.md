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

Testing: Executing the software to find defects that may trigger.

Debugging: We analyze, examine the root cause of the bug and solving the bug.

## Prevention vs Detection

Prevention: Is finding or identifying the bug before code is written.(Reviewing requirements documents, design review and static testing)

Detection: Finding bugs by executing the software.

NOTE: Prevention is always cheaper.

## The 1-10-100 Rule

1. Fix at the requirement stage: costs 1 unit
2. Fix at the Testing stage: costs 10 units
3. Fix at production stage: Costs 100 units

## Quation

A bank releases a mobile app update. The update has a bug that charges customers twice for transactions. It was not caught in testing. Walk me through what the cost of that bug looks like — to the bank, to the customers, and to the QA team that missed it.

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

- The failure was not in test execution
- It was in test DESIGN — nobody asked
  "what happens if this request is sent twice?"
- That question should have been asked at
  requirements stage, not after release

## What suprised me today

Is the 1-10-100 rule, I was suprised to learn that the cost at each stage where the bug is found differs,means at the production stage the defect costs more expensive compared to the other two stages testing and requirement.

Also I wondering what is the purpose of QA yet we have developers and project lead who can test, but I learnt something to do with the curse of knownledge where a developer or the product lead will test the happy path to prevent anything will cause defects, based on what we know but now the QA will have negative testing breaks everything to identify or check is there in bugs.

Dynamic: Execution of software product to find the bug, uses different testing approaches and testing technique

Static: Finding bugs without running the software mostly happens before developing a product.(Requirements review, code review, design review, static analysis)
