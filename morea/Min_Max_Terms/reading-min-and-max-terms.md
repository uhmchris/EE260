---
title: "Min and Max Terms Reading"
published: false
morea_id: r outcome-min-and-max-terms
morea_url: -[Minterms_and_Maxterms](https://drive.google.com/file/d/13ykVfLJ93eI178MYQBgNGcVIeeTTjnOO/view?usp=sharing)
morea_summary: "In order to create a circuit schematic from a truth table, a _canonical sum of products (CSOP)_ can be used based on minterms. A minterm can be written at every index but we only care about the minterms when the output is High. To write the minterms of a function, look at the inputs and see what needs to be done to the inputs so the minterm output is High when the inputs are all And-ed together. After doing this at each index, Or all the And gate outputs together to get the output function. To write in a more compact way, a _minterm list_ can be used. Use the “Σ” symbol to denote a minterm list, subscript the input variables, and put the indices of when the output function is High. Another way to create a circuit schematic from a truth table is to use a _canonical product of sums (CPOS)_  and maxterms. A maxterm can be written at every index but we only care about the maxterms when the output is Low. To write the maxterms of a function, look at the inputs and see what needs to be done to the inputs so the maxterm output is Low when the inputs are all Or-ed together. After doing this at each index, And all the Or gate outputs together to get the output function. To write in a more compact way, a _maxterm list_ can be used. Use the “Π” symbol to denote a maxterm list, subscript the input variables, and put the indices of when the output function is Low. For more information, see pages 115 - 121."
morea_type: reading
morea_sort_order: 2
morea_labels:
  - <reading 10>
---

### Topics covered

* Textbook summary
* Minterms
* Maxterms
* Minterm vs Maxterm

#
### Textbook summary

* Minterms
  * In order to create a circuit schematic from a truth table, a _canonical sum of products (CSOP)_ can be used based on minterms. A minterm can be written at every index but we only care about the minterms when the output is High. To write the minterms of a function, look at the inputs and see what needs to be done to the inputs so the minterm output is High when the inputs are all And-ed together. After doing this at each index, Or all the And gate outputs together to get the output function. To write in a more compact way, a _minterm list_ can be used. Use the “Σ” symbol to denote a minterm list, subscript the input variables, and put the indices of when the output function is High. For more information, see pages 115 - 118.

* Maxterms
  * Another way to create a circuit schematic from a truth table is to use a _canonical product of sums (CPOS)_  and maxterms. A maxterm can be written at every index but we only care about the maxterms when the output is Low. To write the maxterms of a function, look at the inputs and see what needs to be done to the inputs so the maxterm output is Low when the inputs are all Or-ed together. After doing this at each index, And all the Or gate outputs together to get the output function. To write in a more compact way, a _maxterm list_ can be used. Use the “Π” symbol to denote a maxterm list, subscript the input variables, and put the indices of when the output function is Low. For more information, see pages 118 - 121.


#
### Minterms

Example Truth Table with Minterms:

|Index|Input|Output|Minterm|
|-|-|-|-|
|     |ABC  |F     |m|
|0|000|0|A'B'C'|
|1|001|0|A'B'C|
|2|010|1|A'BC'|
|3|011|1|A'BC|
|4|100|0|AB'C'|
|5|101|1|AB'C|
|6|110|0|ABC'|
|7|111|1|ABC|

Above is a truth table with all minterms for all indices written out. Notice that when an input is 0, the input variable for the minterm is negated. This is due to how the And gate works: an And gate only outputs a High when all inputs are also High. However, for designing a circuit from the truth table, we only care about the minterms where the output "F" is equal High. Therefore, only the minterms in index 2, 3, 5, and 7 will be used to design the circuit. This can be written out the following way:

  General way: Σ<sub>m</sub>(index numbers) = corresponding minterms

  Specific example: Σ<sub>m</sub>(2, 3, 5, 7) = A'BC' + A'BC + AB'C + ABC

Note that the function is all the sums being added together. This is the reasoning for why Minterms are called Sum of Products. The unsimplification of these is the reason for it being called the canonical sum of products or CSOP.

To create the design for this, there will be three inputs, one Not gate per input, four 3-input And gates, and one 4-input Or gate.



#
### Maxterms

Example Truth Table with Maxterms:

|Index|Input|Output|Maxterm|
|-|-|-|-|
|     |ABC  |F     |M|
|0|000|0|A+B+C|
|1|001|0|A+B+C'|
|2|010|1|A+B'+C|
|3|011|1|A+B'+C'|
|4|100|0|A'+B+C|
|5|101|1|A'+B+C'|
|6|110|0|A'+B'+C|
|7|111|1|A'+B'+C'|

Above is a truth table with all maxterms for all indices written out. Notice that when an input is 1, the input variable for the maxterm is negated. This is due to how the Or gate works: an Or gate only outputs a Low when all inputs are also Low. However, for designing a circuit from the truth table, we only care about the maxterms where the output "F" is equals Low. Therefore, only the maxterms in index 0, 1, 4, and 6 will be used to design the circuit. This can be written out the following way:

  General way: Π<sub>M</sub>(index numbers) = corresponding maxterms

  Specific example: Π<sub>M</sub>(0, 1, 4, 6) = (A+B+C)(A+B+C')(A'+B+C)(A'+B'+C)

Note that the function is all the sums being multiplied together. This is the reasoning for why Maxterms are called Product of Sums. The unsimplification of these is the reason for it being called the canonical product of sums or CPOS.

To create the design for this, there will be three inputs, one Not gate per input, four 3-input Or gates, and one 4-input And gate.


#
### Minterm vs Maxterm

Both minterms and maxterms can be used to create a circuit simulation however, the simpler the circuit, the better. Therefore, usually the option with fewer gates is used. No matter if you use minterms/CSOP or maxterms/CPOS, the output function should be the same.

_Example truth table from above with both Min and Max terms on same table:_

|Index|Input|Output|Minterm|Maxterm|
|-|-|-|-|-|
|     |ABC  |F     |m|M|
|0|000|0||A+B+C|
|1|001|0||A+B+C'|
|2|010|1|A'BC'||
|3|011|1|A'BC||
|4|100|0||A'+B+C|
|5|101|1|AB'C||
|6|110|0||A'+B'+C|
|7|111|1|ABC||

Using the truth table above, the circuit can be designed using either minterms/CSOP or maxterms/CPOS. Link to Falstad with both minterm and maxterm circuits: [https://tinyurl.com/ymdlzsk7]

The following circuit uses minterms/CSOP:

![Minterm_design](https://github.com/tarynlt/Logic-Gates-Truth-Tables-Min-and-Max-Terms/assets/131204960/075ffe05-e5ff-462b-9cf8-c7e50299d534)


The following circuit uses maxterms/CPOS:

![Maxterm_design](https://github.com/tarynlt/Logic-Gates-Truth-Tables-Min-and-Max-Terms/assets/131204960/0a570dbb-b854-439c-ac38-da409df4b8ab)


