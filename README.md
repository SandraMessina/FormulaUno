# FormulaUno
FormulaUno project to extract info about pilots

Dataset contains results about 2008 World Championship in 5 columns:
1. Driver: Name
2. Team: Manufacturer for which the driver competes
3. Race: City where the Grand Prix took place
4. Country: Country where the Grand Prix took place
5. Position: Number between 0 and 8 that represents the driver arrival order in the single race (0 means that the driver did not arrive in the first 8).

At the end of a Grand Prix, points are assigned to the drivers based on the order of arrival: 10 to the winner, 8 to the second, 6 to the third, and then decreasing by 1 point until the eighth.
Code meant to implement a set of functions to analyze the results of the Formula 1 World Championship:
1. A function that receives the name of a driver as input and returns a list containing the total points of the driver, the number of victories (how many times the driver arrived first) and the number of podiums (how many times the driver was on the podium).
2. A function that does not receive any input parameters and must return a dictionary made up of key-value pairs, where the key is a string containing the name of the driver, while the value associated with the key is an integer representing the total points that the driver has achieved at the end of the world championship.
It then saves the standings in a txt type text file with the following format:
Drivers Standings 2008 Formula 1
DriverName1: TotalScore
DriverName2: TotalScore.
3. A function that does not receive any input parameters and return a dictionary made up of key-value pairs, where the key is a string containing the name of the manufacturer, while the value associated with the key is an integer representing the total points that the manufacturer has achieved at the end of the world championship. The points achieved by a manufacturer are the sum of the points that the drivers who race for the manufacturer have achieved during the year. To do this, it uses the data saved in the file created previously.
