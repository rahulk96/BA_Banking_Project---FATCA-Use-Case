# BA_Banking_Project-FATCA_Use_Case
# FATCA Declaration – Internet Banking

## Project Overview

This project demonstrates a Business Analyst solution for enhancing an existing retail bank's Internet Banking facility to support FATCA self-declaration.

The enhancement enables customers to:

- View their FATCA declaration status
- Complete and submit the FATCA self-declaration
- Postpone the declaration for up to 6 months after rollout, where applicable
- Continue using Internet Banking after postponement
- Be redirected to the FATCA submission journey when the declaration remains pending

## Business Scenario

The bank has received a requirement to introduce FATCA declaration and relevant information submission into its existing Internet Banking facility.

The customer is required to complete the FATCA declaration when the declaration is pending. If the six-month postponement window is still open, the customer can postpone the declaration and continue using Internet Banking.

## Key Use Cases

1. **Check FATCA Status and Display FATCA Page**
   - Check the customer's FATCA status during login
   - Display the FATCA page when the status is pending
   - Route submitted customers directly to the Internet Banking dashboard

2. **Submit FATCA Declaration**
   - Capture country of birth
   - Capture citizenship and past citizenship
   - Capture tax residency and TIN
   - Capture US tax liability
   - Capture US TIN where applicable
   - Capture customer self-declaration
   - Validate and submit the declaration

3. **Postpone FATCA Declaration**
   - Allow postponement within the six-month window
   - Display a confirmation popup
   - Record the postponement
   - Keep the FATCA status as pending
   - Display the FATCA journey again on the next login

## Actors

| Actor/System | Role |
|---|---|
| Customer | Provides FATCA information, submits or postpones the declaration |
| Internet Banking System | Authenticates the customer and manages the FATCA journey |
| Core Banking System | Provides FATCA status and receives the updated submitted status |

## Deliverables

This repository contains:

- Use Case Document
- Use Case Diagram
- PlantUML source code
- FATCA Wireframes
- Traceability Matrix

## Repository Structure

```text
FATCA-Declaration-Internet-Banking/
│
├── README.md
│
├── Documentation/
│   └── FATCA_Use_Case_Document.pdf
│
├── Wireframes/
│   ├── Wireframe-01-Login.png
│   ├── Wireframe-02-FATCA-Declaration.png
│   ├── Wireframe-03-Expired-Postponement.png
│   ├── Wireframe-04-Validation-Errors.png
│   ├── Wireframe-05-Declaration-Submitted.png
│   └── Wireframe-06-Postpone-Confirmation.png
│
└── Use-Case-Diagram/
    ├── FATCA-Use-Case-Diagram.png
    └── FATCA-Use-Case-Diagram.puml



Project Task - 

Assume that you are a business analyst working in IT department of a leading retail bank in India.
Your team has received a mandate to include FATCA declaration and relevant information submission form into existing internet banking facility.
The users should land on FATCA submission page every time they use net banking facility.
The user can postpone the FATCA declaration submission for up to 6 months after the functionality is rolled out.
Create a Use Case diagram for this functionality.
