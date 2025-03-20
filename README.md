# 911 Data Analysis Project

## Overview
This project analyzes 911 call data to uncover insights regarding emergency calls, patterns, and trends. The dataset contains information such as call timestamps, locations (zip codes and townships), and reasons for emergency calls.

## Objectives
- Identify the top locations (zip codes and townships) with the highest number of 911 calls.
- Determine the most common reasons for 911 calls.
- Visualize trends in emergency calls based on time, location, and reason.
- Map traffic-related 911 calls for geographic insights.

## Technologies Used
- **Python**
- **Pandas** (for data analysis)
- **Matplotlib & Seaborn** (for data visualization)
- **Folium** (for web map generation)

## Questions & Solutions
### **1. Top 10 Zip Codes for 911 Calls**
- Computed the top 10 zip codes receiving the highest number of calls.
- **Are Zip Codes 19446 and 19090 present?** ✅ Yes, they are included in the dataset.

### **2. Top 4 Townships (TWP) for 911 Calls**
- Computed the top 4 townships with the highest number of emergency calls.
- **Missing Townships?** LOWER POTTSGROVE, NORRISTOWN, HORSHAM, and ABINGTON were checked for presence in the dataset.

### **3. Most Common Reason for 911 Calls**
- Created a new feature column "Reason" based on call categories.
- **Most Common Reason?** ✅ "Traffic" was the most common reason.
- **Second Most Common Reason?** ✅ "Fire" followed after traffic.

### **4. Barchart for 911 Calls by Reason**
- **Plotted a bar chart using Matplotlib** to visualize calls by reason.
- **How to plot bars horizontally?** ✅ Used `plt.barh()` to create a horizontal bar chart.

### **5. Countplot of Day of the Week vs. Reason**
- Used Seaborn countplot to visualize call distributions across weekdays.
- **Day with lowest traffic calls?** ✅ Sunday had the fewest traffic-related calls.

### **6. Countplot for Calls by Month**
- Created a monthly countplot to track emergency calls over the year.
- **Month with highest fire-related calls?** ✅ December had the highest number of fire-related emergency calls.

### **7. Web Map for Traffic Calls**
- Generated an interactive **Folium Web Map** for traffic-related 911 calls.
- **Why do some areas have zero or low traffic calls?**
  - Sparse population or fewer roadways in those areas.
  - Emergency calls may not be properly categorized in the dataset.

## Setup Instructions
1. **Clone this repository:**
   ```sh
   git clone https://github.com/your-repo/911-Data-Analysis.git
   cd 911-Data-Analysis
   ```
2. **Install Dependencies:**
   ```sh
   pip install pandas matplotlib seaborn folium
   ```
3. **Run the Analysis Script:**
   ```sh
   python analysis.py
   ```



