# Mortgage Calculator

A simple mortgage calculator widget that takes in a loan amount, interest rate, loan term, and calculates the monthly mortgage payment, total payment amount, and total interest paid.

## Requirements

### User Inputs
- **Loan amount ($)**: Enter the loan amount.
- **Annual interest rate (%)**: Also known as the Annual Percentage Rate (APR).
- **Loan term (in years)**: Enter the term of the loan in years.

### Outputs
The calculator should compute and display the following:
- **Monthly mortgage payment**: The monthly payment amount.
- **Total payment amount**: Total payment over the term of the loan.
- **Total interest paid**: Total interest paid over the term of the loan.

### Additional Requirements
- If a non-numerical value is entered into any input field, an error message should be displayed.
- Handle any other invalid input cases appropriately.
- Round all calculated results to **2 decimal places**.

> Note: The last two requirements might not be explicitly given during interviews, but you are expected to ask for clarification.

### Formula for Monthly Payment

The monthly mortgage payment is calculated using the formula:
- `**M = P(i(1+i)n)/((1+i)n - 1)**`

- **M**: Monthly mortgage payment
- **P**: Loan amount
- **i**: Monthly interest rate (APR / 12)
- **n**: Total number of payments (loan term in years x 12)

