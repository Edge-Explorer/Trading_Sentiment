# Internship Assignment
# Trading_Sentiment
Explore the relationship between trader performance (Hyperliquid historical data) and Bitcoin market sentiment (Fear &amp; Greed Index).

# Trading Sentiment & Performance Analysis

## 📌 Overview

This project is part of an internship assignment aimed at analyzing the relationship between **trader performance** and **market sentiment**.
We combine historical trading data with the **Bitcoin Fear & Greed Index** to uncover patterns and generate insights that can drive smarter trading strategies in Web3 markets.

---

## 📊 Datasets

1. **Historical Trader Data** (`historical_data.csv`)

   * Columns: `Account`, `Coin`, `Execution Price`, `Size Tokens`, `Size USD`, `Side`, `Timestamp`, `Closed PnL`, `Trade ID`, etc.
   * Captures detailed trade-level activity from Hyperliquid.

2. **Bitcoin Fear & Greed Index** (`fear_greed_index.csv`)

   * Columns: `timestamp`, `value`, `classification`, `date`
   * Provides daily sentiment classification (`Fear`, `Greed`, `Extreme Greed`, `Neutral`).

---

## 🔑 Steps Performed

1. **Data Loading & Cleaning**

   * Imported historical trading data and sentiment index.
   * Standardized timestamps and extracted daily dates.

2. **Aggregation**

   * Computed **daily total PnL**, **number of trades**, and **traded volume (USD)** from raw trades.

3. **Merge with Sentiment**

   * Joined daily trader stats with sentiment data for aligned analysis.

4. **Exploratory Analysis**

   * Generated correlation matrix between PnL, trades, volume, and sentiment index.
   * Grouped performance metrics by sentiment classification.

5. **Visualization**

   * Bar plots comparing **avg PnL, avg trades, avg volume** across different sentiment phases.

6. **Insights & Conclusion**

   * Strong **negative correlation** between sentiment and performance.
   * **Fear phases** show higher profitability and stronger trading activity.
   * **Greed/Extreme Greed** phases see more trades but lower average returns.
   * Suggests that **contrarian strategies (buying during Fear)** may yield better outcomes.

---

## 📈 Key Results

* **Correlation**: Higher sentiment (Greed) = lower trader profitability.
* **Performance by Sentiment**:

  * **Fear** → Highest average PnL & activity.
  * **Greed/Extreme Greed** → High trade counts but lower returns.
  * **Neutral** → Moderate results.

---

## 🚀 How to Run

1. Clone this repository or download the notebook.
2. Install required libraries:

   ```bash
   pip install pandas matplotlib seaborn
   ```
3. Place the datasets in the same folder as the notebook.
4. Run the Jupyter Notebook:

   ```bash
   jupyter lab
   ```

---

## 📌 Conclusion

This analysis confirms a strong link between **market sentiment** and **trader performance**.

* **Fear periods** present the best opportunities for profitable trading.
* **Greed periods** may encourage over-trading with reduced efficiency.

These insights can help design smarter **risk-adjusted trading strategies** by leveraging sentiment signals.

---

## 👩‍💻 Author

* **\[Karan Rohidas Shelar]** – Data Science Intern Candidate
