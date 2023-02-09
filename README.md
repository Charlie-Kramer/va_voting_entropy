#Political Polarization in Virginia, 2016-2020

I used data from the MIT Election Lab to measure political polarization in Virginia by county. I aggregated precinct-level data to county level to account for absentee ballots, for the 2016, 2018 2020 House and Senate races. I included Independent and Libertarian party candidates but not write-ins. I joined this to data on unemployment and population by county from the Census Bureau.

For each county, year and race, I measured political polarization via entropy, as

$$\sum_i p_i log_2(p_i), i = 1,..N parties$$

Entropy measures the dispersion or complexity of a discrete distribution. For example, in a race where one candidate receives all the votes, entropy is zero. In a two-party race where each gets an equal number of votes, entropy is 
