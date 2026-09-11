# SDLC and STLC

## SDLC (Software Development Lifecycle)

- Is the entire process that guides the software team(designers, PM, developers & QA) while developing the software product

## STLC(Software Testing Lifecycle)

- is a subset process that lives inside the SDLC that specifically guides the QA. Meaning that every phase of SDLC, QA has a corresponding activity

## CHEF ANALOGY FOR BOTH SDLC & STLC

- SDLC: Assume am a private chef hired to make a meal, which my client wants. They provide for me a recipe which will guide me through the preparation of the meal, to the stage I'll serve the meal, that's what SDLC is in software development. Without it team might build something wrong.

- STLC: Am a junior chef being supervised by senior chef. So every step a carry out in the previous meal I was preparing, the senior must be present to ensure everything goes accordance with the recipe and also taste the meal to ensure every spice is balanced. This is what STLC is QA is present in every phase of the SDLC to ensure everything is built meets the requirements.

## V-Model

- It implies that every testing activity corresponds with the development activity.
  -EXAMPLE: Requirements - Acceptance Testing
  System Design - System Testing
  Architecture Design - Integration testing

## Why Automation Matters in V-Model

- In V-Model regression testing occurs a lot, and QA prefers to use automated tools. Because let's assume I am required to carry out 500 regression testing, manually will take hours or even days, but automation is quick and also efficient

## What happens when QA is involved too late

- When a QA gets involved too late there are cases that would cost the company or team a lot.
  Finding bugs at the requirements phase costs 1 unit as to compared to finding bugs at Testing which is 10 unit costly. Since a bug might be even in the requirement phase.

- Developer team at Tala Company spent one week building a faster payment feature to make the app lightning-quick, but because they excluded QA from the design phase, they accidentally created a loophole that let users fake their repayments and trick the system into upgrading their loan limits. And this cost the company since they lost millions, where if a customer was repaying back his loan, then clicks pay all, the app will respond fast and assume all the loan has been repaid even before checking the M-pesa and increase the loan limit, making the customer to borrow again

## SOFTWARE TESTING LIFECYCLE(STLC)

- IS a subset process that guides QA on what activity to be carried out at every development phase. It lives inside SDLC process.

- STLC has six phases:
  1. Requirement Analysis: QA reads specifications (specs) and looks for unclear or ambiguous statements, example if the specifications documents says, the app should respond quickly, QA can ask what does it mean by quickly is it 1 sec, 2 sec, 1 minute. Also QA can ask what is testable?
  2. Test Planning: QA decides: What will be tested, How it will be tested, the time will take, tools to be used and with what risks
  3. Test case design: QA writes test cases before development completes/ done
  4. Test Environment setup: QA makes sure the system is ready to be tested example right database, right config
  5. Test Execution: QA runs tests, logs the bugs and retests fixes
  6. Test closure: QA documents what was tested, what was found, what was skipped and why

## Question

- What do you think happens to STLC in a company running Agile sprints? Does this 6-phase sequence still happen or does Agile break it?

## Answer

Yes, in Agile all six phases of STLC happen, but they get time-boxed and parallelised to fit inside a sprint. Every phase still exists, but they run faster and sometimes simultaneously.

## GATE Question for STLC

- You are a QA engineer at a fintech company. A new sprint starts on Monday. The feature is: "Users can now schedule a loan repayment for a future date". Walk me through what YOU would do in each STLC phase for this feature. Be specific: what exactly are you doing, and when?

## ANSWER

- On Monday I would read the specs and find what is testable and ambiguous or unclear. The same day I would decide the tools, timeframe, how and what to test, along with the risks.
- On Tuesday: when the developer codes, I would be writing test cases alongside while making sure that the feature is ready to be tested (here, the test environment setup is running in the background).
- On Wednesday, assuming the developer has finished developing the feature, I would test, log the bugs, and report them if they are present. The developer fixes them, and then I retest the fixes.
  On Thursday, I would document everything I have tested in summary, what was skipped and the reasons why also what was found during testing.

- Worth Noting: In real sprint developers are late or they take time before they complete developing, so instead of waiting as a good QA, use that extra time to sharpen the test cases, prepare test data or even test other tickets. Remember this: You should never sit and wait.

## Explain what is STLC like you are explaining to a junior who have never worked with QA before

- Assume I have two boxes here, Box A and Box B. Box B is inside Box A, and only certain individuals are allowed to open Box B. So, let us assume Box A has layers. When one layer of Box A is opened, Box B will tell the individual what corresponding activity is supposed to be carried out. Whenever every layer of Box A is opened, that is what I mean: STLC (Box B) lives inside SDLC (Box A), so it is not a separate process. Remember this. This is displayed clearly in the V-Model or Agile. However, in Agile, it might seem like the STLC phases are all present at once. You must know they are present because they are time-boxed and parallelised into one sprint, and they happen faster and sometimes simultaneously.
