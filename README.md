# Atlantic Hurricanes Analysis – Excel Project

## 🎯 What I Built
In this project from my justIT Data Skills Bootcamp, I worked with a dataset of major Atlantic hurricanes. The core task was to populate the "Max Wind Speed" column by using the `SWITCH` function to look up the correct speed based on the storm's category (1-5), referencing a key within the worksheet.

#### Biggest Hurricanes Data Table
<img width="590" height="566" alt="Biggest_Atlantic_Hurricanes_data_table" src="https://github.com/user-attachments/assets/a6e1c557-b502-422b-9d02-1dc0206eb4f5" />


## 💡 Key Things I Learnt
- **The `SWITCH` Function**: I learned how to use `SWITCH` as an efficient alternative to a nested `IF` statement for matching a value against a list of possibilities.
- **Absolute Cell Referencing**: This was the most important lesson. By using `$` signs (e.g., `$B$32`), I locked the formula's reference to the wind speed key. This ensured that when I dragged the formula down, it continued to look at the correct key instead of shifting downwards, which would have broken the calculation.
- **Data Integrity**: This task showed me how formulas can be used to complete missing data in a consistent and accurate way, which is a fundamental step before any analysis can be done.

#### Example Switch Formula
<img width="584" height="470" alt="Biggest_Atlantic_Hurricanes_switch_formula" src="https://github.com/user-attachments/assets/b13a4f25-f3b7-4065-b692-7d4f764b4c78" />


## 🔍 Formula Breakdown
This is an exact formula I used in the "Max Wind Speed" column:
`=SWITCH(D6,1,$B$32,2,$B$31,3,$B$30,4,$B$29,5,$B$28,"Unknown")`

-   `SWITCH(D6, ...)`: It checks the value in cell `D6` (the category number).
-   `1, $B$32`: If the category is `1`, it returns the value from cell `$B$32`.
-   `2, $B$31`: If the category is `2`, it returns the value from cell `$B$31`, and so on.
-   `"Unknown"`: If the category is not 1-5, it returns "Unknown".
-   The `$` symbols make the references to the key (e.g., `$B$32`) absolute, which is essential for the formula to work correctly when copied across multiple rows.

## 🛠️ Excel Skills Demonstrated
- `SWITCH` function for conditional logic and lookups
- Absolute vs. Relative Cell Referencing
- Populating data based on a worksheet key
- Basic formula-based data completion

## 🚀 How to Explore
1.  Download `Biggest Atlantic Hurricanes.xlsx`.
2.  Click on any cell in the "Max Wind Speed" column (Column E) to see the `SWITCH` formula in action.
3.  Observe how the formula references the key located in cells B28:B32 at the bottom of the sheet.

## 📁 Project Files
- `Biggest Atlantic Hurricanes.xlsx` - The completed worksheet with the `SWITCH` formula.
- `screenshots/hurricane-switch-formula.png` - The screenshot showing the formula.
- `README.md` - This guide.

## 🎓 Part of My Bootcamp Journey
This project was a practical exercise from Week 1 / Day 3 of my bootcamp, focusing on advanced Excel formulas.

## 🤔 If I Had More Time
- The next logical step would be to use this now-complete dataset to perform a full analysis with Pivot Tables to find insights, such as which wind speed category has caused the most financial damage.

---
*Week 1 of 8 – justIT Data Skills Bootcamp*
