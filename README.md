# Political Polarization in Virginia, 2016-2020

I used data from the MIT Election Lab to measure political polarization in Virginia by county. I aggregated precinct-level data to county level to account for absentee ballots, for the 2016, 2018 2020 House and Senate races. I included Independent and Libertarian party candidates but not write-ins. I joined this to data on unemployment (June of each year--not seasonally adjusted) and population (2020) by county from the Census Bureau.

For each county, year and race, I measured political polarization via entropy, as

$$-\sum_i p_i log_2(p_i), i = 1,..N parties$$

Entropy measures the dispersion or complexity of a discrete distribution. For example, in a race where one candidate receives all the votes, entropy is zero. In a two-party race where each gets an equal number of votes, entropy is 1. In a three-party race where each gets one-third of the vote, entropy is about 1.6. Accordingly, entropy is a better measure of dispersion than (say) the difference in Democratic vs Republican votes, as it accounts for third-party votes as well as the concentration of votes in individual parties. 

I also measure the party leaning for each county, year, and race as the share of Democratic votes and use this to color the associated circles on the chart. 

See the interactive visualization [here:](https://charlie-kramer.github.io/va_voting_entropy/)
