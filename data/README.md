### Data File Descriptions

#### Source Data Files
- AwardsPlayers.csv - From Lahman database.  List of Post Season Awards per player per year.
Batting.csv - From Lahman database.  Primary driver file for data preparation.  Lists offensive statistics per year, per player, per stint.
- Fielding.csv - From Lahman database.  Lists defensive statistics per year, per player, per stint, per position.
- Inflation.csv - Adapted from "SalaryInflationIndex.csv".  Modified to have python friendly headers and values.
- MLB_MinSalary_1967-2017.csv - From Jeff.  League minimum salaried per year.
- Minimum-AverageSalaries.csv - From Jeff.
- MinimumSalaries.csv - Adapeted from MLB_MinSalary_1967-2017.csv.  Modified to have python friendly headers and values.
- Salaries.csv - From Lahman database.  Salaries per player per year per team.
- SalaryInflationIndex.csv - From Jeff. Salary adjustment data to convert salaries to 2017 figures.

#### Data Prep Output Files
- player.csv - No pitchers.  One record per player per year.  Combination of player, fielding, salary, batting, Inflation and minimum salary data files.
- playerNoSal.csv.  Same as player.csv but filtered for players with salary > 0.
- playerNoSalscale.csv - Scaled version of playerNoSal.csv
- playerscale.csv = Scaled version of player.csv
