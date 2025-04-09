# **Robotic Hand Research & Analysis**  

## **Nitinol Arm**  

### **Key Attributes**  
- **Power Draw:** 6-12V  
- **Force Output:**  
  - 3.43N of direct force  
  - 25,000 psi  
  - A 0.01-inch thick wire provides **8.9N** of force  
  - A 1/100-inch thick actuator wire can lift **2 lbs**  
- **Weight:** 16.561 lb/m²  
- **Sound:** Assumed to be relatively quiet  
- **Composition:** 53-57% nickel  

### **Resources**  
- [Activating Nitinol with Electric Current](https://www.imagesco.com/articles/nitinol/06.html)  
- [Nitinol Properties & Strength](https://www.edge-techind.com/Products/Refractory-Metals/Titanium/Nitinol/Nitinol-Muscle-Wire-795-1.html#:~:text=Nitinol%20returns%20to%20its%20original,25%2C000%20pounds%20per%20square%20inch)  



## **Solenoid Actuator Arm**  

### **Key Attributes**  
- **Power Draw:** 6V, 0.15A  
- **Force Output:** 80g (0.7845N)  
- **Weight:** 14g  
- **Sound:** Dependent on final design  

### **Resources**  
- [Solenoid Actuator Example](https://www.amazon.com/Uxcell-a14010700ux0262-Magnet-Electromagnet-Solenoid/dp/B019DT39ZG/ref=sr_1_8?dchild=1&keywords=Solenoid+11mm&qid=1623183175&sr=8-8)  

---

## **Pulley Arms**  

### **Key Attributes**  
- **Power Draw:** Dependent on motor  
- **Force Output:**  
  - Can be greatly multiplied using pulleys  
  - Space constraints determine final force capability  
- **Weight:** Dependent on final design  
- **Sound:**  
  - Pulleys are relatively quiet  
  - Motor generates most of the noise  



## **Planetary Gearbox Arm**  

### **Key Attributes**  
- **Power Draw:** Dependent on motor  
- **Force Output:**  
  - Basic gearbox can **double force**  
  - High-efficiency versions can **increase force 3-10×**  
- **Weight:** Dependent on final design  
- **Sound:** Motor is the primary noise source  



# **Additional Information**  

### **Force Requirements**  
- **500N** required to crush an empty soda can  
- **450N** is the maximum force a human hand can exert  

### **Battery Information**  
- **Voltage:** 7.4V  
- **Capacity:** 3000mAh  

### **Electrical Concepts**  
- **Watts (W):** $( W = V \times A )$
- **Kilowatts (kW):** $( kW = \frac{W}{1000} )$  
- **Torque (Nm):** $( T = \frac{60 \times P_{kW}}{2\pi \times RPM} )$
- **Torque (Nmm):** $( Nmm = \frac{Nm}{1000} )$
- **Efficiency Factor:** $( EFF = 90\% )$  
- **Power Factor:** $( PF = 0.85 )$
- **Horsepower (Hp):** $( Hp = \frac{V \times A \times EFF \times PF \times 1.73}{746} )$



## **Design Goal Equation** 

$F = T$

$F = 500N$

$T = 500N$

**(The goal is to generate 500N of force.)**  

---

## **Potential Motor Options**  
- [Mini DC Motor (3V, 19,000 RPM, 0.7W)](https://www.batteryspace.com/dcmotorminidcmotor3v19000rpm07wforrcflightsandhobby.aspx)  
- [DYS 1300KV Brushless Motor](https://www.amazon.com/DYS-1300KV-Brushless-Multicopters-Helicopter/dp/B077HLPP4N)  
- [Full Motor List & Analysis](https://www.notion.so/bc8e629efaa8453181374d2dd5ee959b?pvs=21)  

| Motor Type              | Voltage (V) | Current (A) | Power (W) | Power (kW) | RPM   | Power per RPM (kW/RPM) | Power per RPM (W/RPM) |
| ----------------------- | ----------- | ----------- | --------- | ---------- | ----- | ---------------------- | --------------------- |
| Battery Specs Motor     | 7.4         | 3           | 22.2      | 0.0222     | 19000 | 0.000011163258         | 0.011163258           |
| Current Motor           | 7.4         | 1.6         | 11.84     | 0.01184    | 19000 | 0.000005953738         | 0.005953738           |
| DC Motor: Mini DC Motor | 3           | 0.09        | 0.27      | 0.00027    | 19000 | 1.35769e-7             | 0.000135769           |
| Brushless Motor         | 14          | 15          | 210       | 0.21       | 18200 | 0.000110240078         | 0.110240078           |

---

# **Final Component Summary**  

### **Nitinol Arm**  

✔ Uses **6-12V**  
✔ Can lift **8.9N** with a **0.01-inch wire**  
✔ Provides **25,000 psi of force**  
✔ Weighs **16.561 lb/m²**  
✔ **Quiet operation** compared to motors  


### **Solenoid Actuator Arm**  

✔ Uses **6V at 0.15A**  
✔ Provides **80g (0.7845N) of force**  
✔ Weighs **14g**  
✔ **Likely loud**, depending on design  


### **Pulley System**  

✔ **Power draw depends on motor**  
✔ Can **greatly multiply force**  
✔ **Space constraints** impact final design  
✔ **Weight depends on implementation**  
✔ **Quiet operation**, motor is primary noise source  


### **Planetary Gearbox**  
✔ **Power draw depends on motor**  
✔ Can **increase force 3-10×**  
✔ **Weight depends on final design**  
✔ **Sound depends on motor & gearbox efficiency**  




