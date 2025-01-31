# 🚗 Car Auction Data Analysis  
📊 *Final Project - MIS 6382 - The University of Texas at Dallas*  

### 📌 Overview  
The dataset contains information about cars listed on an auction website, covering both **electric** and **non-electric vehicles** from various manufacturers. It includes **attributes** such as **make, model, year, fuel type, transmission, mileage, price**, and other relevant details. This **dataset** can be useful for **data analysis, price prediction models, and trend analysis** in the automotive market 🚗⚡📊 using **Python** and **Object-Oriented Programming (OOP)** principles.

🔗 **Project Deliverables:**  
- 📝 **Python Code (Jupyter Notebook)**  
- 📈 **Data Visualizations & Analysis**  
- 📑 **Documentation**  
- 🎤 **Final Presentation Slides**  

---

## 📂 Project Structure  
```
📁 Car-Auction-Data-Analysis
│── 📄 FinalProjectCode.ipynb  # Jupyter Notebook with code & analysis
│── 📊 Group04_MIS6382.501_FinalPresentation.pptx  # Presentation slides
│── 📜 README.md  # This file
```

---


## 📊 Data Visualization Requirements  
Use **Python** to generate the following **seven types of visualizations** to explore and present data trends:  

📊 **Bar Charts** - Comparing car prices across manufacturers.  
📦 **Boxplots** - Displaying price distributions.  
📈 **Line Plots** - Tracking car price trends over time.  
🔵 **Scatter Plots** - Examining price vs. mileage relationships.  
📊 **Histograms** - Understanding price distributions.  
🥧 **Pie Charts** - Showing manufacturer market share.  
🌡️ **Heat Maps** - Identifying customer rating trends (Extra).  

Each visualization must have a **clear explanation** describing data trends.

---

## 📝 Project Components  
### 🏛 **Object-Oriented Programming (OOP) Implementation**  
The project involves **building Python classes** to structure the dataset effectively.

📌 **Class Structure:**  
1️⃣ **Car Class** 🏎️  
   - Attributes: `date`, `model`, `company`, `type`, `rating`, `price`, `mileage`  
   - Includes a **Unique ID** (`unique_id`) assigned using `id(self)`.  
   - Implements `__str__` method to return a **formatted string representation**.  

2️⃣ **Subclasses:**  
   - 🔌 **ElectricCar** → Represents electric cars.  
   - 🚗 **NonElectricCar** → Represents non-electric cars.  

3️⃣ **Brand-Specific Subclasses:**  
   - 🚘 **Tesla (inherits ElectricCar)**  
   - 🚙 **Ford (inherits NonElectricCar)**  
   - 🚗 **BMW (inherits NonElectricCar)**  

📌 **Example Usage:**  
```python
FordCar = Ford("2022-11-15", "Model A", 2, 641, 86.06)
print(str(FordCar))
# Output: unique_id,2022-11-15,Model A,Ford,NonElectric,2,641,86.06
```

---

## 📂 **Dataset Processing & CSV Generation**  
📌 Steps to **process and convert the dataset** into CSV:  
1️⃣ Load the **provided dataset (pickle file)**.  
2️⃣ Convert the objects into a structured **CSV file**.  
3️⃣ Write the **column headers**:  
   ```
   unique_id,date,model,company,type,rating,price,mileage
   ```
4️⃣ Loop through objects and save them in CSV format.  

📌 **Snippet for CSV Generation:**  
```python
with open('data.csv', 'w') as f:
    f.write("unique_id,date,model,company,type,rating,price,mileage
")
    for obj in objects:
        f.write(str(obj) + '\n')
```

---

## 📜 **Documentation Requirements**  
📌 The Jupyter Notebook should include:  
✅ **Introduction** - Overview of the dataset & attributes.  
✅ **Data Cleaning** - Handling missing values:  
   - Categorical → Replace with **mode**.  
   - Numerical → Replace with **mean/median**.  
✅ **Data Trends** - Explanation of each visualization.  
✅ **Conclusion** - Summary of key insights.  
✅ **Recommendations** - Suggestions for improving dataset quality.  

---

## 📌 **Key Insights from Analysis**  
✔ **Price Comparison:** No major differences in **average car price** across Tesla, Ford, and BMW.  
✔ **Trend Over Time:** Price drops **sharply in September 2022** and rises in **December 2022**.  
✔ **Price vs. Mileage:** Higher mileage **generally** leads to lower prices.  
✔ **Market Share:** Tesla holds the **largest share**, accounting for nearly **50%** of the dataset.  
✔ **Customer Ratings:** Most cars are rated between **1-3**, with **Tesla having higher ratings overall**.  

---

## 💡 **Recommendations**  
🔹 **Include more vehicle specifications** (e.g., engine size, fuel efficiency).  
🔹 **Add historical maintenance data** to analyze long-term value.  
🔹 **Expand dataset coverage** to more car manufacturers.  
🔹 **Incorporate geographic data** for regional pricing trends.  
🔹 **Analyze seasonal patterns** to identify best buying/selling periods.  

---

## 🚀 **Technologies Used**  
- 🐍 **Python** (Jupyter Notebook)  
- 📊 **Matplotlib & Seaborn** (Data Visualization)  
- 🏗 **Object-Oriented Programming (OOP)**  
- 📝 **CSV & Pickle for Data Handling**  

---

## 📥 **How to Run the Project**  
1️⃣ Clone the repository:  
   ```bash
   git clone https://github.com/prayag-verma/Car-Auction-Data-Analysis.git
   cd Car-Auction-Data-Analysis
   ```

2️⃣ Run the Jupyter Notebook:  
   ```bash
   jupyter notebook FinalProjectCode.ipynb
   ```

3️⃣ Review the visualizations and analysis.  

---

### 📢 **Contributors**  
👤 **Prayag Verma**  
👥 **The University of texas at Dallas**  

🔗 **Portfolio:** [profile.aimtocode.com](https://profile.aimtocode.com/)  
🔗 **LinkedIn:** [linkedin.com/in/prayagv](https://www.linkedin.com/in/prayagv/)

💬 Feel free to raise an issue or contribute via pull requests!  

---

### 📜 **License**  
📄 This project is licensed under the **MIT License**.  
