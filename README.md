#  Smart Snack Vending System using ATmega328P

An embedded system project that automates snack dispensing using the **ATmega328P** microcontroller. The system allows users to select one of three different snacks, automatically dispenses the selected item, and updates the remaining stock count in real time. This project demonstrates embedded system concepts such as motor control, user interaction, inventory management, and real-time display.

---

##  Project Overview

The Smart Snack Vending System is designed to provide an automated and efficient method of dispensing snacks. The system stores three different snack types in separate compartments. When a user selects a snack, the corresponding dispensing mechanism releases exactly one snack, updates the available stock count, and displays the remaining quantity. If a snack is out of stock, the system prevents dispensing and informs the user.

---

##  Features

-  Dispenses three different types of snacks
-  Individual button for each snack selection
-  Dedicated LCD display for each snack line
-  Real-time inventory tracking
-  Automatic stock count update after dispensing
-  Out-of-stock detection and notification
-  Accurate stepper motor control for dispensing


---

##  Components Used

| Component | Quantity |
|----------|:--------:|
| ATmega328P Microcontroller | 1 |
| 16×2 LCD Display (I2C) | 1 |
| Push Buttons | 3 |
| Stepper Motors | 3 |
| ULN2003 / A4988 Motor Drivers | 3 |
| Relay Modules | 3 |
| Dispensing Coils (Spiral Springs) | 3 |
| 16 MHz Crystal Oscillator | 1 |
| 22 pF Capacitors | 2 |
| 10 kΩ Resistor | 1 |
| Voltage Regulator | 1 |
| Power Supply | 1 |
| PCB | 1 |
| Connecting Wires | As Required |
| Snack Storage Box | build |

---

##  How It Works

1. The system initializes and displays the snack names and available stock.
2. The user presses the button corresponding to the desired snack.
3. The dispensing mechanism rotates and releases exactly one snack.
4. The remaining stock count is decreased by one.
5. The LCD display updates automatically with the new inventory count.
6. If no snacks remain, the system displays **"Out of Stock"** and prevents dispensing.

---

##  System Architecture

```
            User
             │
             ▼
      Press Selection Button
             │
             ▼
      ATmega328P Controller
             │
     ┌───────┼────────┐
     ▼       ▼        ▼
 Stepper1 Stepper2 Stepper3
     │       │        │
     ▼       ▼        ▼
 Snack1  Snack2  Snack3
     │       │        │
     └───────┼────────┘
             ▼
        Snack Output

 LCD 1       LCD 2       LCD 3
 Display     Display     Display
```

##  Future Improvements

- QR code payment integration
- Mobile application control
- Wi-Fi monitoring using ESP8266/ESP32
- Cloud-based inventory management
- Automatic refill notification
- Touchscreen interface

---

##  Applications

- University cafeterias
- Office snack stations
- Smart vending machines
- Libraries
- Waiting rooms
- Small retail shops
- Exhibition demonstrations
- Embedded systems education

---

##  Development Tools

- Microcontroller: ATmega328P
- Programming Language: Embedded C
- IDE: Arduino IDE
- PCB Design: EasyEDA

---

##  Author

**Vishwa Anjana**

Department of Physics

University Of Colombo

Embedded Systems Project

---

##  License

This project is licensed under the **MIT License**.

Feel free to use, modify, and distribute this project for educational and personal purposes.

---
