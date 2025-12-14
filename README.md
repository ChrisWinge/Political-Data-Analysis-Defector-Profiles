# Strategic Messaging Analysis: Targeting 2024 "Democratic Defectors"

## 🎯 Project Goal
This analysis identifies the most effective economic policy frames to win back **"Democratic Defectors"**—voters who participated in the 2024 Democratic primary but cast a vote for a non-Democratic candidate in the general election.

---

## 🛠️ The Technical Challenge
Working with the **2024 Cooperative Election Study (CES)**—a massive dataset with over 60,000 respondents—requires more than just simple averages. To ensure professional-grade accuracy, this project implemented:

* **Voter Validation:** Filtered the raw sample down to validated registered voters who completed both pre- and post-election survey waves.
* **Weighted Descriptive Analysis:** Applied `vvweight_post` (post-stratification weights) to ensure results are representative of the actual U.S. electorate rather than just the raw survey sample.
* **Data Integrity Protection:** Developed a custom row-by-row alignment loop to handle complex missing values (NaNs). This ensured every policy support calculation was perfectly paired with its corresponding statistical weight, preventing biased results.

---

## 💻 Key Technical Skills
* **Python Data Stack:** Advanced usage of `Pandas`, `NumPy`, `Matplotlib`, and `Seaborn`.
* **Complex Data Cleaning:** Implementation of masked alignment, `.loc` assignment, and mitigation of `SettingWithCopy` warnings.
* **Programmatic Visualization:** Generation of a 2x2 grid of subplots featuring partisan color-mapping (`RdBu_r`) and automated percentage formatting (`PercentFormatter`) for stakeholder-ready reporting.
* **Advanced Segmentation:** Utilizing the 7-point partisan identity scale (`pid7`) to isolate and analyze movable sub-groups within the defector population.

---

## 📊 Strategic Findings & Recommendations
The data revealed a clear path for winning back defectors through specific economic messaging:

* **The Consensus Bridge:** **Infrastructure Investment ($150B/year)** emerged as the most powerful message, commanding **85.5% support** among defectors—outperforming traditional tax policy messages by nearly 30 points.
* **The Movable Middle:** Voters identified as "Not very strong Democrats" (PID 2) showed a remarkable **99.7% support** for infrastructure, despite being highly conflicted on individual tax cuts.
* **Messaging Guidance:** While defectors support taxing the wealthy (58.8%), a majority also support extending existing tax cuts (60.9%). Successful messaging should pivot toward **"public investment and infrastructure growth"** rather than "tax repeal" to avoid alienating this segment.

<img width="987" height="759" alt="image" src="https://github.com/user-attachments/assets/3239369c-0ed1-4895-bbc0-1c5ef194fa61" />


---

## 🚀 How to Run the Analysis
1. Clone this repository.
2. Download the `CCES24_Common_OUTPUT_vv_topost_final.csv` from the [CES Dataverse](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/SBYYSA).
3. Ensure you have the required libraries installed:
   ```bash
   pip install pandas numpy matplotlib seaborn

**Author**: Chris Winge

**Dataset**: 2024 Cooperative Election Study (CES)
