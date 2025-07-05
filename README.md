# Astro-latency-probe
A toolkit for measuring, analyzing, and optimizing end-to-end latency in astronomical imaging and tracking systems. Designed for researchers and engineers, it enables microsecond-precision benchmarking of camera pipelines, shared memory architectures, and real-time feedback loops.

## Features

- **Hardware-Triggered Latency Measurement:**  
  Uses Arduino-based LED triggers and timestamping for precise, repeatable latency tests.

- **Microsecond Precision:**  
  Achieves high-resolution timing suitable for demanding real-time astronomical applications.

- **Shared Memory Architecture:**  
  Uses CACAO, MILK and included library ImageStreamIO to provide a platform, and subsequently push the captured frames to a shared memory location.

- **Live Camera Interface:**  
  Live image acquisition and frame captures from rtimv.

- **Flexible Test Setup:**  
  Supports a variety of scientific cameras (e.g., FLIR Blackfly S, Basler), USB3 interfaces, and custom test enclosures.

## Hardware Requirements

- Arduino UNO (or compatible microcontroller)
- LED and resistor (e.g., 100 Ω)
- Scientific camera (e.g., FLIR Blackfly S, Basler)
- Custom dark box or enclosure with acrylic diffuser (recommended)
- USB3 cables and power supply

## Quick Start

1. **Clone the Repository:**
    ```
    git clone [https://github.com/yourusername/astro-latency-bench.git](https://github.com/Tapomugdha/Astro-latency-probe/tree/main)
    cd astro-latency-probe
    ```

2. **Set Up Hardware:**
    - Assemble the LED circuit and connect to Arduino as per `hardware_setup.md`.
    - Position the camera to face the diffuser inside the dark box.

3. **Upload Arduino Sketch:**
    - Flash the provided sketch in the Arduino zip file to your Arduino.

4. **Install Python Dependencies:**
    ```
    Recommended: Anaconda python distributor
    ```

5. **Run Latency Test:**
    ```
    Compile mentioning proper directories, and run commands give in Running_Commands file
    ```

6. **See Live Capture:**
    - Adjut if required, the position of the LED into the darkbox for better diffusivity of flash to the camera.


## Example Results

- Achieved round-trip latency measurements in the microsecond range.
- Validated performance across multiple camera models and exposure settings.

## Recommended
Extract everything from the zip file "Basler_sharedmem_Tapo", and keep them in the same folder.
