> **Disclaimer**: This project was developed for work purposes, and due to confidentiality requirements, no actual data or proprietary details can be shared. However, please feel free to connect with me if you're interested in learning more about the process or discussing similar projects.


# Utilization Simulation Solution

## **Objective**

The objective of this solution is to help operations teams ensure that all headcounts (HCs) adhere to the utilization target by utilizing the correct amount of billable hours for each billable code, and meeting the target utilization percentage set by the client. The target utilization range is between **85% to 92%** of actual billable working hours for the week.

The solution is designed to simulate the remaining billable hours needed for the week, based on current data such as daily hours worked, leave tracker, and team changes.

## **Tools Used**

- **Client System**: Extracts actual hours worked on a daily basis
- **Excel**: Used for modeling, calculations, and the final utilization forecast
- **Power Query**: For data transformation and preparation
- **Advanced Excel Formulas**: For calculating total billable hours, leave adjustments, and target utilization forecasts

## **Process Flow**

1. **Data Sources**: 
    - **Actual Hours**: Extracted daily hours worked from the client system.
    - **Leave Tracker**: Keeps track of employee leaves (sick, vacation, etc.), affecting the total available working hours.
    - **Change Log**: Records any changes to the team (e.g., role change, team transfer) that might affect the billable hours.
  
2. **Billable Hours Calculation**:
    - A full-time HC has **37 billable hours per week**, assuming 5 working days with 7.4 hours each day (5 * 7.4).
    - The target utilization range is set between **85%** and **92%** of the actual working hours.

3. **Utilization Forecast**:
    - Based on current data (e.g., actual hours worked, leave tracker), the solution calculates how many hours remain for each billable code.
    - Billable codes include:
      - **Production**
      - **Meeting**
      - **Wellness**
      - **Coaching**
      - **Policy Training**
  
4. **Simulated Forecast**:
    - The forecasted hours per billable code for the remaining days of the week are calculated.
    - The system also adjusts these forecasts in real-time to account for changes such as team shifts or additional leave days.

5. **Adherence to Target**:
    - The solution ensures that the HC’s forecasted billable hours fall within the **85%-92% utilization range**.
    - If the HC’s current utilization falls outside the target range, corrective actions (like adjusting hours for each billable code) can be taken.

## **How It Works**

1. **Input Data**: 
    - Actual hours worked each day are entered into the Excel system (extracted from the client system).
    - The leave tracker and change log are used to adjust the available billable hours for each HC.
  
2. **Calculation**: 
    - Based on the leave tracker, the expected billable hours for the week are adjusted.
    - Remaining hours for the week are calculated and allocated across different billable codes (e.g., Production, Coaching, etc.).
  
3. **Forecasting**: 
    - The remaining hours per billable code are distributed proportionally across the remaining working days of the week.
    - This ensures that the HC meets the utilization target and corrects any imbalances in billable code allocation.

4. **Output**:
    - The final output is a forecast of the remaining billable hours required for the HC to meet the utilization target.
    - The simulation helps visualize how many hours should be allocated to each billable code to achieve the desired utilization percentage.

## **Challenges**

- **Multiple Billable Codes**: Different billable codes (Production, Meeting, Wellness, Coaching, Policy Training) require careful allocation to ensure the total billable hours add up correctly for each HC.
  
- **Dynamic Adjustments**: The need to adjust forecasts dynamically based on real-time data such as leave days and team changes can be complex.
  
- **Manual Process**: Extracting data from the client system, tracking leave days, and applying changes manually can be time-consuming.

## **What I Learned**

- **Optimizing Data Processing**: By leveraging Power Query in Excel, I was able to streamline the ETL process, automatically transforming data to fit the calculation needs.
  
- **Advanced Excel Formulas**: I enhanced the solution by applying advanced Excel formulas to dynamically calculate billable hours per HC and ensure utilization targets were met.
  
- **Business Acumen**: Understanding the business needs (e.g., utilization targets) and working closely with operations teams helped tailor the solution to meet stakeholder requirements. The solution bridges the gap between operational data and the key performance metrics that drive decision-making.

## **Conclusion**

This solution allows the operations team to forecast utilization accurately, ensuring that HCs adhere to the utilization targets set by the client. By simulating the remaining billable hours required for each billable code and adjusting for leaves and team changes, the solution provides actionable insights for both the operations team and the stakeholders.

