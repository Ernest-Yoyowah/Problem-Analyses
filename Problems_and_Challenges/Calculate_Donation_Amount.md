# Algorithm: Calculate Donation Amount

1. **Start**

2. **Declare Variables:**
   - `movieName` (string): Store the movie name.
   - `adultTicketPrice` (double): Store the price of an adult ticket.
   - `childTicketPrice` (double): Store the price of a child ticket.
   - `numAdultTicketsSold` (integer): Store the number of adult tickets sold.
   - `numChildTicketsSold` (integer): Store the number of child tickets sold.
   - `donationPercentage` (double): Store the percentage of gross amount to be donated.
   - `totalGrossAmount` (double): Store the total gross ticket sales.
   - `donationAmount` (double): Store the calculated donation amount.

3. **User Input:**
   - Prompt the user to input the following:
     - Movie name (`movieName`).
     - Adult ticket price (`adultTicketPrice`).
     - Child ticket price (`childTicketPrice`).
     - Number of adult tickets sold (`numAdultTicketsSold`).
     - Number of child tickets sold (`numChildTicketsSold`).
     - Percentage of gross amount to be donated (`donationPercentage`).

4. **Calculate Total Gross Amount:**
   - `totalGrossAmount` = (adultTicketPrice * numAdultTicketsSold) + (childTicketPrice * numChildTicketsSold).

5. **Calculate Donation Amount:**
   - `donationAmount` = (donationPercentage / 100) * `totalGrossAmount`.

6. **Display Results:**
   - "Movie Name: " + `movieName`.
   - "Gross Ticket Sales: $" + `totalGrossAmount`.
   - "Donation Percentage: " + `donationPercentage` + "%".
   - "Donation Amount: $" + `donationAmount`.

7. **End**

