# Test Cases — Home Credit LAP AI Voice Agent

## 1. Project Overview

**Project:** Home Credit Loan Against Property (LAP) AI Voice Agent  
**Platform:** Retell AI  
**Purpose:** To verify customer identity, conduct preliminary eligibility checks, identify ineligible applicants, and direct qualified customers to a senior loan expert.

## 2. Eligibility Test Cases

| Test ID | Test Scenario | Test Input | Expected Result | Status |
|---|---|---|---|---|
| TC-01 | Eligible residential property | Customer has a residential house or flat and meets all other eligibility requirements. | Agent continues the eligibility questions and provides the senior-expert handoff after all seven items pass. | Pass |
| TC-02 | Agricultural property | Customer confirms the property is agricultural land. | Agent explains that agricultural property is ineligible and ends the call. | Pass |
| TC-03 | Joint ownership | Customer confirms the property is jointly owned. | Agent accepts joint ownership and continues qualification. | Pass |
| TC-04 | Original documents unavailable | Customer confirms that original property documents are unavailable. | Agent explains that original documents are required and ends the call. | Pass |
| TC-05 | Loan amount above ₹75 lakh | Customer requests more than ₹75 lakh. | Agent explains the ₹75 lakh limit and asks whether the customer wants to proceed with ₹75 lakh. | Pass |
| TC-06 | Cash-based income | Customer confirms that income is received mainly in cash. | Agent explains the bank-income requirement and ends the call. | Pass |
| TC-07 | Eligible tenure | Customer requests a tenure within the range of 3–15 years. | Agent records the tenure and continues qualification. | Pass |

## 3. Additional Functional Checks

| Test ID | Test Scenario | Expected Result | Status |
|---|---|---|---|
| TC-08 | Customer identity mismatch | Agent politely ends the conversation without continuing qualification. | Tested |
| TC-09 | Customer is busy | Agent asks for a preferred callback time and closes the conversation. | Pending verification |
| TC-10 | Existing property loan or EMI reduction | Agent directs the customer to a loan-transfer specialist and ends the call. | Pending verification |
| TC-11 | Unclear speech or unexpected response | Agent asks for clarification instead of immediately rejecting the customer. | Needs improvement |
| TC-12 | Successful qualification | Agent confirms completion of preliminary eligibility and directs the customer to a senior loan expert. | Pass |
| TC-13 | Call termination | Agent invokes the end-call function after a terminal outcome. | Verify in recording |
| TC-14 | Greeting and identity verification | Agent asks to speak with the named customer before introducing the offer. | Needs final verification |

## 4. Eligibility Rules Verified

- Maximum loan amount under this offer: ₹75 lakh.
- Eligible property types: residential, commercial, and industrial.
- Agricultural property is ineligible.
- Sole and joint ownership are eligible.
- Original property documents must be available.
- Eligible occupations: salaried and self-employed.
- Income must be received through a bank, not mainly in cash.
- Eligible loan tenure: 3–15 years, inclusive.
- No minimum property market value is specified in the assignment.
- Final approval and exact interest rates are determined by the senior loan expert.

## 5. Test Environment

- **Voice agent platform:** Retell AI
- **Agent type:** Single-prompt voice agent
- **Testing method:** Retell Test Audio
- **Knowledge base:** Not required for the core eligibility rules documented above.

## 6. Known Limitations

- Voice transcription may occasionally misinterpret spoken words, particularly property types.
- Test Audio results can depend on microphone quality, background noise, and speech recognition.
- The agent should clarify unclear responses before making an eligibility decision.
- A closing statement alone does not guarantee that the call has ended; the end-call function must be invoked.

## 7. Conclusion

The main eligibility scenarios have been tested in Retell AI. Additional checks should be completed for callback handling, loan-transfer routing, reliable call termination, and identity verification. Results should be updated after each test is confirmed.
