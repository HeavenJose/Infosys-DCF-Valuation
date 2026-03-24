# Infosys DCF Valuation (Python)

## Overview
This project builds a complete Discounted Cash Flow (DCF) model for Infosys using Python and real financial data. The goal is to estimate the intrinsic value of the company based on its future cash generating ability.

---

## What is DCF?

Discounted Cash Flow (DCF) is a valuation method used to estimate the value of a company by projecting its future cash flows and discounting them to present value using a required rate of return (WACC).

---

## Key Concepts Explained

### Free Cash Flow (FCF)
Free Cash Flow represents the cash available to investors after the company has paid for operating expenses and capital expenditures.

**Formula used:**
FCF = Cash Flow from Operations + Capital Expenditure

---

### Forecasting
Future Free Cash Flows were projected for 5 years based on historical growth trends. Extreme fluctuations were adjusted to ensure realistic projections.

---

### Beta
Beta measures how sensitive a stock is relative to the overall market.

- Beta > 1 → More volatile than market  
- Beta < 1 → Less volatile than market  

In this project, Beta was calculated using covariance of stock and market returns.

---

### Cost of Equity (CAPM)
Cost of equity represents the return expected by equity investors.

**Formula (CAPM):**
Cost of Equity = Risk-Free Rate + Beta × (Market Return − Risk-Free Rate)

---

### Cost of Debt
Cost of debt represents the effective interest rate the company pays on its borrowings.

**Formula used:**
Cost of Debt = Interest Expense / Total Debt

---

### WACC (Weighted Average Cost of Capital)
WACC is the average rate of return required by all investors (equity + debt). It is used as the discount rate in DCF.

---

### Terminal Value
Terminal value represents the value of the company beyond the forecast period.

**Formula (Gordon Growth Model):**
Terminal Value = FCF × (1 + g) / (WACC − g)

---

### Enterprise Value
Enterprise Value is the total value of the firm based on discounted future cash flows.

---

### Equity Value
Equity Value is calculated by adjusting enterprise value for cash and debt.

**Formula:**
Equity Value = Enterprise Value + Cash − Debt

---

### Intrinsic Value per Share
This represents the estimated fair value of one share.

**Formula:**
Intrinsic Value per Share = Equity Value / Number of Shares

---

## Sensitivity Analysis
Sensitivity analysis was performed to understand how changes in:

- WACC (discount rate)
- Terminal growth rate

affect the valuation.

---

## Scenario Analysis

Three scenarios were created:

- **Bear Case**: Conservative assumptions  
- **Base Case**: Most realistic assumptions  
- **Bull Case**: Optimistic assumptions  

---

## Key Results

- Base Case Value: ₹404 per share  
- Bear Case: ₹292  
- Bull Case: ₹566  

---

## Tools Used

- Python  
- Pandas  
- NumPy  
- Financial Modelling Techniques  

---

## Key Insights

- Valuation is highly sensitive to WACC and growth assumptions  
- Terminal value contributes a significant portion of total valuation  
- Scenario analysis helps understand valuation under uncertainty  

---

## Limitations

- The model relies on assumptions which may not hold in the future  
- External macroeconomic factors are not fully captured  
- Results should be interpreted as estimates, not exact values  

---

## Conclusion

This project demonstrates how real-world financial valuation models are built using Python. It combines financial theory with practical implementation, similar to models used in investment banking and equity research.
