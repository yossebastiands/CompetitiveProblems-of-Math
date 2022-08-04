Agoda has made it to a parallel world where human life expectancy is exceedingly high, and people have lots of time to spend for holidays. So, a typical booking with Agoda can span tens of thousands of days!

You are a data scientist in this parallel world, and you would like to find Agoda’s busiest day, which is defined as the day with the highest total number of room nights from Agoda’s bookings. There are N bookings in Agoda’s system. Each booking has a check-in date and a check-out date. A room night is a measure of occupancy, where one room is occupied for one night.

For instance, here is an example of three bookings in the system:

Check-in date = 2121–01–01 and check-out date = 2121–01–04 (Room 001)
Check-in date = 2121–01–02 and check-out date = 2121–01–05 (Room 002)
Check-in date = 2121–01–03 and check-out date = 2121–01–06 (Room 003)
So, the total number of room nights per day is as follows:

1 on 2121–01–01 (Room: 001)
2 on 2121–01–02 (Room: 001 and 002)
3 on 2121–01–03 (Room: 001, 002, and 003)
2 on 2121–01–04 (Room: 002 and 003)
1 on 2121–01–05 (Room: 003)
0 on 2121–01–06 (Empty)
Therefore, the busiest day is 2121–01–03 because it has the highest total number of room nights.

# Input format ------------------------------------------------------------------------------------

The first line is an integer N, for the number of bookings in Agoda’s system.
N lines follow, with each line containing a check-in date and a check-out date of a booking in yyyy-mm-dd format.

# Constraints

1 <= N <= 40,000
0001–01–01 <= check-in date < check-out date <= 9999–12–31
The maximum number of days between each pair of check-in and check-out dates is 3,652,058 days.

# Output format ------------------------------------------------------------------------------------

Report the busiest day in yyyy-mm-dd format. (In the event of a tie, please report the earliest busiest day.)

# Sample input 1 ------------------------------------------------------------------------------------

3
2121–01–01 2121–01–04
2121–01–02 2121–01–05
2121–01–03 2121–01–06

(3 is the number of rooms. The dates are the corresponding check-ins and check-outs)

# Sample output 1 ------------------------------------------------------------------------------------

2121–01–03

# Sample input 2 ------------------------------------------------------------------------------------

2
2121–01–07 2121–01–09
2121–01–07 2121–01–09

# Sample output 2 ------------------------------------------------------------------------------------

2121–01–07

# Sample input 3 ------------------------------------------------------------------------------------

3
2121–01–01 2121–01–31
2121–01–10 2121–01–20
2121–01–20 2121–01–21

# Sample output 3 ------------------------------------------------------------------------------------

2121–01–10

# Explanation of Sample Output ------------------------------------------------------------------------------------

First test case — omitted

Second test case, the total number of room nights per day is
2 on 2121–01–07
2 on 2121–01–08
0 on 2121–01–09
Hence, the earliest busiest day is 2121–01–07 because it is the earliest date with the highest total number of room nights

Third test case — omitted
