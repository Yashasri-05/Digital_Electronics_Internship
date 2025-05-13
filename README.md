#                                                                                       DIGITAL ELECTRONICS

# What is digital electronics?
Digital electronics is a branch of electronics that deals with systems that use discrete (distinct) signal levels, typically represented by binary numbers — 0 and 1. Unlike analog electronics, where signals can vary smoothly across a range of values, digital electronics processes information using only two states (usually referred to as LOW and HIGH, or OFF and ON).

These two states are typically represented by:

0 → low voltage (e.g., 0 volts)

1 → high voltage (e.g., 5 volts or 3.3 volts)

# Applications of DE





1. Communication Systems


2. Mobile phones and Tablets


3. Automotive Industry


4. Medical and Healthcare Devices


5. Industrial Automation and Robotics


6. Military and Aerospace


7. Automobiles


8. Banking, Security, and E-commerce

# Digital VS Analog signals
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

---

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
# BASIC LOGIC GATES
# 1.AND GATE
# Symbol:
A D-shaped gate with two inputs and one output.
![image](https://github.com/user-attachments/assets/e31cb1e3-f24e-4d0e-b578-62df47243714)
# Function:
The AND gate outputs 1 (true) only when both inputs are 1. Otherwise, it outputs 0.

A.B=X.
The value of X will be True when both the inputs will be True.
# Truth Table
| A | B | A AND B |
|---|---|---------|
| 0 | 0 |    0    |
| 0 | 1 |    0    |
| 1 | 0 |    0    |
| 1 | 1 |    1    |
# 2. OR GATE
# Symbol:
A curved-shaped gate with two inputs and one output.
![image](https://github.com/user-attachments/assets/0e00f4a2-03be-4a14-b6d3-2683a953a1c8)
# Function:
The OR gate outputs 1 (true) if at least one input is 1. It outputs 0 only when both inputs are 0.
# Truth Table
| A | B | A OR B |
|---|---|--------|
| 0 | 0 |   0    |
| 0 | 1 |   1    |
| 1 | 0 |   1    |
| 1 | 1 |   1    |
# 3. NOT GATE
# Symbol:
The symbol for a NOT gate is a triangle with a small circle at the output
![image](https://github.com/user-attachments/assets/167b5b31-b5a7-4d2e-8a05-2be10719deb6)
# Function :
The output Y is the negation of the input A, respresented as, Y =  Ā 
Returns 1, if the input is 0.
Returns 0, if the input is 1.
# Truth table : 
| Input | Output |
|-------|--------|
|   0   |   1    |
|   1   |   0    |



 



















 











            
