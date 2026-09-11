# SDLC and STLC

## SDLC (Software Development Lifecycle)

- Is the entire process that guides the software team(designers, PM, developers & QA) while developing the software product

## STLC(Software Testing Lifecycle)

- is a subset process that lives inside the SDLC that specifically guides the QA. Meaning that every phase of SDLC, QA has a corresponding activity

## CHEF ANOLOGY FOR BOTH SDLC & STLC

- SDLC:  Assume am a private chef hired to make a meal, which my client wants. They provide for me a recipe which will guide me through the preparation of the meal, to the stage I'll serve the meal, that's what SDLC is in software development. Without it team might build something wrong.

- STLC: Am a junior chef being supervised by senior chef. So every step a carry out in the previous meal I was preparing, the senior must be present to ensure  everything goes accordance with the recipe and also taste the meal to ensure every spice is balanced. This is what STLC is QA is present in every phase of the SDLC to ensure everything is built meets the requirements.

## V-Model

- It implies that every testing activity corresponds with the developement activity.
   -EXAMPLE: Requirements - Acceptance Testing
             System Design - System Testing
             Architecture Design - Integration testing

## Why Automation Matters in V-Model

- In V-Model regression testing occurs alot, and QA prefers to use automated tools. Because let's assume I am required to carry out 500 regression testing, manually will take hours or even days, but automation is quick and also efficient

## What happens when QA is involved too late

- When a  QA gets invovled to late there are cases that would cost the company or team alot.
 Finding bugs at the requirements pahse costs 1 unit as to compared to finding bugs at Testing which is 10 unit costly. Since a bug might be even in the requirement phase.

- Developer team at Tala Company spent one week building a faster payment feature to make the app lightning-quick, but because they excluded QA from the design phase, they accidentally created a loophole that let users fake their repayments and trick the system into upgrading their loan limits.  And this cost the company since they lost millions, where if a customer was repaying back his loan, then clicks pay all, the app will respond fast and assume all the loan has been repaid even before checking the M-pesa and increase the loan limit, making the customer to borrow again
