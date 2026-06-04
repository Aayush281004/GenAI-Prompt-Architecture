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
