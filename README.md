# Bacen Currency Converter (Excel Automation) 💱

This project automates the update of exchange rates in an Excel workbook using **official data from the Central Bank of Brazil (BACEN)**.  
It combines **Power Query**, **Excel Scripts**, and **Power Automate** to keep currency conversions in BRL (Brazilian Real) automatically up to date.


## How It Works

The automation runs on a simple Power Automate flow:

1. **Recurrence trigger** — defines how often the process runs (daily, hourly, etc.).  
2. **Run Script** — executes an Excel Script that refreshes all Power Query connections in the workbook.


## Technologies Used

- **Excel + Power Query** — to import and transform BACEN’s currency rate data  
- **Power Automate** — to schedule and trigger automatic updates  
- **Excel Script (Office Scripts)** — to refresh all data connections via code  


## How to Use

1. Open the provided Excel file and check the Power Query connections.  
2. Store the file in **OneDrive** or **SharePoint**.  
3. Import the Power Automate flow.  
4. Link the “Run Script” action to your Excel Script.  
5. Set your desired recurrence (e.g. every 24 hours).  

💡 Notes
+ Make sure the Excel file is accessible from Power Automate.
+ The flow can be customized to trigger on-demand or on a schedule.
+ For advanced scenarios, you can extend the Power Query to convert multiple currencies automatically.

---

## Data Source 🌎

Exchange rates are retrieved directly from:
+ Banco Central do Brasil - [Open Data](https://dadosabertos.bcb.gov.br/)
+ Banco Central do Brasil - [Exchange Rate API](https://ptax.bcb.gov.br/ptax_internet/consultaBoletim.do?method=consultarBoletim&RadOpcao)

---
