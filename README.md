# AF3005 - Programming for Finance 
# Assignment # 01
# Smart Financial Management System - SecureBank

## Description
This repository contains the implementation of the **Smart Financial Management System** for SecureBank. The system is designed to automate various financial operations using Python, with interactive elements powered by `ipywidgets`. The project is divided into five key modules, each focusing on a different aspect of financial management.


## Objectives
The primary goals of the Smart Financial Management System are to:
1. **Assess customer eligibility for loans.**  
2. **Classify investment portfolios based on risk.**  
3. **Automate loan repayment tracking.**  
4. **Monitor stock market trends and trigger alerts.**  
5. **Track currency exchange rates and suggest conversions.**  


## Features and Implementation Details

### 🟢 Part 1: Loan Eligibility Checker  
**Objective:**  
Assess customer eligibility for loans based on employment status, income, and credit score.

**Functionality:**  
- **Employment Verification:** Rejects the loan immediately if the customer is unemployed.  
- **Income Check:** Approves the loan only if the monthly income is at least PKR 50,000.  
- **Credit Score Evaluation:**  
  - `750+`: Loan Approved at **5% Interest Rate**.  
  - `650 - 749`: Loan Approved at **8% Interest Rate**.  
  - `Below 650`: Loan Rejected.  

**Interactive Features:**  
- User inputs for employment status, monthly income, and credit score.  
- Displays loan approval status and interest rate, if applicable.  

---

### 🟢 Part 2: Investment Risk Assessment  
**Objective:**  
Classify investment portfolios based on the risk level of stock returns.

**Functionality:**  
- **High Risk:** If any stock has a **negative return**.  
- **Medium Risk:** All stocks have positive returns, but at least one is below 5%.  
- **Low Risk:** All stock returns are **5% or above**.  

**Interactive Features:**  
- Accepts a list of stock returns as input.  
- Displays the portfolio's risk level.  


### 🟢 Part 3: Loan Repayment Tracker  
**Objective:**  
Automate loan repayment tracking and provide a real-time balance overview.

**Functionality:**  
- Starts with an **initial loan balance** (e.g., PKR 500,000).  
- Deducts a **fixed monthly payment** (e.g., PKR 25,000).  
- Continues until the loan balance reaches zero.  
- Displays the **remaining balance** after each payment.  

**Interactive Features:**  
- User inputs for initial loan amount and monthly payment.  
- Real-time display of remaining balance after each installment.  


### 🟢 Part 4: Stock Price Monitoring and Trading Strategy  
**Objective:**  
Monitor stock prices and trigger alerts based on trading strategies.

**Functionality:**  
- **Skip** missing stock data (`None` values).  
- **Stop tracking** once the stock price reaches **PKR 200**.  
- Displays tracked prices and alerts when the target price is reached.  

**Interactive Features:**  
- Input for a list of daily stock prices.  
- Outputs a log of tracked prices and trading alerts.


### 🟢 Part 5: Currency Exchange Rate Tracker  
**Objective:**  
Track daily currency exchange rates and provide conversion suggestions.

**Functionality:**  
- Starts at **PKR 290/USD** and **increases by 1 PKR** per day.  
- **Stops tracking** once it reaches the target rate of **PKR 300/USD**.  
- Logs the daily exchange rate and suggests conversions when favorable.  

**Interactive Features:**  
- Inputs for starting rate, target rate, and daily increment.  
- Real-time display of the daily exchange rate.  


## Implementation Details
- **ipywidgets:** Used for all interactive inputs and outputs.  
- **Loops:** Efficient iteration over lists for stock returns, stock prices, and currency rates.  
- **Conditional Statements:** To evaluate loan eligibility, risk classification, and trading strategy.  
- **Break and Continue Statements:** Efficient flow control in stock price monitoring and currency tracker.  



## How to Run
- Open the notebook in Jupyter.
- Ensure `ipywidgets` is installed (`pip install ipywidgets`).
- Run each cell sequentially for interactive functionality.


## Author
- Ahmed Saleh Riaz
- 22i-2289
