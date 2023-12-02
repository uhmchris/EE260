---
title: "Logic Gates Reading"
published: false
morea_id: r outcome-logic-gates
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
* ![Not_gate](https://github.com/tarynlt/Logic-Gates-Truth-Tables-Min-and-Max-Terms/assets/131204960/26794427-8590-46dd-a203-3776950671bb)
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
* ![And_gate](https://github.com/tarynlt/Logic-Gates-Truth-Tables-Min-and-Max-Terms/assets/131204960/275011a2-0b3e-4883-9d1b-f6161a8de422)

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
* ![Or_gate](https://github.com/tarynlt/Logic-Gates-Truth-Tables-Min-and-Max-Terms/assets/131204960/c639bc22-9e4d-4b04-b39a-ee08efe42006)

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
* ![Nand_gate](https://github.com/tarynlt/Logic-Gates-Truth-Tables-Min-and-Max-Terms/assets/131204960/2e3e354d-9b5c-49bb-9395-2809177d09b8)

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
* ![Nor_gate](https://github.com/tarynlt/Logic-Gates-Truth-Tables-Min-and-Max-Terms/assets/131204960/347af3a3-7375-43b7-a360-779b8d111b57)

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
* ![Xor_gate](https://github.com/tarynlt/Logic-Gates-Truth-Tables-Min-and-Max-Terms/assets/131204960/80c973f7-5ee9-4713-b0e4-7c9c4fa7d21a)

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
* ![Xnor_gate](https://github.com/tarynlt/Logic-Gates-Truth-Tables-Min-and-Max-Terms/assets/131204960/e0625417-ad43-4b38-93db-ae4175a10027)

* Truth table:

    | Input | Output |
    | ----- | ------ |
    |00|1|
    |01|0|
    |10|0|
    |11|1|

* Logic function:
  * (A ⊕ B)'
