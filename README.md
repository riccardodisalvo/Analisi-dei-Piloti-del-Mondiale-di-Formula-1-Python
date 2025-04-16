# Project Analysis Formula 1 Pilots

This project implements the following 3 functions, importing a CSV file called `formula1_data.csv`:

1. **Driver Statistics Function:**
   - Function: `get_pilot_stats(data_pilot, pilot_name)`
   - Takes as input the name of a driver.
   - Returns a list containing:
     - The driver's total points.
     - The number of victories (how many times the driver finished first).
     - The number of podiums (how many times the driver finished in the top three).

2. **Drivers Standings Function:**
   - Function: `total_points(data_pilot)`
   - Reads race data from a CSV file.
   - Calculates the total points for each driver.
   - Returns a dictionary consisting of key-value pairs:
     - Key: A string containing the driver's name.
     - Value: An integer representing the total points the driver has accumulated by the end of the World Championship.
   - Saves the standings in a txt file called 'Drivers_Standings_2008.txt'.

3. **Constructors Standings Function:**
   - Function: `total_team_points(data_pilot, driver_points)`
   - Reads the drivers' standings from the previously generated txt file.
   - Calculates the total points for each constructor by summing up the points of the drivers racing for the constructor.
   - Returns a dictionary consisting of key-value pairs:
     - Key: A string containing the name of the constructor (Team).
     - Value: An integer representing the total points the constructor has accumulated by the end of the Championship.

## Data

The data used in this project is sourced from a CSV file named `formula1_data.csv`.

### Dataset Structure

The dataset `formula1_data.csv` contains the results of the 2008 Formula 1 World Championship season. It consists of 180 rows and the following 5 columns:

1. **Driver:** Name of the Driver
2. **Team:** Constructor for which the driver races
3. **Race:** City where the Grand Prix was held
4. **Country:** Country where the Grand Prix was held
5. **Position:** A number between 0 and 8 representing the driver's position in the race (0 means the driver did not finish in the top 8).
