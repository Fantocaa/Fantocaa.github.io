# Logistics & Finance Workspace

For an operations team, issuing an invoice is only the start of the story. Payments may arrive later or be corrected, amounts remain receivable or payable, and the same activity has to make sense in cash and bank reports. The workspace brings those connected steps into one application.

## The problem to solve

A list of transactions is not enough if staff cannot tell what has been paid, what is still outstanding, and how a correction affects the balance. Reports also need to remain understandable when someone changes the date range or selects a different cash or bank account.

## How I approached it

I worked on the invoice payment calculations, receivables and payables, and settlement corrections alongside the reporting views. The cash and bank reports bring forward an opening balance, apply date and account filters, and show a running balance. They can also be exported to PDF or a spreadsheet when the team needs to review the figures outside the app.

Laravel handles the transaction and reporting logic; React and TypeScript provide the workspace where staff enter and inspect records. The transaction and reporting views need to describe the same underlying activity, even after a payment is corrected.

## What this delivers

Staff can review the same financial activity at different stages: what was invoiced, what has been settled, and how it appears in the cash or bank report.

This is a private project. Client records and source code are not published here. [Discuss a similar project](mailto:fantocaa17@gmail.com).
