# Grocery Store Checkout Counter (Single Server Queue) Simulation

This project is a Python-based simulation of a single-server queuing model, specifically designed for a grocery store checkout counter. It follows the logic defined in **Table 2.10** of the textbook. The simulation calculates Inter-Arrival Times (IAT), Service Times (ST), Waiting Times (WT), and Server Idle Time based on random digit assignments and probability distributions.

## 🚀 Overview
The simulation performs the following steps:
1.  **Probability Tables:** Creates IAT and Service Time tables with cumulative probabilities.
2.  **Random Digit Mapping:** Assigns random digits to determine the IAT and Service Time for each customer.
3.  **Simulation Logic:** Calculates Arrival Time (AT), Time Service Begins (TSB), Time Service Ends (TSE), Waiting Time (WT), and Server Idle Time.
4.  **Analysis:** Provides a final simulation table for performance evaluation.

## 🛠️ Technologies Used
- **Python 3.x**
- **Pandas:** For data manipulation and table management.
- **Google Colab:** For cloud-based execution and Google Drive integration.

## 📊 Logic & Formulas
The simulation follows these core queuing theory formulas:
- **Arrival Time (AT):** $AT_i = AT_{i-1} + IAT_i$
- **Time Service Begins (TSB):** $TSB_i = \max(AT_i, TSE_{i-1})$
- **Time Service Ends (TSE):** $TSE_i = TSB_i + ST_i$
- **Waiting Time (WT):** $WT_i = TSB_i - AT_i$
- **Time in System (TTS):** $TTS_i = WT_i + ST_i$
- **Idle Time:** $Idle = TSB_i - TSE_{i-1}$ (if $TSB_i > TSE_{i-1}$)

## 🖥️ Final Simulation Output
Below is the snapshot of the generated simulation table:

![Simulation Output](YOUR_IMAGE_LINK_HERE)

> **Note:** Replace `YOUR_IMAGE_LINK_HERE` with the actual path or URL of your output image in the repository.

## 📁 File Structure
- `iat_table.csv`: Probability table for Inter-Arrival Times.
- `service_time_table.csv`: Probability table for Service Times.
- `simulation_script.ipynb`: The main execution script.

## 📝 How to Run
1. Open the `.ipynb` file in Google Colab.
2. Ensure your Google Drive is mounted.
3. Run the cells sequentially to generate the tables and the final simulation result.
