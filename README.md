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

## Usage

1. Open the HTML file in a browser.
2. Enter a year in the input field and click the **Generate Year Calendar** button.
3. The calendar for the specified year will be displayed month by month.
4. Click **Show Explanation** to learn about how the calendar is generated.

## Files

- `index.html`: The HTML file containing the structure of the calendar and the JavaScript to generate it.
- `style`: Basic CSS for layout and design.

## Technologies Used

- HTML
- CSS
- JavaScript

