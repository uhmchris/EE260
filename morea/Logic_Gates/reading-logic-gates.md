---
title: "Logic Gates Reading"
published: true
morea_id: reading-logic-gates
morea_url:
  -[NOT, AND, OR Gates](https://drive.google.com/file/d/1LCGSKg_Z8hj4HYrpz02kCZ70Hn7khwEs/view?usp=sharing)

  [NAND and NOR Gates](https://drive.google.com/file/d/1phs_aWtJtTNtO4B-ZopXx7hSngGTBPYG/view?usp=sharing)
  
  [XOR and XNOR Gates](https://drive.google.com/file/d/1YWvgWgt46IeqtMxyjuYGFJu3dKomsYzU/view?usp=sharing)
morea_summary: "The logic gates covered in this summary are Not, And, Or, Nand, Nor, Xor, and Xnor. Multiple, combined logic gates can be used to create any given circuit. Each logic gate has its own, unique truth table, circuit symbol, and logic function in Boolean algebra. The standard logic gate has 1-2 inputs and one output but logic gates can have multiple inputs."
morea_type: reading
morea_sort_order: 2
morea_labels:
  - <reading 10>
---

### Topics covered
* Textbook summary
* NOT/Inverter
* AND Gate
* NAND Gate
* OR Gate
* NOR Gate
* XOR Gate
* XNOR Gate


### Textbook summary
The logic gates covered in this summary are Not, And, Or, Nand, Nor, Xor, and Xnor. Multiple, combined logic gates can be used to create any given circuit. Each logic gate has its own, unique truth table, circuit symbol, and logic function in Boolean algebra. The standard logic gate has 1-2 inputs and one output but logic gates can have multiple inputs.


#
### Not gate/Inverter
* Page 46
* ![Not_gate](/morea/Logic_Gates/Not_gate.jpg)
* Truth table:

    | Input | Output |
    | ----- | ------ |
    |   0   |    1   |
    |   1   |    0   |

* Logic function:
  * Ā or A'

 #
### And gate
* Page 46
* ![And_gate](/morea/Logic_Gates/And_gate.jpg)
* Truth table:

    | Input | Output |
    | ----- | ------ |
    |  00   |    0  |
    |  01   |    0   |
    |10|0|
    |11|1|

* Logic function:
  * A ⋅ B or AB

#
### Or gate
* Page 47
* ![Or_gate](/morea/Logic_Gates/Or_gate.jpg)
* Truth table:

    | Input | Output |
    | ----- | ------ |
    |00|0|
    |01|1|
    |10|1|
    |11|1|

* Logic function:
  * A + B


#
### Nand gate
* Page 47
* ![Nand_gate](/morea/Logic_Gates/Nand_gate.jpg)

* Truth table:

    | Input | Output |
    | ----- | ------ |
    |00|1|
    |01|1|
    |10|1|
    |11|0|
* Logic function:
  * (A ⋅ B)' or (AB)'

#
### Nor gate
* Page 47-48
* ![Nor_gate](/morea/Logic_Gates/Nor_gate.jpg)

* Truth table:

    | Input | Output |
    | ----- | ------ |
    |00|1|
    |01|0|
    |10|0|
    |11|0|

* Logic function:
  * (A + B)'

#
### Xor gate
* Page 48-49
* ![Xor_gate](/morea/Logic_Gates/Xor_gate.jpg)

* Truth table:

    | Input | Output |
    | ----- | ------ |
    |00|0|
    |01|1|
    |10|1|
    |11|0|

* Logic function:
  * A ⊕ B

#
### Xnor gate
* Page 49
* ![Xnor_gate](/morea/Logic_Gates/Xnor_gate.jpg)

* Truth table:

    | Input | Output |
    | ----- | ------ |
    |00|1|
    |01|0|
    |10|0|
    |11|1|

* Logic function:
  * (A ⊕ B)'
