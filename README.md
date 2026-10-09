# Home Credit LAP AI Voice Agent

## Project Overview

This project implements an AI voice agent for Home Credit's Loan Against Property (LAP) offering. The agent conducts preliminary customer eligibility screening through a natural voice conversation.

The offer is for a loan amount of up to ₹75 lakh, subject to preliminary eligibility checks.

## Objectives

- Verify the customer's identity before discussing the offer.
- Introduce the Loan Against Property offer.
- Collect and validate seven eligibility details.
- Handle ineligible cases politely.
- Route existing property loan and EMI-reduction enquiries to a loan-transfer specialist.
- Handle busy customers and callback requests.
- Transfer qualified leads to a senior loan expert.

## Technology

- Retell AI Voice Agent
- Large Language Model (LLM)
- Voice conversation and speech recognition
- Prompt-based conversation control
- Call termination using the `end_call` function

## Seven Eligibility Checks

1. **Property type:** Residential, commercial, or industrial property is eligible under the specified criteria. Agricultural property is ineligible.
2. **Ownership:** Sole or joint ownership.
3. **Original documents:** Original property documents must be available.
4. **Loan amount:** Maximum ₹75 lakh under this offer.
5. **Occupation and income:** Salaried or self-employed; income must be received through a bank.
6. **Market value:** Record the estimated current property market value.
7. **Loan tenure:** Between 3 and 15 years, inclusive.

## Conversation Handling

The agent is designed to:
- Verify customer identity.
- Process answers provided out of order.
- Avoid repeating questions that have already been answered.
- Handle corrections and clarify unclear responses.
- End calls after disqualification or completed qualification.
- Avoid inventing interest rates or guaranteeing loan approval.

## Testing

The voice agent was tested against the assignment's eligibility and conversation scenarios, including agricultural property, unavailable original documents, cash-based income, identity mismatch, and the normal qualification flow.

## Demo

Published Retell AI voice-agent link: https://agent.retellai.com/orb/agent_a3b36cbca006f5a4e8c4802546?token=9339305463a36d972e77f809649399fa
## Limitations

This is a preliminary screening agent. It does not approve loans, calculate a final interest rate, or guarantee eligibility for final lending.

## Author

AI Voice Agent Assignment — Home Credit Loan Against Property.
