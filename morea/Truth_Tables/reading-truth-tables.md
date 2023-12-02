---
title: "Truth Tables Reading"
published: false
morea_id: reading-truth-tables
morea_url: -[Truth_Tables](https://drive.google.com/file/d/1-dkOuaJmtceTfKMli0C3BBkvVauJGEUS/view?usp=sharing)
morea_summary: "A truth table shows every possible input-output combination of a given function. If a logic circuit has n-number of inputs, there will be 2n possible inputs. The typical truth table is a canonical truth table, a truth table in which the binary code inputs are in ascending order. The output(s) of a truth table depends on the circuit; in general, 1 is High and 0 is Low."
morea_type: reading
morea_sort_order: 2
morea_labels:
  - <reading 5>
---
#
### Topics covered
* Textbook summary
* What is a Truth Table
* How to create a Truth Table from a given situation
* How to use a Truth Table


#
### Textbook summary
A truth table shows every possible input-output combination of a given function. If a logic circuit has n-number of inputs, there will be 2n possible inputs. The typical truth table is a canonical truth table, a truth table in which the binary code inputs are in ascending order. The output(s) of a truth table depends on the circuit; in general, 1 is High and 0 is Low. For more information, see page 44 of textbook.

#
### What is a Truth Table

Example Truth Table:

  | Index | Input | Output |
  |-|-|-|
  |       |  ABC  |    F   |
  |0|000|0|
  |1|001|0|
  |2|010|1|
  |3|011|1|
  |4|100|0|
  |5|101|1|
  |6|110|0|
  |7|111|1|

The inputs to a truth table are the binary numbers from 0 to 2<sup>n</sup> where n is the number of inputs. _In the above table, there are 3 inputs (A, B, C) so there are 2<sup>n</sup> or 8 indices._ The outputs of the truth table depend on the function given to us in a problem or based on a gate (see logic gates). _In this truth table, the function is defined as: when A is Low, F = B. When A is High, F = C._

The truth table above is a canonical truth table, meaning the inputs are in increasing order from least to greatest and the 
indices correlate with the decimal number of the corresponding binary number.

#
### How to create a truth table from a given situation:

_A certain logic circuit has 3 inputs (A, B, C) and 1 output (F). When A and B are both Low or both High, F = C. When A is Low and B is High, F = High. Otherwise, F = ~C._

Pretend we are given the above question to solve. How do we create a truth table from a given situation? Start with writing out the canonical truth table.

  |Index|Inputs|Output|
  |-|-|-|
  | |ABC|F|
  |0|000||
  |1|001||
  |2|010||
  |3|011||
  |4|100||
  |5|101||
  |6|110||
  |7|111||

Now that we have written the canonical truth table, we can figure out when F is High (1) and Low (0). The problem tells us F is equal to C when A and B are both Low or both High. From this, we can add to our previous truth table to create the following:

  |Index|Inputs|Output|
  |-|-|-|
  | |ABC|F|
  |0|000|0|
  |1|001|1|
  |2|010||
  |3|011||
  |4|100||
  |5|101||
  |6|110|0|
  |7|111|1|

The problem also tells us F is High when A is Low and B is High at the same time. From this, we can create the following:

  |Index|Inputs|Output|
  |-|-|-|
  | |ABC|F|
  |0|000|0|
  |1|001|1|
  |2|010|1|
  |3|011|1|
  |4|100||
  |5|101||
  |6|110|0|
  |7|111|1|

Finally, the problem tells us that in all other situations, F is Not C. Therefore, our final truth table is:

  |Index|Inputs|Output|
  |-|-|-|
  | |ABC|F|
  |0|000|0|
  |1|001|1|
  |2|010|1|
  |3|011|1|
  |4|100|1|
  |5|101|0|
  |6|110|0|
  |7|111|1|

We have finished creating the truth table of the given problem. We can then use this truth table to create the circuit schematic.

#
### How to use a Truth Table

In a future section, Minterms and Maxterms will be discussed. Minterms and Maxterms use a truth table to figure out how to go from the truth table to an actual circuit.

