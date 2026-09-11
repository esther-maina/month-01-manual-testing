# SDLC and STLC

## SDLC (Software Development Lifecycle)

- Is the entire process that guides the software team(designers, PM, developers & QA) while developing the software product

## STLC(Software Testing Lifecycle)

- is a subset process that lives inside the SDLC that specifically guides the QA. Meaning that every phase of SDLC, QA has a corresponding activity

## CHEF ANALOGY FOR BOTH SDLC & STLC

- SDLC: Assume I am a private chef hired to make a meal, which my client wants. They provide for me a recipe which will guide me through the preparation of the meal, to the stage I'll serve the meal, th[...]

- STLC: I am a junior chef being supervised by senior chef. So every step I carry out in the previous meal I was preparing, the senior must be present to ensure everything goes in accordance with the recip[...]

## V-Model

- It implies that every testing activity corresponds with the development activity.
  - EXAMPLE: Requirements - Acceptance Testing
  System Design - System Testing
  Architecture Design - Integration testing

## Why Automation Matters in V-Model

- In V-Model regression testing occurs a lot, and QA prefers to use automated tools. Because let's assume I am required to carry out 500 regression tests, manually will take hours or even days, but [...]

## What happens when QA is involved too late

- When a QA gets involved too late there are cases that would cost the company or team a lot.
  Finding bugs at the requirements phase costs 1 unit as compared to finding bugs at Testing which is 10 units costly. Since a bug might be even in the requirement phase.

- Developer team at Tala Company spent one week building a faster payment feature to make the app lightning-quick, but because they excluded QA from the design phase, they accidentally created a loophol[...]

## SOFTWARE TESTING LIFECYCLE(STLC)

- IS a subset process that guides QA on what activity to be carried out at every development phase. It lives inside SDLC process.

- STLC has six phases:
  1. Requirement Analysis: QA reads specifications (specs) and looks for unclear or ambiguous statements, example if the specifications document says, the app should respond quickly, QA can ask what [...]
  2. Test Planning: QA decides: What will be tested, How it will be tested, the time it will take, tools to be used and what risks
  3. Test case design: QA writes test cases before development completes/ is done
  4. Test Environment setup: QA makes sure the system is ready to be tested example right database, right config
  5. Test Execution: QA runs tests, logs the bugs and retests fixes
  6. Test closure: QA documents what was tested, what was found, what was skipped and why

## Question

- What do you think happens to STLC in a company running Agile sprints? Does this 6-phase sequence still happen or does Agile break it?

## Answer

Yes, in Agile all six phases of STLC happen, but they get time-boxed and parallelised to fit inside a sprint. Every phase still exists, but they run faster and sometimes simultaneously.

## GATE Question for STLC

- You are a QA engineer at a fintech company. A new sprint starts on Monday. The feature is: "Users can now schedule a loan repayment for a future date". Walk me through what YOU would do in each STLC[...]

## ANSWER

- On Monday I would read the specs and find what is testable and ambiguous or unclear. The same day I would decide the tools, timeframe, how and what to test, along with the risks.
- On Tuesday: when the developer codes, I would be writing test cases alongside while making sure that the feature is ready to be tested (here, the test environment setup is running in the backgro[...]
- On Wednesday, assuming the developer has finished developing the feature, I would test, log the bugs, and report them if they are present. The developer fixes them, and then I retest the fixes.
  On Thursday, I would document everything I have tested in summary, what was skipped and the reasons why also what was found during testing.

- Worth Noting: In real sprint developers are late or they take time before they complete developing, so instead of waiting as a good QA, use that extra time to sharpen the test cases, prepare test da[...]

## Explain what is STLC like you are explaining to a junior who have never worked with QA before

- Assume I have two boxes here, Box A and Box B. Box B is inside Box A, and only certain individuals are allowed to open Box B. So, let us assume Box A has layers. When one layer of Box A is opened, B[...]
