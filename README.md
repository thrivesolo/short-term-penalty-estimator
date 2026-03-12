# Penalty & Interest Calculator

This simple web app helps individual taxpayers estimate the IRS **penalties and interest** they might owe when paying a 1040 tax balance after the April 15 deadline.[web:18][web:19]

It is designed for clarity and ease of use so you can quickly see the cost of waiting to pay.

---

## What this tool does

- Estimates **failure‑to‑pay penalties** on an unpaid individual income tax balance.[web:19][web:38]
- Estimates **interest** the IRS charges on unpaid balances, using a flat annual rate (compounded daily).[web:10][web:33][web:36]
- Shows how much extra you would pay if you make a **single lump‑sum payment on the 15th of each month from May through September** (short‑term payment window).[web:34][web:39]

This is a **planning tool**, not an official IRS calculator.

---

## How to use it

1. **Open the app**

   If this repository is published on GitHub Pages, you can visit the live link in your browser (for example:  
   `https://<your‑github‑username>.github.io/short-term-penalty-estimator/`).

   Or open `index.html` (or `penalty_interest_calculator.html`) directly in your browser.

2. **Enter your unpaid balance**

   - Type your unpaid balance into the **“Unpaid balance”** field.
   - The field automatically formats the amount in US dollars with no cents.

3. **Review the assumptions**

   - **Original due date:** Fixed at **April 15**, assuming you filed on time (no failure‑to‑file penalty).[web:35]
   - **Failure‑to‑pay penalty:** Default **0.5% per month** on the unpaid balance.[web:38]
   - **Interest rate:** Default **7.0% per year**, compounded daily (aligned with recent IRS underpayment rates).[web:10][web:36]
   - Both rates can be adjusted if IRS rules or your situation differ.

4. **Click “Update estimates”**

   The table will display, for each month (May–September):

   - **Payment date** (15th of the month)
   - **Penalty**
   - **Interest**
   - **Total additional cost** (penalty + interest)
   - **Total due** (original balance + total additional cost)

---

## What this tool assumes

- You are an **individual (Form 1040) taxpayer**.
- Your **return was filed on time**, so only failure‑to‑pay penalties and interest are modeled.[web:19][web:35]
- You make **one lump‑sum payment** by a specific date.
- You are looking at a **short‑term horizon** (within roughly 180 days) rather than a long‑term installment agreement.[web:34][web:39]
- The penalty and interest rates stay **constant** during the period (in reality, IRS interest rates can change quarterly).[web:10][web:33][web:36]

Because of these simplifications, your actual IRS bill may differ.

---

## Important disclaimer

This calculator is for **educational and planning purposes only**. It does **not**:

- File or pay your taxes.
- Replace official IRS notices or calculations.
- Account for all possible penalties (for example, failure‑to‑file penalties or penalties after a levy notice).[web:19][web:18][web:31]

For personalized advice about your situation, you should speak with a qualified tax professional.

---

## Running locally

You do not need any special tools or libraries.

1. Clone the repository:

   ```bash
   git clone https://github.com/thrivesolo/short-term-penalty-estimator.git
   cd short-term-penalty-estimator
