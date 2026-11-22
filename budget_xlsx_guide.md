# TOTAL — a downloadable trip budget

Claude can create a downloadable XLSX with formulas from a chat request.
The numbers below are sample inputs, not ticket prices or spending forecasts.

## Steps
1. In Claude, check **Settings → Capabilities → Create and edit files**.
2. The older name is **Code execution and file creation**.
3. Start a chat and use the prompt below, replacing sample inputs with your data.
4. Download the `.xlsx` and open it in Excel or a compatible app.
5. Check formulas and units, then add one expense.

## Copy this prompt
“Create an XLSX trip budget. All amounts are in USD. Budget: 1000; outbound travel: 200; return travel: 200; accommodation: 300; food: 100. Columns: item and amount. Calculate total expenses and remaining budget with formulas, not fixed values. Do not invent expenses.”
“Leave rows for more expenses and include them in the total. Highlight a negative balance.”

## Check the sample
Initially, expenses should total 800, leaving 200.
Change food to 150: the total should become 850, leaving 150.
Add an expense of 50 in a reserved row: total 900, remaining budget 100.
If values do not update, ask Claude to fix formulas in a new copy.
For mixed currencies, agree on an exchange rate and date before combining amounts.
Workplace administrators may restrict file creation.
Source: [Create and edit files with Claude](https://support.claude.com/en/articles/12111783-create-and-edit-files-with-claude).
More tips: https://t.me/neuromentor_en
This is not official Anthropic/OpenAI material.
