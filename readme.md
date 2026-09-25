# Class-D Audio Amplifier v2.0 
An high-efficiency, digitally controlled Class-D audio power amplifier based on a **Full-Bridge (Bridge-Tied Load / BTL)** power stage. Version 2.0 introduces high-resolution stereo analog audio acquisition using the **PCM1808 24-bit ADC**, interfaced to an STM32 microcontroller configured via STM32Cube peripheral drivers and built using a CMake workflow in VS Code.
* **Power Stage Topology:** Full-Bridge (BTL) output stage offering doubled voltage swing across the load without requiring negative supply rails.
* **Audio Frontend (v2.0 Upgrade):** **PCM1808** 24-bit, 96 kHz stereo single-ended audio ADC sending digital audio over **$I^2S$ / DMA**.
* **Microcontroller Core:** STM32 MCU executing real-time signal handling, PWM dead-time generation, and digital modulation.
* **Filter Stage:** Differential 2nd-order LC reconstruction filter optimized for $4\Omega$ and $8\Omega$ speaker impedances.
* **Toolchain & Build System:** Firmware structured using **STM32CubeMX / Cube HAL**, configured for compilation with **CMake**, **Ninja**, and **GCC Arm Embedded** in **VS Code**.
* **PCB Hardware:** 2-layer optimized PCB layout engineered for minimal loop inductance, ground isolation between analog and digital/power sections, and EMI mitigation.

