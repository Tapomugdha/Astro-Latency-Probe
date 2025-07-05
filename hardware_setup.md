This guide describes how to assemble the hardware for precise, repeatable latency measurements in astronomical imaging systems using the Astro Latency Probe toolkit.
1. Components Required

    Arduino UNO (or compatible microcontroller)

    LED (standard 5mm, any color)

    Resistor (100 Ω recommended)

    Breadboard or custom PCB (optional, for prototyping or permanent setup)

    Jumper wires

    USB cable (for Arduino power and programming)

    Basler acA720-520um camera

    Dark box or enclosure (to block ambient light)

    Acrylic diffuser sheet (for uniform LED illumination)

    Camera mount/holder (to secure camera inside the enclosure)

    Laptop/PC (for running the latency measurement software)

2. Circuit Diagram
   +5V (Arduino) ----[100Ω]----|> (LED)----GND (Arduino)
               |
           Pin 13 (Digital Output)

    Pin 13 (or any digital output pin) is used to toggle the LED ON/OFF.

    The 100 Ω resistor limits current to the LED.

    Connect the anode (longer leg) of the LED to the resistor, and the cathode (shorter leg) to GND.

3. Assembly Steps

    Build the LED Circuit

        Insert the LED and resistor on a breadboard or solder onto a small PCB.

        Connect the resistor to Arduino Pin 13 (or chosen digital output).

        Connect the LED cathode to Arduino GND.

        Connect the LED anode (via resistor) to Pin 13.

    Prepare the Dark Box

        Use a small, light-tight enclosure or box.

        Cut a hole for the LED to face inward, behind the acrylic diffuser.

        Place the acrylic sheet inside the box, between the LED and camera position, to diffuse the LED light evenly.

    Mount the Camera

        Secure the scientific camera inside the box, facing the diffuser.

        Ensure the camera lens is aligned with the illuminated area of the diffuser.

    Connect Devices

        Connect the Arduino to your PC via USB (for programming and power).

        Connect the camera to your PC via USB3 or appropriate interface.

    Power Up

        Ensure all connections are secure.

        Power on the Arduino and camera.

[Camera] ---> [Acrylic Diffuser] ---> [LED] ---> [Dark Box Wall]

The camera looks through the diffuser at the LED. The LED is toggled by the Arduino to simulate a fast, repeatable event.

5. Tips for Reliable Measurements

    Shield the box from ambient light for consistent results.

    Use a stable mount for the camera to avoid misalignment during tests.

    Test the LED circuit separately before integrating with the camera setup.

    Label connections if using a custom PCB for easy troubleshooting.

6. Optional Enhancements

    Add a push-button to manually trigger the LED for testing.

    Use a multi-color LED for more advanced signal encoding.

    Integrate a temperature/humidity sensor for environmental monitoring.

7. Safety Notes

    Double-check wiring before powering the Arduino.

    Do not exceed the recommended current through the LED (typically ~20mA).

    Ensure the enclosure is ventilated if running extended tests.
