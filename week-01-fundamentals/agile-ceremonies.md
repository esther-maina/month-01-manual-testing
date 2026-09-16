# AGILE AND AGILE CEREMONIES

1. What is Agile? It is an SDLC model where a software product is broken down into small features or chunks, and the team works/builds each feature at a time within sprints.

Sprints: It is a short and fixed time during which the agile team builds a specific feature of the software. It usually lasts a maximum of 2 weeks.

- Agile Ceremonies: These are structured meetings that happen within the sprint.

Steps taken for Agile ceremonies.

1. Sprint Planning: PM provides the requirements for the feature that will be built in this sprint. QA and the team commit to what they can complete within the sprint and estimate the time.
2. Daily Standups: The team synchronizes together daily and asks questions like: What did I do yesterday? What am I focusing on today? and Is there anything blocking me?
3. Sprint Review: The feature demo that was built is presented before the stakeholders. Here, QA just makes final touches on the demo to ensure it does not break.
4. Sprint Retrospective: The team asks questions like: What went wrong? What went well? Is there anything to change in the next sprint?
5. Backlog Refinement: PM and the team clarify and review the requirements provided for the next feature before the next sprint starts. Here, QA reads all the requirements to find unclear or untestable items. This is the stage where QA is most required, since bugs can be caught early, which is cheaper than finding them in production, where the cost is 100 times higher.

## QUESTION: Explain what Agile ceremonies are like, as if you are explaining to a junior or non-tech person

- Answer: Agile ceremonies are like structured events that happen in each sprint. What do I mean? Example: you want to cook a meal. First, you gather all the ingredients and tools like a sufuria. Next, you prepare the ingredients and follow the steps to cook, then serve the meal. These steps, from gathering ingredients to serving the meal, are what we refer to as ceremonies in Agile.

## Definition of Done(DoD)

- It is a checklist that a team agrees before starting a sprint.

- Example of a DoD
  ✅ Each member understands the feature they are building
  ✅ Code is pushed to GitHub daily
  ✅ Feature has been tested by someone who did not build it
  ✅ No known bugs before integration
  ✅ All features are integrated and working together
  ✅ Group has reviewed the final product together before presentation.

1. Why "done" without a DoD means nothing: A developer might say, "I am done," but QA says they have not tested it yet, or PM says they have not approved it yet. This means that if the team has not agreed on the definition of done, the product cannot proceed to the next step if it is shipping.

## WHAT SPRINT FEELS LIKE?

- Day 1 — Monday
  Sprint planning. Long meeting. Everyone is optimistic.
  QA reads every user story and asks "how do we test this?"
  Some stories are unclear. QA flags them. PM rewrites them.
  Some stories are too big. Team splits them. Sprint starts.

Day 2-3 — Developers start coding
QA is writing test cases. Not waiting.
QA is setting up test data — fake accounts, test transactions.
QA finds a story that has no acceptance criteria. Flags it now.

Day 4-5 — First features land in staging
QA starts testing immediately. Does not wait for everything.
First bugs found. Logged in Jira. Assigned to developer.
Developer fixes. QA retests. Some pass. Some fail again.

Day 6 — Wednesday, mid-sprint
Backlog refinement. Team looks at next sprint's stories.
QA reads them and flags unclear requirements for next sprint.
Meanwhile testing continues on current sprint.

Day 7-8 — Reality hits
Some features are delayed. Developer underestimated the work.
QA communicates impact — "if this isn't ready by Day 10,
we cannot test it properly before the review."
PM makes a call — descope or crunch.

Day 9-10 — Final testing window
QA executes all remaining test cases.
Regression testing — does the new feature break old features?
All critical bugs must be fixed by end of Day 10.

Day 11 — Buffer day
Fix any last blockers. Stabilise the build.
QA does a final smoke test — quick check nothing exploded.

Day 12 — Sprint Review
Demo to stakeholders. QA confirmed it works. PM presents.
Stakeholders give feedback. New items added to backlog.

Day 13 — Sprint Retrospective
What went well? What went wrong? What changes next sprint?
Honest conversation. No blame. Just improvement.

Day 14 — Rest or next sprint planning begins

- The two most dangerous moments for a QA to go silent and why?

1. Sprint Planning: Because bugs found in this stage won't be flagged early and will surface later in development, making them more costly than in the requirement phase.
2. Day 7-8: Reality phase: When QA goes quiet and doesn't flag the timeline risk, by Day 11 when a feature arrives, QA has only one day to test, and in a hurry some bugs may not be flagged, which may lead to broken features when presenting to stakeholders.

- What QA is doing while developers are coding?
  - QA writes test cases alongside developers.
  - Flags if a user story has no acceptance criteria.

What separates junior QA and mid-level QA? A mid-level QA will speak up in both critical instances—during sprint planning and during the Day 7-8 reality check—because they will flag anything that could cause the feature to break.
