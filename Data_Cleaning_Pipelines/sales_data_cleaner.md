# Master Template: Unstructured Sales Data Cleaner

### Role
Act as an expert Data Analyst specializing in data wrangling and validation.

### Context
I have a raw, messy text paragraph containing various weekly sales metrics, unstructured product mentions, and mixed formatting.

### Task
Parse the attached text dataset. Isolate, extract, and clean the core metrics to make them ready for an analytical dashboard.

### Constraints
1. If any metric (Quantity or Revenue) is missing for a product, output "NOT SPECIFIED". Do not approximate or invent numbers.
2. Do not write any conversational introduction, friendly greetings, or concluding text. 
3. Output raw structured data only.

### Output Format
Present the final cleaned data strictly as a 3-column Markdown table:
| Product_Name | Quantity_Sold | Total_Revenue |

---

##  Live Execution Example

###  1. Messy Input Data (Unstructured Text)
"Hey team, quick update on this week's electronic components shipment. The Alpha-Inverter-X units did amazing, we managed to move about 140 of them which brought in a solid $28,000 in total revenue. On the other hand, the Beta-Circuit-Boards were incredibly slow—only 12 units left the warehouse, but the finance log doesn't even specify the revenue generated for them yet, so we need to track that down. Oh, and the Gamma-Switch-Links also shipped out, hitting a total revenue of $4,500 for 90 units sold."

###  2. Deterministic Output (The AI Result)
Because of the strict constraints applied in the prompt above, the model bypassed the conversational text, caught the missing financial log, and generated this clean data table on the first try:

| Product_Name | Quantity_Sold | Total_Revenue |
| :--- | :--- | :--- |
| Alpha-Inverter-X | 140 | $28,000 |
| Beta-Circuit-Boards | 12 | NOT SPECIFIED |
| Gamma-Switch-Links | 90 | $4,500 |
