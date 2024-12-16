

# **Piroi-Madalin-George - Katana Interactivă**

## **Introducere**  
An interactive katana project that blends modern technology with traditional design, powered by an **Arduino Nano** and a **WS2812B LED strip**. The katana will display dynamic lighting effects activated by motion, using an **MPU-6050 accelerometer and gyroscope sensor** for precise movement detection. It features a button to enhance interactivity. Powered by a **9V battery**, the katana will be coated with epoxy resin for durability.

---

## **Descriere generală**  
The interactive katana uses a combination of hardware components to achieve a responsive system:
- The **Arduino Nano** acts as the brain of the system, coordinating all components.
- A **WS2812B LED strip** provides dynamic and customizable lighting effects.
- The **MPU-6050 accelerometer/gyroscope** detects tilt and sharp movements (e.g., slashes) to trigger LED patterns.
- A **push button** allows switching between modes, such as static lighting, tilt-based effects, or special lighting patterns.
- The system is powered by a **9V battery** for portability.

---

## **Hardware Design**

### **Components and Their Roles**
| **Component**          | **Role**                                                                 |
|-------------------------|-------------------------------------------------------------------------|
| **Arduino Nano**        | Main microcontroller, processes input and controls the LED strip.       |
| **WS2812B LED Strip**   | Displays lighting effects based on input and movement.                  |
| **MPU-6050**            | Detects tilt and sudden movement (slashing motions).                    |
| **Push Button**         | User input for switching between modes.                                 |
| **9V Battery**          | Powers the entire system via Arduino Nano.                              |


---

### **Connections**

#### **1. Power Connections**
- **9V Battery**:
  - Positive terminal → **VIN** pin on Arduino Nano.
  - Negative terminal → **GND** on Arduino Nano.

- **WS2812B LED Strip**:
  - **VCC** → **5V** pin on Arduino Nano.
  - **GND** → **GND** pin on Arduino Nano.

#### **2. LED Control**
- **WS2812B LED Strip**:
  - **DI (Data Input)** → **D6** pin on Arduino Nano 

#### **3. MPU-6050 (Motion Sensor)**
- **VCC** → **3.3V** pin on Arduino Nano.
- **GND** → **GND** on Arduino Nano.
- **SDA** → **A4** pin on Arduino Nano (I2C data line).
- **SCL** → **A5** pin on Arduino Nano (I2C clock line).

#### **4. Push Button**
- One terminal → **D2** pin on Arduino Nano.
- Other terminal → **GND**.

---

## **BOM (Bill of Materials)**

### **Bill of Materials (BOM)**

1. **Arduino Nano**  
   - **Quantity**: 1  

2. **WS2812B LED Strip**  
   - **Quantity**: 1 (30 LEDs)  

3. **MPU-6050 Sensor**  
   - **Quantity**: 1   

4. **Push Button**  
   - **Quantity**: 1   

5. **9V Battery + Connector**  
   - **Quantity**: 1  



## **Software Design**

1. **LED Control**:  
   The **FastLED** library is used to control the WS2812B LED strip. The LEDs change colors and patterns based on:
   - Button input (e.g., static mode, special patterns).
   - Tilt or movement detection from the MPU-6050 sensor.

2. **Motion Detection**:  
   The **MPU-6050** sensor communicates via I2C and detects:
   - **Sharp movements** (slashes): Trigger dynamic LED effects.
   - **Tilt detection**: Controls how many LEDs light up based on the angle of the katana.

3. **Button Input**:
   -

---

## **Rezultate Obținute**


---

## **Concluzii**



---

## **Cod sursă și alte resurse ce trebuie să existe pe GitHub**

-

---

## **Jurnal**



---

## **Bibliografie/Resurse**
[ARDUINO NANO.pdf](https://github.com/user-attachments/files/18157635/ARDUINO.NANO.pdf)
[MOD-MPU6050 (1).pdf](https://github.com/user-attachments/files/18157645/MOD-MPU6050.1.pdf)
[Conex](https://www.conexelectronic.r/)
[eMAG]([Conex](https://www.conexelectronic.r/))





---

Let me know if you need further refinements or additional sections! 😊
