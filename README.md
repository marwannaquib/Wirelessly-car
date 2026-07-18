<img width="400" height="713" alt="WhatsApp Video 2026-07-18 at 8 07 06 PM" src="https://github.com/user-attachments/assets/0e3d6ce3-5997-48c2-a7d7-3d533592124f" />


I made a wireless-controlled car. The car uses a differential steering system, just as in tanks. The system works so that when moving forward or backwards, both wheels turn. However, steering for a specific direction stops one wheel and moves the other. For example, turning left, the left wheel stops and the right moves forward. 

The car is composed of an ESP32 Dev1 WROOM module that processes all inputs through Bluetooth and controls everything. Then the ESP32's GPIO pins are connected to the L298 motor driver module. Then the 2 DC motors are connected to the 2 outputs of the motor driver. The motor driver controls the speed and the direction of the spin of the DC motors depending on the ESP32's outputs.

The whole system is powered by a 11.1 V 2200 mAh lithium polymer battery. In my case, I connected it first to a power distribution circuit because its wires were too thick to enter the motor driver, but this is a case-sensitive thing. Then, from the power distribution board, the positive is hooked into the 12v port of the motor driver and the GND to the GND. Then the esp32 is connected to the motor driver’s 5v port and to GND.

Then, the wireless system is that the ESP32’s Bluetooth chip works and acts as a discoverable device to connect to, and with the Dabble app, gamepad, and digital mode using the arrows in it, the car is controlled.

Full youtube video:https://youtube.com/shorts/i4z68DzTvhQ?feature=share

<img width="1280" height="576" alt="WhatsApp Image 2026-07-18 at 9 56 32 PM" src="https://github.com/user-attachments/assets/3fe2894a-71ec-4ef4-b58e-db858482ee55" />
