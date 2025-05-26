                                                                                      DIGITAL ELECTRONICS
# Table of Contents

-  [What is Digital Electronics](#What-is-Digital-Electronics) 
-  [Applications of Digital Electronics](#Applications-of-Digital-Electronics)
-  [Digital vs Analog Signals](#Digital-vs-Analog-Signals)
-  [Number Systems](#Number-Systems)
-  [Conversion between Number System](#Conversion-between-Number-System)
-  [Basic Logic Gates](#Basic-Logic-Gates)
-  [Integrated Circuits-Ic's](#Integrated-Circuits-Ic's)
-  [Implementation of Logic Gates](#Implementation-of-Logic-Gates)
-  [Implementation of Half Adder](#Implementation-of-Half-Adder)

  
# What is Digital Electronics
Digital electronics is a branch of electronics that deals with systems that use discrete (distinct) signal levels, typically represented by binary numbers — 0 and 1. Unlike analog electronics, where signals can vary smoothly across a range of values, digital electronics processes information using only two states (usually referred to as LOW and HIGH, or OFF and ON).

These two states are typically represented by:

0 → low voltage (e.g., 0 volts)

1 → high voltage (e.g., 5 volts or 3.3 volts)

# Applications of Digital Electronics





1. Communication Systems


2. Mobile phones and Tablets


3. Automotive Industry


4. Medical and Healthcare Devices


5. Industrial Automation and Robotics


6. Military and Aerospace


7. Automobiles


8. Banking, Security, and E-commerce

# Digital vs Analog Signals
|  ASPECT | DIGITAL SIGNAL | ANALOG SIGNAL|
|----------|----------|----------|
| Nature | Discrete   | Continuous
| Signal Representation |  Square waves | Sine waves (or continuous waveforms)|
|  Values| Finite set of values (typically 2: 0 and 1) | Infinite possible values within range|
| Transmission | Difficult over long distances | Easy and accurate over long distances   |
|Devices| Computers, digital watches, microcontrollers | Microphones, speakers, analog radios | | Data Processing | Easier and more precise | More complex and less precise |            
| Examples | Computer data, digital telephony  | Audio signals, temperature sensors |
# LOGIC LEVELS
In digital electronics, logic levels refer to the specific voltage ranges that represent binary states — typically 0 (LOW) and 1 (HIGH). These levels indicate how the digital system interprets voltages as logical TRUE (1) or FALSE (0).
| Logic Level | Binary State | Typical Voltage (TTL)* | Typical Voltage (CMOS)* |
|-------------|--------------|------------------------|-------------------------|
| LOW         | 0            | 0 V to 0.8 V           | 0 V to ~1/3 Vdd         |
| HIGH        | 1            | 2 V to 5 V             | ~2/3 Vdd to Vdd         |
* TTL = Transistor-Transistor Logic (usually Vcc = 5V)
* CMOS = Complementary Metal-Oxide-Semiconductor
# NUMBER SYSTEM
A number system is a way to represent and express numbers using a set of symbols or digits. In digital electronics, number systems are used to represent data and perform calculations inside digital circuits and computers.

# Different number systems are BINARY, OCTAL,DECIMAL, HEXADECIMAL
| Number System | Base | Digits Used              | Key Point | Example |
|---------------|------|--------------------------|-----------|---------|
| Binary        | 2    | 0, 1                     | Fundamental for all digital circuits and computers; data is processed in bits (0s & 1s). | 1011₂ ( = 11 in decimal ) |
| Octal         | 8    | 0-7                      | Compact representation of binary; often used in older computer systems and some embedded systems. | 745₈ ( = 493 in decimal ) |
| Decimal       | 10   | 0-9                      | Natural number system used by humans; common for input/output display. | 259₁₀ |
| Hexadecimal   | 16   | 0-9, A-F (A=10 ... F=15) | Compact representation of binary; widely used in programming, memory addressing. | 3F₁₆ ( = 63 in decimal ) |
# Conversion between number system
### 1. Binary → Decimal  
Binary: 1011₂

= (1×2³) + (0×2²) + (1×2¹) + (1×2⁰)  
= 8 + 0 + 2 + 1  
= **11₁₀**

--------

### 2. Decimal → Binary  
Decimal: 13₁₀

13 ÷ 2 = 6 remainder **1**  
6 ÷ 2 = 3 remainder **0**  
3 ÷ 2 = 1 remainder **1**  
1 ÷ 2 = 0 remainder **1**

Read remainders bottom to top → **1101₂**

---

### 3. Binary → Octal  
Binary: 110110₂

Group in 3 bits → **110** | **110**  
110₂ = 6₈  
110₂ = 6₈

Result → **66₈**

---

### 4. Octal → Binary  
Octal: 57₈

5₈ → **101₂**  
7₈ → **111₂**

Result → **101111₂**

---

### 5. Binary → Hexadecimal  
Binary: 10101110₂

Group in 4 bits → **1010** | **1110**  
1010₂ = A₁₆  
1110₂ = E₁₆

Result → **AE₁₆**

---

### 6. Hexadecimal → Binary  
Hex: 3F₁₆

3₁₆ → **0011₂**  
F₁₆ → **1111₂**

Result → **00111111₂**

---

### 7. Decimal → Octal  
Decimal: 125₁₀

125 ÷ 8 = 15 remainder **5**  
15 ÷ 8 = 1 remainder **7**  
1 ÷ 8 = 0 remainder **1**

Read remainders bottom to top → **175₈**

---

### 8. Octal → Decimal  
Octal: 745₈

= (7×8²) + (4×8¹) + (5×8⁰)  
= (7×64) + (4×8) + (5×1)  
= 448 + 32 + 5  
= **485₁₀**

---

### 9. Decimal → Hexadecimal  
Decimal: 254₁₀

254 ÷ 16 = 15 remainder **14 (E)**  
15 ÷ 16 = 0 remainder **15 (F)**

Read remainders bottom to top → **FE₁₆**

---

### 10. Hexadecimal → Decimal  
Hex: 2A₁₆

= (2×16¹) + (A×16⁰)  
= (2×16) + (10×1)  
= 32 + 10  
= **42₁₀**

---

### 11. Octal → Hexadecimal  
Octal: 745₈

Step 1: Octal → Binary  
7 → **111**  
4 → **100**  
5 → **101**  
Binary = **111100101₂**

Step 2: Binary → Hex  
Group 4 bits: **0011** | **1100** | **101** (pad left 0 → 0101)  
0011 → 3  
1100 → C  
0101 → 5

Result → **3C5₁₆**

---

### 12. Hexadecimal → Octal  
Hex: 2F₁₆

Step 1: Hex → Binary  
2 → **0010**  
F → **1111**  
Binary = **00101111₂**

Step 2: Binary → Octal  
Group 3 bits: **000** | **101** | **111**  
000 → 0  
101 → 5  
111 → 7

Result → **057₈**
------------------------------------------------
# BASIC LOGIC GATES
# 1.AND GATE
# Symbol: 
![image](https://github.com/user-attachments/assets/dece6c82-9d25-4ffd-ba99-19ff4d517094)

A curved-shaped gate with two inputs and one output.
# Function:
The AND gate outputs 1 (true) only when both inputs are 1.  Otherwise, it outputs 0.

- A.B=X.
- The value of X will be True when both the inputs will be True.
# Truth Table
| INP A | INP  B | OUTPUT Y|
|---|---|---------|
| 0 | 0 |    0    |
| 0 | 1 |    0    |
| 1 | 0 |    0    |
| 1 | 1 |    1    |
----------------------------------------------
# 2. OR GATE
# Symbol:
![image](https://github.com/user-attachments/assets/f28a85ff-f485-4797-9208-147a4ccc13fd)

A curved-shaped gate with two inputs and one output.
# Function:
The OR gate outputs 1 (true) if at least one  input  is  1.
- It outputs 0 only when both inputs are 0.
# Truth Table
|INP A | INP B | OUTPUT Y |
|---|---|--------|
| 0 | 0 |   0    |
| 0 | 1 |   1    |
| 1 | 0 |   1    |
| 1 | 1 |   1    |
----------------------------------------------------
# 3. NOT GATE
# Symbol:
![image](https://github.com/user-attachments/assets/3480276f-2c3a-44c8-9679-c2a2c5025db2)

The NOT gate symbol represents a digital logic inverter, and it is visually distinct from other logic gates. It typically consists of:

- A triangle pointing to the right

- A small circle (called a "bubble") at the output, which indicates inversion
# Function : 
The output Y is the negation of the input A, respresented as, Y =  Ā 
Returns 1, if the input is 0.
Returns 0, if the input is 1.
# Truth table : 
| INP A| OUTPUT Y |
|-------|--------|
|   0   |   1    |
|   1   |   0    |
-------------------------------------------------
# 4.NAND GATE
# Symbol: 
![image](https://github.com/user-attachments/assets/32766c05-987f-4de2-92b0-d144c72abf21)
# Function : 
A NAND (Not AND) gate gives an output of 0 only when both inputs are 1. 
- It is the inverse of the AND gate.
# Truth Table

| INP A | INP B | OUTPUT Y|
|---|---|--------------|
| 0 | 0 |      1       |
| 0 | 1 |      1       |
| 1 | 0 |      1       |
| 1 | 1 |      0       |
---------------------------------
# 5.NOR GATE
# Symbol : 
![image](https://github.com/user-attachments/assets/788f5889-9200-4f3e-ad64-44335ca412f4)
# Function : 
A NOR (Not OR) gate gives an output of 1 only when both inputs are 0. 
- It is the inverse of the OR gate.
# Truth Table : 

| INP A | INP B | OUTPUT Y|
|---|---|--------------|
| 0 | 0 |      1       |
| 0 | 1 |      0       |
| 1 | 0 |      0       |
| 1 | 1 |      0       |
----------------------------------------------
# 6. XOR GATE
# Symbol : 
![image](https://github.com/user-attachments/assets/78b2e40f-0922-4638-b52c-06d1429d82a3)
# Function : 
The XOR (Exclusive OR) gate gives an output of 1 only when the inputs are different.

- Boolean Expression : Y = A ⊕ B = A̅·B + A·B̅

# Truth Table : 

| INP A | INP  B | OUTPUT Y |
|---|---|------------|
| 0 | 0 |     0      |
| 0 | 1 |     1      |
| 1 | 0 |     1      |
| 1 | 1 |     0      |
--------------------------------------------------
# 7. XNOR GATE : 
# Symbol : 
![image](https://github.com/user-attachments/assets/426f91b1-d20e-450e-bad5-f53eaf0635b9)
# Function : 
The XNOR (Exclusive NOR) gate gives an output of 1 only when the inputs are the same.

- Boolean Expression : Y = (A ⊕ B)̅ = A·B + A̅·B̅
# Truth Table : 

| INP A |  INP B | OUTPUT Y|
|---|---|---------------|
| 0 | 0 |       1       |
| 0 | 1 |       0       |
| 1 | 0 |       0       |
| 1 | 1 |       1       |
-----------------------------------------------------
# Integrated Circuits(Ic's)
# What is an Ic?
- IC (Integrated Circuit) – A microelectronic device that integrates multiple electronic components into a single chip to perform a specific function or set of functions.
# Types of Logic Gates and Their ICs
### Logic Gate IC Table

| Logic Gate | IC Number | Description                  | Number of Gates | Pin Count |
|------------|-----------|------------------------------|-----------------|-----------|
| NOT        | 7404      | Hex Inverter                 | 6               | 14        |
| AND        | 7408      | Quad 2-Input AND Gate        | 4               | 14        |
| NAND       | 7400      | Quad 2-Input NAND Gate       | 4               | 14        |
| OR         | 7432      | Quad 2-Input OR Gate         | 4               | 14        |
| NOR        | 7402      | Quad 2-Input NOR Gate        | 4               | 14        |
| XOR        | 7486      | Quad 2-Input XOR Gate        | 4               | 14        |
| XNOR       | 74266     | Quad 2-Input XNOR Gate       | 4               | 14        |
---------------------------------------------
  # Applications of IC's
| Logic Gate | IC Number | Applications                                                              | Number of Gates | Pin Count |
|------------|-----------|---------------------------------------------------------------------|-----------------|-----------|
| NOT        | 7404      | Signal inversion, pulse shaping, oscillator circuits                      | 6               | 14        |
| AND        | 7408      | Digital control systems, enable circuits, logic comparisons               | 4               | 14        |
| NAND       | 7400      | Alarm systems, combinational logic design, universal gate implementation  | 4               | 14        |
| OR         | 7432      | Data selection, address decoding, control logic                           | 4               | 14        |
| NOR        | 7402      | Timing circuits, reset logic, universal gate applications                 | 4               | 14        |
| XOR        | 7486      | Arithmetic circuits (adders), parity checkers, digital comparators        | 4               | 14        |
| XNOR       | 74266     | Equality checkers, error detection, phase detectors                       | 4               | 14        |

# 1.IC 7408 – Quad 2-Input AND Gate
![image](https://github.com/user-attachments/assets/45aee511-1515-4439-b4e1-4f886250f4a1)

![image](https://github.com/user-attachments/assets/5efd3b5d-e367-4872-a328-f8b7948c90db)

### 🔸 AND Gate using IC 7408



👉 [Open in Tinkercad](https://www.tinkercad.com/things/6HdIkZViZFl-and-gate-ic-7408)


| Pin | Label | Direction | Function         |
|-----|--------|-----------|------------------|
| 1   | 1A     | Input     | Gate 1 input A   |
| 2   | 1B     | Input     | Gate 1 input B   |
| 3   | 1Y     | Output    | Gate 1 output    |
| 4   | 2A     | Input     | Gate 2 input A   |
| 5   | 2B     | Input     | Gate 2 input B   |
| 6   | 2Y     | Output    | Gate 2 output    |
| 7   | GND    | —         | Ground           |
| 8   | 3Y     | Output    | Gate 3 output    |
| 9   | 3A     | Input     | Gate 3 input A   |
| 10  | 3B     | Input     | Gate 3 input B   |
| 11  | 4Y     | Output    | Gate 4 output    |
| 12  | 4A     | Input     | Gate 4 input A   |
| 13  | 4B     | Input     | Gate 4 input B   |
| 14  | Vcc    | —         | +5V Power Supply |

Description:

- Contains 4 AND gates.

- Each AND gate outputs HIGH only if both inputs are HIGH.

- Power: Pin 14 (Vcc), Ground: Pin 7.
----------------------------------------------
# 2. IC 7432 – Quad 2-Input OR Gate
![image](https://github.com/user-attachments/assets/c7a91fb3-7d3a-4f40-b5b4-b2173fdfdd41)

![image](https://github.com/user-attachments/assets/0b529e47-8422-421c-b7f6-0f99d7b36bc6)



### 🔸 OR Gate using IC 7432



👉 [Open OR Gate Circuit in Tinkercad](https://www.tinkercad.com/things/c17sYaTdDOo-or-gate-ic-7432)


| Pin | Label | Direction | Function         |
|-----|--------|-----------|------------------|
| 1   | 1A     | Input     | Gate 1 input A   |
| 2   | 1B     | Input     | Gate 1 input B   |
| 3   | 1Y     | Output    | Gate 1 output    |
| 4   | 2A     | Input     | Gate 2 input A   |
| 5   | 2B     | Input     | Gate 2 input B   |
| 6   | 2Y     | Output    | Gate 2 output    |
| 7   | GND    | —         | Ground           |
| 8   | 3Y     | Output    | Gate 3 output    |
| 9   | 3A     | Input     | Gate 3 input A   |
| 10  | 3B     | Input     | Gate 3 input B   |
| 11  | 4Y     | Output    | Gate 4 output    |
| 12  | 4A     | Input     | Gate 4 input A   |
| 13  | 4B     | Input     | Gate 4 input B   |
| 14  | Vcc    | —         | +5V Power Supply |


Description:

- Features 4 OR gates.

- Each gate gives a HIGH output when at least one input is HIGH.

- Power supply on Pin 14, Ground on Pin 7.
---------------------------------------------------------------------------
# 3. IC 7404 – Hex Inverter (NOT Gate)
![image](https://github.com/user-attachments/assets/3b30e215-e5e4-4324-8286-a39debbb4f89)

![image](https://github.com/user-attachments/assets/2332a6a8-8492-493d-836d-f3b40a570025)


### 🔸 NOT Gate using IC 7404  
👉 [Open NOT GATE in Tinkercad](https://www.tinkercad.com/things/4CX1sjaLXq8-not-gate-ic-7404a)


| Pin | Label | Direction | Function           |
|-----|--------|-----------|--------------------|
| 1   | 1A     | Input     | Inverter 1 input   |
| 2   | 1Y     | Output    | Inverter 1 output  |
| 3   | 2A     | Input     | Inverter 2 input   |
| 4   | 2Y     | Output    | Inverter 2 output  |
| 5   | 3A     | Input     | Inverter 3 input   |
| 6   | 3Y     | Output    | Inverter 3 output  |
| 7   | GND    | —         | Ground             |
| 8   | 4Y     | Output    | Inverter 4 output  |
| 9   | 4A     | Input     | Inverter 4 input   |
| 10  | 5Y     | Output    | Inverter 5 output  |
| 11  | 5A     | Input     | Inverter 5 input   |
| 12  | 6Y     | Output    | Inverter 6 output  |
| 13  | 6A     | Input     | Inverter 6 input   |
| 14  | Vcc    | —         | +5V Power Supply   |

Description:

- Has 6 NOT gates (inverters).

- Each gate has 1 input and 1 output.

- Used to invert a digital signal.

- Vcc and GND are on Pins 14 and 7 respectively.
----------------------------------------------------------------------
# 4. IC 7400 – Quad 2-Input NAND Gate
![image](https://github.com/user-attachments/assets/abae2531-623d-43d1-adbc-73efa6e21c35)

![image](https://github.com/user-attachments/assets/9cc191db-7759-436f-b26c-52c495a567c1)



### 🔹 NAND Gate using IC 7400  
👉 [Open in Tinkercad](https://www.tinkercad.com/things/89AgKOYdJ2J-nand-gate-ic-7400)



| Pin | Label | Direction | Function         |
|-----|--------|-----------|------------------|
| 1   | 1A     | Input     | Gate 1 input A   |
| 2   | 1B     | Input     | Gate 1 input B   |
| 3   | 1Y     | Output    | Gate 1 output    |
| 4   | 2A     | Input     | Gate 2 input A   |
| 5   | 2B     | Input     | Gate 2 input B   |
| 6   | 2Y     | Output    | Gate 2 output    |
| 7   | GND    | —         | Ground           |
| 8   | 3Y     | Output    | Gate 3 output    |
| 9   | 3A     | Input     | Gate 3 input A   |
| 10  | 3B     | Input     | Gate 3 input B   |
| 11  | 4Y     | Output    | Gate 4 output    |
| 12  | 4A     | Input     | Gate 4 input A   |
| 13  | 4B     | Input     | Gate 4 input B   |
| 14  | Vcc    | —         | +5V Power Supply |


Description:

- Contains 4 NAND gates, each with 2 inputs (A & B) and 1 output (Y).

- Pins 1-6 & 8-13 are logic gate inputs and outputs.

- Pin 14 is for power supply (Vcc = +5V), and Pin 7 is for Ground.
------------------------------------------------------------------------------
  
# 5. IC 7402 – Quad 2-Input NOR Gate
![image](https://github.com/user-attachments/assets/93787e33-8b3b-4980-9982-b575e4a2af11)


![image](https://github.com/user-attachments/assets/5a9d3247-d4db-41bd-b27c-09bd360e1fa4)


### 🔹 NOR Gate using IC 7402  
👉 [Open in Tinkercad](https://www.tinkercad.com/things/3KaIfRwXhun-nor-gate-ic-7402)


| Pin | Label | Direction | Function         |
|-----|--------|-----------|------------------|
| 1   | 1A     | Input     | Gate 1 input A   |
| 2   | 1B     | Input     | Gate 1 input B   |
| 3   | 1Y     | Output    | Gate 1 output    |
| 4   | 2A     | Input     | Gate 2 input A   |
| 5   | 2B     | Input     | Gate 2 input B   |
| 6   | 2Y     | Output    | Gate 2 output    |
| 7   | GND    | —         | Ground           |
| 8   | 3Y     | Output    | Gate 3 output    |
| 9   | 3A     | Input     | Gate 3 input A   |
| 10  | 3B     | Input     | Gate 3 input B   |
| 11  | 4Y     | Output    | Gate 4 output    |
| 12  | 4A     | Input     | Gate 4 input A   |
| 13  | 4B     | Input     | Gate 4 input B   |
| 14  | Vcc    | —         | +5V Power Supply |


Description:

- Includes 4 independent NOR gates.

- Each gate takes 2 inputs and gives 1 output based on NOR logic.

- Pin 14 supplies power; Pin 7 connects to ground.
--------------------------------------------------------------------------------
# 6. IC 7486 – Quad 2-Input XOR Gate
![image](https://github.com/user-attachments/assets/0108f188-5c14-4b4e-abda-4daf1efb4fc1)

![image](https://github.com/user-attachments/assets/0ed28f26-279e-47d3-b9fe-3ca86e3d8c0a)

### 🔹 XOR Gate using IC 7486  
👉 [Open in Tinkercad](https://www.tinkercad.com/things/dVM7spCgh4L-xor-gate-ic-7486)




| Pin | Label | Direction | Function         |
|-----|--------|-----------|------------------|
| 1   | 1A     | Input     | Gate 1 input A   |
| 2   | 1B     | Input     | Gate 1 input B   |
| 3   | 1Y     | Output    | Gate 1 output    |
| 4   | 2A     | Input     | Gate 2 input A   |
| 5   | 2B     | Input     | Gate 2 input B   |
| 6   | 2Y     | Output    | Gate 2 output    |
| 7   | GND    | —         | Ground           |
| 8   | 3Y     | Output    | Gate 3 output    |
| 9   | 3A     | Input     | Gate 3 input A   |
| 10  | 3B     | Input     | Gate 3 input B   |
| 11  | 4Y     | Output    | Gate 4 output    |
| 12  | 4A     | Input     | Gate 4 input A   |
| 13  | 4B     | Input     | Gate 4 input B   |
| 14  | Vcc    | —         | +5V Power Supply |


Description:

- Has 4 XOR gates.

- Output is HIGH when only one input is HIGH.

- Commonly used in adders and parity checkers.
--------------------------------------------------------
 # 7.  IC 74266 – Quad 2-Input XNOR Gate
 ![image](https://github.com/user-attachments/assets/42dd988e-525d-4f70-b67b-4b3a37b793e2)

 ![image](https://github.com/user-attachments/assets/0cb6999c-f562-48aa-a446-b5be1b561c78)

 ### 🔹 XNOR Gate  
👉 [Open in Tinkercad](https://www.tinkercad.com/things/foLhOr8GhDX-xnor-gate)



 | Pin | Label | Direction | Function              |
|-----|--------|-----------|-----------------------|
| 1   | 1A     | Input     | Gate 1 input A        |
| 2   | 1B     | Input     | Gate 1 input B        |
| 3   | 1Y     | Output    | Gate 1 output         |
| 4   | 2A     | Input     | Gate 2 input A        |
| 5   | 2B     | Input     | Gate 2 input B        |
| 6   | 2Y     | Output    | Gate 2 output         |
| 7   | GND    | —         | Ground                |
| 8   | 3Y     | Output    | Gate 3 output         |
| 9   | 3A     | Input     | Gate 3 input A        |
| 10  | 3B     | Input     | Gate 3 input B        |
| 11  | 4Y     | Output    | Gate 4 output         |
| 12  | 4A     | Input     | Gate 4 input A        |
| 13  | 4B     | Input     | Gate 4 input B        |
| 14  | Vcc    | —         | +5V Power Supply      |

  Description:

- Implements 4 XNOR gates with open-collector outputs (requires pull-up resistor).

- Output is HIGH when inputs are the same.

- Special use in equality checking circuits.
----------------------------------------------------------------------


## IMPLEMENTATION OF LOGIC GATES

 IMPLEMENTATION OF AND GATE USING NAND GATE 7400
 
![image](https://github.com/user-attachments/assets/dc20e6cf-d5bc-4c5b-a14b-463b782abd9f)

 Tinkercad Project Link

👉 [View  AND GATE USING NAND Gate 7400  Project on Tinkercad](https://www.tinkercad.com/things/5QLXe5UlPai-and-using-nand)

-----------------------------------
IMPLEMENTATION OF OR GATE  USING NAND GATE 7400

![image](https://github.com/user-attachments/assets/e912b171-a7f1-4739-9aab-3156317bcd2e)


Tinkercad Project Link:

👉 [View  OR GATE USING NAND GATE 7400 Circuit on Tinkercad](https://www.tinkercad.com/things/i38juEEBKzw-or-using-nand)

-------------------------------------
 IMPLEMENTATION OF NOT GATE USING NAND GATE 7400

![image](https://github.com/user-attachments/assets/e581f8f1-bded-499c-a4bd-e2964cd17cc0)


 Tinkercad Project Link :
  
👉 [View NOT GATE USING NAND 7400](https://www.tinkercad.com/things/a9MY7WZkC7Q-not-gate-using-nand)

-----------------------------------------------
 IMPLEMENTATION OF AND GATE USING NOR GATE 7402

 ![image](https://github.com/user-attachments/assets/cce5f8b9-3921-424e-9f51-db751d8bd1a9)

Tinkercad Project Link:

👉[View AND GATE USING NOR 7402](https://www.tinkercad.com/things/6ExuAsd1Ohq-and-gate-using-nor-7402)
 
 -------------------------------------
 
IMPLEMENTATION OF OR GATE USING NOR GATE 7402

![image](https://github.com/user-attachments/assets/6b37dcab-1ac6-4ed7-a929-f16a2ba25b63)

 Tinkercad Project Link:
 
👉[View OR GATE USING NOR 7402](https://www.tinkercad.com/things/hlNbfl7z4OF-or-gate-using-nor-7402)

--------------------------------------------
IMPLEMENTATION OF NOT GATE USING NOR GATE 7402

![image](https://github.com/user-attachments/assets/8f5cb303-badd-4985-b53f-52269f24e7ee)

Tinkercad Project Link:

👉 [View NOT GATE USING NOR GATE 7402](https://www.tinkercad.com/things/gHPBkiHX2zU-not-gate-using-nor-gate-7402)

------------------------------------------------------------------------
# Implementation of Half Adder
  
  ![image](https://github.com/user-attachments/assets/6a7d9236-cb01-46f3-b07e-b88bf0b4440b)

  ![image](https://github.com/user-attachments/assets/74004944-d3af-40c7-bf36-479b88b12770)

  ### Half Adder using 7400 NAND IC — Pin-to-Pin Connection Table

| S.No | From Pin         | To Pin              | Comment                               |
|------|------------------|---------------------|---------------------------------------|
| 1    | Pin 1            | Input A (Switch)    | First input to NAND1                  |
| 2    | Pin 2            | Input B (Switch)    | Second input to NAND1                 |
| 3    | Pin 3            | Pin 5               | Output of NAND1 → input of NAND2      |
| 4    | Pin 3            | Pin 10              | Output of NAND1 → input of NAND3      |
| 5    | Pin 4            | Input A (Switch)    | A again for NAND2                     |
| 6    | Pin 6            | Pin 12              | Output of NAND2 → input of NAND4      |
| 7    | Pin 9            | Input B (Switch)    | B again for NAND3                     |
| 8    | Pin 8            | Pin 13              | Output of NAND3 → input of NAND4      |
| 9    | Pin 11           | LED (Sum Output)    | Final XOR (SUM) output                |
| 10   | Pin 3            | Pin 1 (2nd IC)      | NAND1 output → both inputs of NAND5   |
| 11   | Pin 3            | Pin 2 (2nd IC)      | For Generating Carry                  |
| 12   | Pin 3 (2nd IC)   | LED (Carry Output)  | Output of NAND5 = CARRY               |
| 13   | Pin 14           | +5V                 | Power (VCC)                           |
| 14   | Pin 7            | GND                 | Ground                                |


Outputs:

- Sum → Pin 11
- Carry → Pin 3 of second 7400 IC (NAND5 output)
  
-  Half Adder Truth Table

| A | B | Sum | Carry |
|---|---|-----|-------|
| 0 | 0 |  0  |   0   |
| 0 | 1 |  1  |   0   |
| 1 | 0 |  1  |   0   |
| 1 | 1 |  0  |   1   |

  - Tinkercad Project Link:

 👉 [Half-Adder using NAND Gates (7400)](https://www.tinkercad.com/things/iq6dWuUZlBf-half-adder-using-nand-gates-7400)

































 



















 











            
