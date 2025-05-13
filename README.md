# 🧾 Excel Retail Sales Data Assignment

This project showcases data cleaning, transformation, and analysis performed on an online retail dataset using Microsoft Excel. The goal was to answer a structured set of business questions provided in a PDF using formulas, charts, and PivotTables in Excel.

---

## 📄 Files in This Repository

- [**📊 Excel assignment 2.xlsx**](./Excel%20assignment%202.xlsx) – The completed Excel workbook with all solutions implemented.
- [**📑 Assignment Questions (PDF)**](./67f8ff6f877553f71d753602.pdf) – The original assignment instructions (includes a link to the Excel solution).


---

## ✅ Problem Areas Covered

### 1. **Data Cleaning & Transformation**
- Identified and highlighted nulls in `Quantity`, `Price_Per_Unit`, and `Total_Amount` using Conditional Formatting.
- Replaced `"null"` text values with actual blanks and filled missing numerical values using the column average.
- Used `TRIM()` to remove extra spaces in the `Product` column.
- Converted all entries in `Customer_Region` to uppercase using the `UPPER()` function.

  ![Screenshot 2025-05-13 102822](https://github.com/user-attachments/assets/0854fbc8-0e2e-4846-8634-8ab06a8f8f12)


---

### 2. **Pivot Table Analysis**
- Created a PivotTable to display total revenue (`Total_Amount`) grouped by `Customer_Region`.
- Identified the region with the highest revenue.
- Applied **Data Bars** to visualize relative performance of each region.

![Screenshot 2025-05-13 102845](https://github.com/user-attachments/assets/0f81fe9d-b33d-479f-8a18-60e9a5f7320f)

---

### 3. **Lookup Operations**
- Used `VLOOKUP` to find `Total_Amount` for `Order_ID = 1015`.
- Used `INDEX/MATCH` to retrieve the `Category` for `Order_ID = 1027`.
- Compared both methods:
  - `VLOOKUP` is easier to use but less flexible.
  - `INDEX/MATCH` allows for dynamic lookups in either direction and is more robust.

    ![Screenshot 2025-05-13 102856](https://github.com/user-attachments/assets/666f30ae-80a6-4ede-a8d9-1b9c6738b59f)


---

### 4. **Trend Analysis**
- Created a **Line Chart** to plot `Total_Amount` over `Order_Date`.
- Analyzed the trend:
  - Identified a major spike in early April.
  - No clear seasonal pattern observed across other months.

![Screenshot 2025-05-13 102905](https://github.com/user-attachments/assets/c86378fc-9a57-472c-9429-723269bb171d)

---

### 5. **Profit Margin Calculation**
- Added a new column:
  ```excel
  Profit_Margin = Total_Amount - (Quantity × Price_Per_Unit × 0.6)

  

![Screenshot 2025-05-13 102936](https://github.com/user-attachments/assets/31831a94-394c-4046-b492-96b47df5b953)

  

