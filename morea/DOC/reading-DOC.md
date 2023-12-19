---
title: "Purpose of Don't Cares"
published: true
morea_id: reading-DOC
morea_summary: "Using Don't Cares can simplify the equations used to later design your circuits by allowing more optimized groupings due to Don't Cares ability to be either low or high."
morea_type: reading
morea_labels:
---

# What are Don't Cares?
Don't cares mean that you "do not care" about the output given certain inputs.

The scenarios that you would use Don't Cares for varies depending on the problems.

For example, if a battery of 12 volts uses 4 bits and the  voltage battery is greater than 6, the output is High. Otherwise, it is low. 

In a 4 bit truth table, it goes all the way from 0-15 rows. But if the voltage battery only goes up to 12, then the output for the rows after the max voltage don't matter. While you can write the output for these rows as high, you can use a Don't Care to show that these outputs do not affect the circuit. 

To denote a Don't Care, simply use "X" as the symbol.

When written in a Kmap, Don't Cares can be grouped with either 0 or 1 to form larger, more optimized groupings. But they don't have to all be grouped as it does not actually affect the circuit.  

![Example of Don't Cares in a Kmap.](/morea/DOC/DOCinKmapEx.png)
