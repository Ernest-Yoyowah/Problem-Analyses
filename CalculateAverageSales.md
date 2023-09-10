## Problem Analysis

The problem is to calculate the average sales for each day, week, and month based on daily sales data.

## Algorithm: Calculate Average Sales

1. Initialize variables to keep track of daily, weekly, and monthly sales totals and counts.
   - `dailyTotal = 0`
   - `dailyCount = 0`
   - `weeklyTotal = 0`
   - `weeklyCount = 0`
   - `monthlyTotal = 0`
   - `monthlyCount = 0`

2. Start a loop to input daily sales data until the user decides to stop.
   - For each sale:
     - Input the daily sales amount (`dailySale`).
     - Add `dailySale` to `dailyTotal`.
     - Increment `dailyCount` by 1.

3. After a day's sales data has been collected, calculate and display the daily average.
   - `DailyAverage = dailyTotal / dailyCount`

4. Accumulate the daily total into the weekly and monthly totals.
   - Add `dailyTotal` to `weeklyTotal`
   - Add `dailyTotal` to `monthlyTotal`
   - Increment `weeklyCount` and `monthlyCount` by 1.

5. Check if a week or month has ended based on your business rules (e.g., every 7 days for a week, every 30 days for a month).

6. If a week has ended, calculate and display the weekly average.
   - `weeklyAverage = weeklyTotal / weeklyCount`

7. If a month has ended, calculate and display the monthly average.
   - `monthlyAverage = monthlyTotal / monthlyCount`

8. Repeat steps 2-7 as needed for new daily sales data.
