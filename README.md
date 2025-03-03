# Calendar Generator

This project generates a yearly calendar based on a given year. It calculates the starting day of the week for each month and displays the calendar in a structured format. Additionally, it explains the calculation process, including how leap years affect the calendar.

## Features

- Enter a year to generate a full yearly calendar.
- Automatically accounts for leap years.
- Displays a month-by-month calendar breakdown, showing the week's days and dates.
- Includes a toggleable explanation on how the calendar is generated.

## How It Works

The calendar generator uses the following approach:

1. **Leap Year Calculation**: The program checks if a year is a leap year. Leap years have 366 days, while non-leap years have 365 days. The formula for determining leap years is:  
    A year is a leap year if:
    - It is divisible by 4, but not by 100, unless it is also divisible by 400.

2. **Odd Days Calculation**: For each month, the program calculates the "odd days." This determines which day of the week the month starts on:
    - The total number of days from previous years and months is calculated.
    - The remainder when divided by 7 gives the odd days, which determine the starting day of the month.

3. **Calendar Display**: The calendar for each month is displayed in a table format, with each day of the week marked and the dates filled in accordingly.

### Understanding Odd Days and Leap Years  

The concept of **odd days** helps determine the day of the week for a given date. Odd days are calculated as the number of days remaining after complete weeks are subtracted. This remainder is critical in calendar computations.  

---

### Days of the Week  
The days of the week are:  
**Sunday, Monday, Tuesday, Wednesday, Thursday, Friday, and Saturday.**  

---

### Odd Days in a Year  
1. **Ordinary Year**:  
   - Contains 365 days.  
   - Dividing 365 by 7 leaves a remainder of 1, so an ordinary year has **1 odd day**.  

2. **Leap Year**:  
   - Contains 366 days, with February having 29 days.  
   - Dividing 366 by 7 leaves a remainder of 2, so a leap year has **2 odd days**.  

---

### Leap Year Rules  

A leap year occurs every 4 years, but with specific conditions:  

1. **Case 1**:  
   - If the last two digits are **not zero**, the year is a leap year if divisible by 4.  
   - Example:  
     - **2012** (divisible by 4) → Leap year.  
     - **2014** (not divisible by 4) → Not a leap year.  

2. **Case 2**:  
   - If the last two digits are **zero**, the year is a leap year only if divisible by 400.  
   - Example:  
     - **2000** (divisible by 400) → Leap year.  
     - **1000** (not divisible by 400) → Not a leap year.  

---

### Odd Days in Centuries  

1. **100 years**:  
   - 24 leap years + 76 ordinary years.  
   - Total odd days = (24 × 2) + (76 × 1) = 124.  
   - Dividing 124 by 7 gives a remainder of **5**, so 100 years have **5 odd days**.  

2. Odd days for longer periods:  
   - **200 years** = \( 2 × 5 = 10 \mod 7 = 3 \) odd days.  
   - **300 years** = \( 3 × 5 = 15 \mod 7 = 1 \) odd day.  
   - **400 years** = \( 4 × 5 = 20 + 1 \) (leap year) = \( 21 \mod 7 = 0 \) odd days.  

---

### Summary of Odd Days  

| **Years**         | **Odd Days** |  
|--------------------|--------------|  
| Ordinary Year      | 1            |  
| Leap Year          | 2            |  
| 100 Years          | 5            |  
| 200 Years          | 3            |  
| 300 Years          | 1            |  
| 400 Years          | 0            |  

---

### Day of the Week Based on Odd Days  

The day of the week corresponds to the number of odd days:  

| **Odd Days** | **Day**      |  
|--------------|--------------|  
| 0            | Sunday       |  
| 1            | Monday       |  
| 2            | Tuesday      |  
| 3            | Wednesday    |  
| 4            | Thursday     |  
| 5            | Friday       |  
| 6            | Saturday     |  

---

### Conclusion  

- Odd days are the extra days beyond complete weeks in a given period.  
- By calculating odd days, we can find the day of the week for any date.  
- Leap years play a significant role in determining the total number of days in a year.  
- Leap years follow specific rules, ensuring calendar accuracy over centuries.  

Understanding odd days simplifies the process of determining the weekday for historical or future dates!

