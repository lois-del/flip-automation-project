# flip-automation-project
This repo is for a database solution that tracks withdrawal charges and automatically updates rollover information on a bank's investment product 

Overview
This project automates the computation of withdrawal charges and updates rollover information for a financial institution’s investment product (code-named "FLIP"). It empowers branch teams to instantly advise customers on how much a customer can withdraw with associated charges incurred.

Problem
The product team introduced a modified version of the FLIP investment product — keeping the original name but adding new features and a new product code. 
However, the core banking application could not fully support the enhanced logic around withdrawal charges and rollover rules.

This created a critical gap in operational readiness before go-live. Specifically:
- The system lacked logic to reflect updated product behavior
- There was no built-in support to determine penalty-free withdrawal amounts
- Branch staff needed a reliable, user-friendly way to advise customers accurately from day one

Solution
I designed and implemented a backend solution to:
- Track each customer’s rollover status based on product rules
- Dynamically compute allowable withdrawal amounts and associated charges
- Feed this logic into a centralized reporting tool for branch-wide access
- Ensure business continuity despite the limitations of the core banking platform

Tools & Technologies
- Oracle SQL – data modeling, stored procedures, ETL logic
- Business Objects – front-end visualization for business users
- Excel - initial simulation and validation phase

Key Features
- Charge computation engine based on revised FLIP product rules
- Automated tracking of rollover status and investment maturity
- User-accessible interface with read-only logic (no manual edits)
- Built-in flexibility to accommodate future changes to the product

Impact
- Enabled 100% readiness for go-live across all branches
- Reduced manual dependencies and potential for advisory errors
- Provided real-time, accurate withdrawal guidance from day one
- Set a reusable model for handling future product modifications
- Flagged a loophole where users could withdraw via the mobile app bypassing branch advisory, and escalated it for prompt fix before go-live.

