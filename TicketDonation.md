# Problem Analysis: Theater Ticket Donation

## Problem Statement

A theater owner agrees to donate a portion of gross ticket sales to a charity. The program is designed to calculate the donation amount based on the following user inputs:

1. Movie Name: The name of the movie being shown at the theater.
2. Adult Ticket Price: The price of an adult ticket for the movie.
3. Child Ticket Price: The price of a child ticket for the movie.
4. Number of Adult Tickets Sold: The number of adult tickets sold for the movie.
5. Number of Child Tickets Sold: The number of child tickets sold for the movie.
6. Percentage of Gross Amount to be Donated: The percentage of the total gross ticket sales that the theater owner agrees to donate to a charity.

The program's objective is to calculate the total gross ticket sales and the donation amount based on the provided inputs.

## Input

The program will prompt the user to input the following information:
- **Movie Name**: A string representing the name of the movie.
- **Adult Ticket Price**: A positive float representing the price of an adult ticket.
- **Child Ticket Price**: A positive float representing the price of a child ticket.
- **Number of Adult Tickets Sold**: A non-negative integer representing the number of adult tickets sold.
- **Number of Child Tickets Sold**: A non-negative integer representing the number of child tickets sold.
- **Percentage of Gross Amount to be Donated**: A float between 0 and 100 representing the percentage of the total gross ticket sales that the theater owner agrees to donate to a charity.

## Output

The program should provide the following output:
- **Movie Name**: The name of the movie.
- **Total Gross Ticket Sales**: The total gross ticket sales, calculated as the sum of the sales from adult and child tickets.
- **Donation Amount**: The amount that will be donated to the charity, calculated based on the percentage of the total gross amount.

## Constraints

- The adult ticket price and child ticket price are positive float values.
- The number of adult tickets sold and number of child tickets sold are non-negative integers.
- The percentage of gross amount to be donated is a float between 0 and 100.

## Example

### Input

```plaintext
Movie Name: "Avengers: Endgame"
Adult Ticket Price: 12.50
Child Ticket Price: 7.50
Number of Adult Tickets Sold: 150
Number of Child Tickets Sold: 50
Percentage of Gross Amount to be Donated: 10.5
