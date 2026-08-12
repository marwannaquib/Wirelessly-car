<img width="400" height="713" alt="WhatsApp Video 2026-07-18 at 8 07 06 PM" src="https://github.com/user-attachments/assets/0e3d6ce3-5997-48c2-a7d7-3d533592124f" />



I made a wireless-controlled car. The car uses a differential steering system, just as in tanks, but only 2 wheels that are in the front that are hooked up to motors, and one wheel at the rear is a desk chair wheel to freely rotate in any direction. The system works so that when moving forward or backwards, both wheels turn. However, steering for a specific direction stops one wheel and moves the other. For example, turning left, the left wheel stops and the right moves forward. 

The car is composed of an ESP32 Dev1 WROOM module that processes all inputs through Bluetooth and controls everything. Then the ESP32's GPIO pins are connected to the L298 motor driver module. Then the 2 DC motors are connected to the 2 outputs of the motor driver. The motor driver controls the speed and the direction of the spin of the DC motors depending on the ESP32's outputs. The PINs and connections from the esp32 to the motor driver are all listed in the wiring diagram.

The whole system is powered by a 11.1 V 2200 mAh lithium polymer battery. In my case, I connected it first to a power distribution circuit because its wires were too thick to enter the motor driver, but this is a case-sensitive thing. Then, from the power distribution board, the positive is hooked into the 12v port of the motor driver and the GND to the GND. Then the esp32 is connected to the motor driver’s 5v port and to GND.

Then, the wireless system is that the ESP32’s Bluetooth chip works and acts as a discoverable device to connect to, and with the Dabble app, gamepad, and digital mode using the arrows in it, the car is controlled.

Full youtube video:https://youtube.com/shorts/i4z68DzTvhQ?feature=share

<img width="1280" height="576" alt="WhatsApp Image 2026-07-18 at 9 56 32 PM" src="https://github.com/user-attachments/assets/3fe2894a-71ec-4ef4-b58e-db858482ee55" />

| Component | Description | Quantity | Unit Price (EGP) | Total Price (EGP) | Source Link |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **ESP32 Dev1 WROOM Module** | 30-pin Development Board with WiFi and Bluetooth (CP2102 chip), acts as the main controller via Bluetooth. | 1 | 320 EGP | 320 EGP | [RAM E-Shop Link](https://www.ram-e-shop.com/shop/kit-esp32-esp32s-30pin-esp-32s-30pin-development-board-wifi-bluetooth-with-new-cp2102-chip-7433) |
| **L298N Motor Driver Module** | Dual H-Bridge Motor Driver Red Board, controls direction and speed of the two DC motors. | 1 | 140 EGP | 140 EGP | [RAM E-Shop Link](https://www.ram-e-shop.com/shop/kit-l298-red-l298-module-red-board-dual-h-bridge-motor-driver-using-l298n-7084) |
| **TT Mini DC Gearbox Motors (Pair)** | Pair of 2 motors with back shaft for driving the differential steering wheels. | 1 | 110 EGP | 110 EGP | [RAM E-Shop Link](https://www.ram-e-shop.com/shop/ro-motor-tt-mini-dc-gearbox-motors-pair-2-motors-with-back-shaft-9455) |
| **Robot Wheels 65x26mm (Pair)** | Pair of 2 tires (RW002) for mini DC gearbox yellow motors. | 1 | 75 EGP | 75 EGP | [RAM E-Shop Link](https://www.ram-e-shop.com/shop/ro-wheel-rw002-robot-wheels-65x26mm-for-mini-dc-gearbox-yellow-motors-2-tires-rw002-8808) |
| **4-Channel DC Power Distributor** | Power distribution circuit used to safely manage thick battery wires to the motor driver. | 1 | 90 EGP | 90 EGP | [Fares PCB Link](https://fares-pcb.com/product/4-channel-dc-power-distributor/) |
| **11.1V 2200mAh LiPo Battery** | 3S Lithium Polymer battery providing the primary power source for the entire vehicle. | 1 | 950 EGP | 950 EGP | - |
| **Jumper Wires & Connecting Wires** | Wiring used to connect ESP32, Motor Driver, and Power Distribution Board. | 1 | - | - | - |
| **Hot Glue / Adhesive** | Structural adhesive for holding components on the chassis. | 1 | - | - | - |
| **Cardboard** | Main material for creating the vehicle chassis/body. | 1 | - | - | - |
| **Desk Chair Wheel** | Used as a caster wheel for stability and free multi-directional movement. | 1 | - | - | - |
| **Soldering Iron & Solder Wire** | Tools used for establishing permanent electrical connections. | 1 | - | - | - |
