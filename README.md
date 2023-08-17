# 3 Stage Ring Oscillator Using MiMCAP

In the realm of analog circuit design and exploration, the 3-stage ring oscillator stands as a fascinating and essential component. This oscillator configuration, characterized by its circular arrangement of inverters, generates continuous oscillations with a frequency determined by the propagation delay of each inverter. The alluring simplicity of the ring oscillator belies its significance in various applications, including clock generation, frequency synthesis, and delay generation for digital circuits.

The primary objective of this project is to delve into the intricacies of the 3-stage ring oscillator, beginning with the conceptualization and schematic creation, followed by meticulous verification through simulations, and culminating in the design of its analog layout. By embarking on this journey, we aim to unravel the underlying principles governing ring oscillator behavior, reinforce our understanding of analog design techniques, and harness the power of simulation tools to validate our concepts in a virtual environment before translating them into physical layouts.

This project will take us through three key phases:

**1. Schematic Design:**

In this initial phase, we will craft a detailed schematic of the 3-stage ring oscillator, carefully selecting the appropriate transistors and components. Each stage will consist of an inverter and an Metal-Insulator-Metal (MiM) Capacitor(MiMCAP) and their interconnected arrangement will facilitate the feedback loop essential for sustained oscillations. The design process will involve considerations such as transistor sizing, biasing, and ensuring the required gain for oscillation initiation.

![image](https://github.com/shrey3000/3-Stage_Ring_Oscillator/assets/72602113/0c8dd655-d579-41a4-92ac-d7967c875c7b)

CMOS Inverter
![image](https://github.com/shrey3000/3-Stage_Ring_Oscillator/assets/72602113/3b7e7666-221b-48f5-8dd9-f0d901ec1a71)

Schematic having 3 CMOS invertor and corresponding 3 Metal-Insulator-Metal (MiM) Capacitors (MiMCAPs).

**2. Simulation and Verification:**

Once the schematic is in place, we will embark on a comprehensive simulation campaign. Utilizing ADE L, we perform transient response to obtain and compare the  
desired output and operational result, as we are simulating for a ring oscillator we need a sinusoidal wave within our defined range. After esuring the correct simulation results we can move ahead.  

![image](https://github.com/shrey3000/3-Stage_Ring_Oscillator/assets/72602113/735973b8-dbc8-4840-885f-deb9df799293)

Simulation circuit with symbol we designed.

![image](https://github.com/shrey3000/3-Stage_Ring_Oscillator/assets/72602113/42c1d725-9273-422a-844d-5448e447705e)

sinusoidal waveform


**3. Analog Layout Design:**

With a verified schematic in hand, we will transition to the layout design phase. Here, we will meticulously translate our circuit into a physical layout while considering factors such as transistor placement, routing, parasitic effects, and noise reduction. The art of analog layout design requires a delicate balance between creativity and precision, as we strive to optimize performance and manufacturability.

![image](https://github.com/shrey3000/3-Stage_Ring_Oscillator/assets/72602113/16144403-9477-4a22-b0ab-54be28503a0d)

**Serpentine connection**

As to maintain uniform parasitics thoughout the design we use some practices and serpentine is one of those. In this practice, we try to maintain the approximately equal net length of crucial nets so that we can predict the accurate propagation delay of CMOS invertors. 

![image](https://github.com/shrey3000/3-Stage_Ring_Oscillator/assets/72602113/a1ef5f28-cb45-4870-90bd-fe6cfba31479)

**Via**

In general, the use of via is avoided as using via means to drill a hole through the layers while manufacturing which can affect its performance and reliability. In the analog layout, I have used the via to connect "metal1" to "metal2" as I was using "metal2" for the interconnection of CMOS invertors.

![image](https://github.com/shrey3000/3-Stage_Ring_Oscillator/assets/72602113/420462a0-b6cf-45ca-8c69-03bb967ab8da)

**Metal-Insulator-Metal (MiM) Capacitor(MiMCAP)**

![image](https://github.com/shrey3000/3-Stage_Ring_Oscillator/assets/72602113/cb9476cf-7040-4222-9d4d-8499c2c32780)


Throughout this project, we will gain valuable insights into analog design principles, circuit behaviour, and the intricacies of oscillator architectures. By combining theoretical knowledge with practical implementation, we will bridge the gap between abstract concepts and tangible circuit layouts. The successful completion of this endeavour will equip us with a deeper appreciation for analog design, simulation techniques, and the artistry behind translating electronic ideas into reality.

So, let us embark on this captivating journey of exploration and creation, as we unravel the mysteries of the 3-stage ring oscillator, simulate its behavior, and craft an analog layout that embodies the harmonious fusion of design and engineering.
