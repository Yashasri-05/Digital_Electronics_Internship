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
-  [Implementation of Full Adder](#Implementation-of-Full-Adder)
-  [MULTIPLEXERS](#MULTIPLEXERS) 

  
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
| INPUT A | INPUT  B | OUTPUT Y|
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
|INPUT A | INPUT B | OUTPUT Y |
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
| INPUT A| OUTPUT Y |
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

| INPUT A | INPUT B | OUTPUT Y|
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

| INPUT A | INPUT B | OUTPUT Y|
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

| INPUT A | INPUT  B | OUTPUT Y |
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

| INPUT A |  INPUT B | OUTPUT Y|
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

![image](https://github.com/user-attachments/assets/b7d118ec-ce1a-43d8-85dc-b2870a8a99ad)


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

![image](https://github.com/user-attachments/assets/54ad4409-dc42-41f1-8cbb-d1aaddadcbcc)


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

![image](https://github.com/user-attachments/assets/676f0fa4-f4d2-4909-aa72-7c779a049b82)


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

![image](https://github.com/user-attachments/assets/8bdc10be-0188-4768-9bb7-98f6db0cb3e1)


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

![image](https://github.com/user-attachments/assets/6faaf761-690b-44f8-b53c-8becac8ff43c)


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

![image](https://github.com/user-attachments/assets/6b1838c4-27ed-4195-9903-e483144477ff)


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

![image](https://github.com/user-attachments/assets/767afb4b-528d-490f-8086-588c93deacca)

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


 🔹Outputs:

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

 ------------------------------------------------------------
 # Implementation of Full Adder 

 ![image](https://github.com/user-attachments/assets/1ce784e4-5e68-4da9-817b-25b7ebd2078f)

 
 ![image](https://github.com/user-attachments/assets/9aac7e74-b5df-4d28-9e2f-a7afc26e8212)


### Full Adder using 7400 NAND IC — Pin-to-Pin Connection Table

| S.No | From Pin               | To Pin                   | Comment                                           |
|------|------------------------|--------------------------|---------------------------------------------------|
|      | **IC1 – First Half Adder (A, B)**                 |                                                   |                                                   
| 1    | Pin 1 (IC1)            | Input A (Switch)         | First input to NAND1                              |
| 2    | Pin 2 (IC1)            | Input B (Switch)         | Second input to NAND1                             |
| 3    | Pin 3 (IC1)            | Pin 5 (IC1)              | NAND1 output → input of NAND2                     |
| 4    | Pin 3 (IC1)            | Pin 10 (IC1)             | NAND1 output → input of NAND3                     |
| 5    | Pin 4 (IC1)            | Input A (Switch)         | A again → input of NAND2                          |
| 6    | Pin 6 (IC1)            | Pin 12 (IC1)             | NAND2 output → input of NAND4                     |
| 7    | Pin 9 (IC1)            | Input B (Switch)         | B again → input of NAND3                          |
| 8    | Pin 8 (IC1)            | Pin 13 (IC1)             | NAND3 output → input of NAND4                     |
| 9    | Pin 11 (IC1)           | Pin 1 (IC2)              | A⊕B output → input of NAND5 (second half adder)   |
| 10   | Pin 6 (IC1)            | Pin 1 (IC3)              | A.B from NAND2 → input of NAND9 (carry logic)     |
| 11   | Pin 6 (IC1)            | Pin 2 (IC3)              | A.B again → second input of NAND9                 |
|      | **IC2 – Second Half Adder (A⊕B, Cin)**           |                                                   |                                                   
| 12   | Pin 2 (IC2)            | Cin (Switch)             | Cin → input of NAND5                              |
| 13   | Pin 3 (IC2)            | Pin 5 (IC2)              | NAND5 output → input of NAND6                     |
| 14   | Pin 3 (IC2)            | Pin 10 (IC2)             | NAND5 output → input of NAND7                     |
| 15   | Pin 4 (IC2)            | From Pin 11 (IC1)        | A⊕B again → input of NAND6                        |
| 16   | Pin 6 (IC2)            | Pin 12 (IC2)             | NAND6 output → input of NAND8                     |
| 17   | Pin 9 (IC2)            | Cin (Switch)             | Cin again → input of NAND7                        |
| 18   | Pin 8 (IC2)            | Pin 13 (IC2)             | NAND7 output → input of NAND8                     |
| 19   | Pin 11 (IC2)           | LED (Sum Output)         | Final SUM output = (A⊕B)⊕Cin                     |
|      | **IC3 – Carry Logic (A.B + (A⊕B).Cin)**          |                                                   |                                                   
| 20   | Pin 1 (IC3)            | From Pin 6 (IC1)         | A.B input from NAND2                              |
| 21   | Pin 2 (IC3)            | Cin (Switch)             | Cin input for (A⊕B).Cin                           |
| 22   | Pin 3 (IC3)            | Carry LED                | Output = Final Carry                              |
|      | **Power Connections (All ICs)**                   |                                                    |                                                   
| 23   | Pin 14 (IC1, IC2, IC3) | +5V                      | Power Supply                                      |
| 24   | Pin 7 (IC1, IC2, IC3)  | GND                      | Ground                                            |

🔹 Inputs: 
- A, B, Cin (Carry-in)

🔹 Outputs:

- Sum = A ⊕ B ⊕ Cin

- Carry = (A · B) + (B · Cin) + (A · Cin)
  
- Tinkercad Project Link:

👉 [View on Tinkercad](https://www.tinkercad.com/things/0fPT0lMxoBd-full-addaer-using-nand-gates-7400)

--------------------------------------------------------------------------
# MULTIPLEXERS 

# 📘 What is a Multiplexer?

A multiplexer (MUX) is a combinational logic circuit that selects one input from multiple data inputs and forwards it to a single output line, based on control signals known as select lines.
- A multiplexer with n select lines can handle 2ⁿ input lines.
  
➤ **Key Features**:
- Acts like a digital switch
- Reduces number of data lines
- Common in communication systems and data routing
  
➤ **Types of multiplexers (MUX)** 

| **Type of MUX** | **Number of Inputs** | **Select Lines** | **Output Lines** | **Selection Capacity**           |
|-----------------|----------------------|------------------|------------------|----------------------------------|
| 2x1 MUX         | 2                    | 1                | 1                | Selects 1 out of 2 inputs        |
| 4x1 MUX         | 4                    | 2                | 1                | Selects 1 out of 4 inputs        |
| 8x1 MUX         | 8                    | 3                | 1                | Selects 1 out of 8 inputs        |
| 16x1 MUX        | 16                   | 4                | 1                | Selects 1 out of 16 inputs       |
| 32x1 MUX        | 32                   | 5                | 1                | Selects 1 out of 32 inputs       |

# 1. 2x1 Multiplexer

![image](https://github.com/user-attachments/assets/648908d8-77aa-4e59-b6a9-4a3397b66b55)

 ➤  **Definition**:

A 2x1 multiplexer (MUX) is a combinational logic circuit that selects one of two input data lines and forwards the selected input to a single output line, based on the value of a control signal (also called a select line).

➤   **Working Principle**:

The output of the 2x1 Mux will depend on the selection line S0,

- When S is 0(low), the I0 is selected
  
- When S0 is 1(High), I1 is selected

  


➤  **How Logic Gates Work Behind the Scenes**:

1.NOT gate inverts S → gives S̅

2.AND gate 1: S̅ · I0 (passes I0 when S = 0)

3.AND gate 2: S · I1 (passes I1 when S = 1)

4.OR gate: Combines both → Output Y = S̅·I0 + S·I1

➤  **Applications of 2x1 MUX**:

- Selects between two data inputs.

- Used in ALUs for operation control.

- Switches signals in communication systems.

- Controls data paths in processors.

- Implements basic logic functions.



![image](https://github.com/user-attachments/assets/a73fa015-7c86-4898-a4f8-478a73c9f28b)

➤   **2x1 Multiplexer Truth Table**:

| **Select Line (S)** | **Input I0** | **Input I1** | **Output (Y)** |
|---------------------|--------------|--------------|----------------|
| 0                   | 0            | X (don’t care) | 0             |
| 0                   | 1            | X             | 1              |
| 1                   | X            | 0             | 0              |
| 1                   | X            | 1             | 1              |

➤  **Explanation**:
- When S = 0, the output Y = I0

- When S = 1, the output Y = I1

- X means "don’t care" because that input is not selected
  
➤  **Pin-to-Pin Connection Table of 2x1 Multiplexer:**

| **Connection**         | **From IC (Pin)**         | **To IC (Pin)**                                | **Comment**                      |
|------------------------------|---------------------------|------------------------------------------|--------------------------------------|
| **VCC** (+5V)                | 7408 (Pin 14)             | VCC                                      | Power for AND gates                  |
|                              | 7432 (Pin 14)             | VCC                                      | Power for OR gate                    |
|                              | 7404 (Pin 14)             | VCC                                      | Power for NOT gate                   |
| **GND**                      | 7408 (Pin 7)              | GND                                      | Ground for AND gates                 |
|                              | 7432 (Pin 7)              | GND                                      | Ground for OR gate                   |
|                              | 7404 (Pin 7)              | GND                                      | Ground for NOT gate                  |
| **Select input (S)**         | Input Switch              | 7404 (Pin 1)                             | S to NOT gate input                  |
| **S̅ (NOT S)**               | 7404 (Pin 2)              | 7408 (Pin 2)                              | NOT S to AND gate 1 input B         |
| **Data input I0**            | Input Switch              | 7408 (Pin 1)                             | I0 to AND gate 1 input A            |
| **Data input I1**            | Input Switch              | 7408 (Pin 4)                              | I1 to AND gate 2 input A            |
| **Select input S**           | Same as above (S)         | 7408 (Pin 5)                              | S to AND gate 2 input B             |
| **Output A (I0 · S̅)**       | 7408 (Pin 3)              | 7432 (Pin 1)                              | Output of AND1 to OR input A        |
| **Output B (I1 · S)**        | 7408 (Pin 6)              | 7432 (Pin 2)                              | Output of AND2 to OR input B        |
| **Final Output (Y)**         | 7432 (Pin 3)              | Output LED or test pin                   | Final MUX output                     |


 **Tinkercad Project Link**:

👉 [View on Tinkercad](https://www.tinkercad.com/things/iDWR7VYfuA9-21-multiplexer)

-------------------------------------------
# 2. 4x1 Multiplexer

![image](https://github.com/user-attachments/assets/b0b30200-6745-4fe4-bc34-daeccda750d9)

➤  **Definition**:

A 4x1 multiplexer is a digital device that selects one of four input lines (I0–I3) and routes it to a single output (Y) based on the combination of two select lines (S1 and S0).

➤ **Logic Expression:** Y = S̅1·S̅0·I0 + S̅1·S0·I1 + S1·S̅0·I2 + S1·S0·I3

➤ **ICs Used to Build 4x1 MUX Using Logic Gates**

| **IC**    | **Function**       | **Details**                           |
|-----------|--------------------|--------------------------------       |
| 7408 - 2     | AND gate (quad 3-input) | Used for input selection logic |
| 7432 - 1     | OR gate (quad 2-input)  | Combines outputs of AND gates  |
| 7404 - 1    | NOT gate (hex inverter)| Inverts select lines           |

➤  **Working Principle:**

- The select lines (S1 and S0) determine which one of the four inputs (I0–I3) is passed to the output (Y).

- Logic gates (AND, OR, NOT) are used to enable only the selected input.

- Only one input line is active at a time, based on the select line combination.

➤   **Applications of 4x1 MUX:**

- Data routing in digital circuits

- Control units in CPUs and microcontrollers

- Function generation using logic expressions

- Signal selection in communication systems

- Arithmetic circuits and ALUs



**4x1 Multiplexer Truth Table**

| **Select Line S1** | **Select Line S0** | **Input Selected** | **Output (Y)** |
|--------------------|--------------------|---------------------|----------------|
| 0                  | 0                  | I0                  | I0             |
| 0                  | 1                  | I1                  | I1             |
| 1                  | 0                  | I2                  | I2             |
| 1                  | 1                  | I3                  | I3             |


![image](https://github.com/user-attachments/assets/868d9789-9a92-43d3-8fac-02291b4c4353)

 **Tinkercad Project Link**:
 👉 [ view on Tinkercad](https://www.tinkercad.com/things/iuB01vg3W2d-4x1-mux)








  




















 



















 











            
