# 25011102018_FIoT_LAB — Foundations of Internet of Things + Lab

**Course Code:** 25CS2741  
**Course Title:** Fundamentals of Internet of Things + Lab  
**Institution:** Shiv Nadar University, Chennai — Department of Computer Science & Engineering  
**Academic Year:** II Year / 3rd Semester B. Tech CSE (IoT) Sections A   
**Student Register Number:** 25011102018  

---

## 1. About the Repository

This repository maintains the complete laboratory experiment submissions, hardware bring-up documentation, circuit schematics, source code, and firmware binaries for the **Foundations of Internet of Things (FIoT) Lab**. 

The laboratory syllabus spans two distinct microcontroller architectures:
1. **8051 Architecture (CAT 2 to CAT 7 — 13 Evaluated Tasks):** Bare-metal Embedded C targeting the Atmel/Microchip **AT89S52** microcontroller development board. All peripherals are controlled through direct register-level memory-mapped I/O access with Keil µVision C51.
2. **STM32 Architecture (CAT 8 to CAT 14 — 20 Evaluated Tasks):** ARM Cortex-M based embedded firmware development using **STM32CubeMX**, **Keil MDK-ARM**, and the **STM32 HAL (Hardware Abstraction Layer)** targeting the STM32 Blue Pill (STM32F103C8T6) and NUCLEO-F401RE (STM32F401RET6) development platforms.

---

## 2. Repository Structure

```text
25011102018_FIoT_LAB/
│
├── README.md                           # Master repository documentation & course index
├── .gitignore                          # Clean build tracking (tracks .hex, ignores temp build files)
│
├── 8051/                               # 8051 Microcontroller Platform (20 Tasks across CAT 2 to 7)
│   ├── CAT2/                            # Continuous Lab Evaluation-2: Hardware Bring-Up, LED Blink & Delay Library
│       ├── TASK2A/                      # Dedicated Task: Hardware Board Bring-Up
│       │   ├── main.c                  # C source file
│       │   ├── STARTUP.A51             # 8051 Assembly startup
│       │   ├── TASK2A.uvproj            # Keil µVision project
│       │   ├── Objects/                # Build output directory
│       │   │   └── TASK2A.hex          # Compiled Intel HEX firmware
│       │   ├── circuit.png             # Task wiring schematic
│       │   └── README.md               # Task technical report
│       ├── TASK2B/                      # Dedicated Task: 1 Hz LED Blink on Port 2
│       │   ├── main.c                  # C source file
│       │   ├── STARTUP.A51             # 8051 Assembly startup
│       │   ├── TASK2B.uvproj            # Keil µVision project
│       │   ├── Objects/                # Build output directory
│       │   │   └── TASK2B.hex          # Compiled Intel HEX firmware
│       │   ├── circuit.png             # Task wiring schematic
│       │   └── README.md               # Task technical report
│       ├── TASK2C/                      # Dedicated Task: Parameterized Delay Library
│       │   ├── main.c                  # C source file
│       │   ├── STARTUP.A51             # 8051 Assembly startup
│       │   ├── TASK2C.uvproj            # Keil µVision project
│       │   ├── Objects/                # Build output directory
│       │   │   └── TASK2C.hex          # Compiled Intel HEX firmware
│       │   ├── circuit.png             # Task wiring schematic
│       │   └── README.md               # Task technical report
│       ├── circuit.png             # CAT2 complete hardware schematic
│       └── README.md               # CAT2 evaluation overview
│
│   ├── CAT3/                            # Continuous Lab Evaluation-3: Timer-Based LED Pattern Generator & Button Controller
│       ├── TASK3A/                      # Dedicated Task: Button Debounced 4-Mode LED Pattern Controller
│       │   ├── main.c                  # C source file
│       │   ├── STARTUP.A51             # 8051 Assembly startup
│       │   ├── TASK3A.uvproj            # Keil µVision project
│       │   ├── Objects/                # Build output directory
│       │   │   └── TASK3A.hex          # Compiled Intel HEX firmware
│       │   ├── circuit.png             # Task wiring schematic
│       │   └── README.md               # Task technical report
│       ├── TASK3B/                      # Dedicated Task: 4-Bit Binary Counter Mode
│       │   ├── main.c                  # C source file
│       │   ├── STARTUP.A51             # 8051 Assembly startup
│       │   ├── TASK3B.uvproj            # Keil µVision project
│       │   ├── Objects/                # Build output directory
│       │   │   └── TASK3B.hex          # Compiled Intel HEX firmware
│       │   ├── circuit.png             # Task wiring schematic
│       │   └── README.md               # Task technical report
│       ├── TASK3C/                      # Dedicated Task: Alternating LED Pattern Mode
│       │   ├── main.c                  # C source file
│       │   ├── STARTUP.A51             # 8051 Assembly startup
│       │   ├── TASK3C.uvproj            # Keil µVision project
│       │   ├── Objects/                # Build output directory
│       │   │   └── TASK3C.hex          # Compiled Intel HEX firmware
│       │   ├── circuit.png             # Task wiring schematic
│       │   └── README.md               # Task technical report
│       ├── TASK3D/                      # Dedicated Task: All-LED Flash Pattern Mode
│       │   ├── main.c                  # C source file
│       │   ├── STARTUP.A51             # 8051 Assembly startup
│       │   ├── TASK3D.uvproj            # Keil µVision project
│       │   ├── Objects/                # Build output directory
│       │   │   └── TASK3D.hex          # Compiled Intel HEX firmware
│       │   ├── circuit.png             # Task wiring schematic
│       │   └── README.md               # Task technical report
│       ├── circuit.png             # CAT3 complete hardware schematic
│       └── README.md               # CAT3 evaluation overview
│
│   ├── CAT4/                            # Continuous Lab Evaluation-4: Human-Machine Interface using Keypad, LEDs & 7-Seg
│       ├── TASK4A/                      # Dedicated Task: 4x4 Keypad Scanning, 7-Segment & LED HMI
│       │   ├── main.c                  # C source file
│       │   ├── STARTUP.A51             # 8051 Assembly startup
│       │   ├── TASK4A.uvproj            # Keil µVision project
│       │   ├── Objects/                # Build output directory
│       │   │   └── TASK4A.hex          # Compiled Intel HEX firmware
│       │   ├── circuit.png             # Task wiring schematic
│       │   └── README.md               # Task technical report
│       ├── TASK4B/                      # Dedicated Task: 7-Segment Display Numerical Output Driver
│       │   ├── main.c                  # C source file
│       │   ├── STARTUP.A51             # 8051 Assembly startup
│       │   ├── TASK4B.uvproj            # Keil µVision project
│       │   ├── Objects/                # Build output directory
│       │   │   └── TASK4B.hex          # Compiled Intel HEX firmware
│       │   ├── circuit.png             # Task wiring schematic
│       │   └── README.md               # Task technical report
│       ├── TASK4C/                      # Dedicated Task: Interactive Keypad LED Pattern Controller
│       │   ├── main.c                  # C source file
│       │   ├── STARTUP.A51             # 8051 Assembly startup
│       │   ├── TASK4C.uvproj            # Keil µVision project
│       │   ├── Objects/                # Build output directory
│       │   │   └── TASK4C.hex          # Compiled Intel HEX firmware
│       │   ├── circuit.png             # Task wiring schematic
│       │   └── README.md               # Task technical report
│       ├── circuit.png             # CAT4 complete hardware schematic
│       └── README.md               # CAT4 evaluation overview
│
│   ├── CAT5/                            # Continuous Lab Evaluation-5: Hardware Timer, Software PWM, & Stepper Motor
│       ├── TASK5A/                      # Dedicated Task: 1ms Hardware Timer 0 Interrupt Driver
│       │   ├── main.c                  # C source file
│       │   ├── STARTUP.A51             # 8051 Assembly startup
│       │   ├── TASK5A.uvproj            # Keil µVision project
│       │   ├── Objects/                # Build output directory
│       │   │   └── TASK5A.hex          # Compiled Intel HEX firmware
│       │   ├── circuit.png             # Task wiring schematic
│       │   └── README.md               # Task technical report
│       ├── TASK5B/                      # Software PWM Fading Analysis Suite
│       │   ├── TASK5B.1/                # Subtask: Software PWM Triangular Wave Modulation
│       │   │   ├── main.c              # C source file
│       │   │   ├── STARTUP.A51         # 8051 Assembly startup
│       │   │   ├── TASK5B_1.uvproj       # Keil µVision project
│       │   │   ├── Objects/            # Build output directory
│       │   │   │   └── TASK5B_1.hex   # Compiled Intel HEX firmware
│       │   │   ├── circuit.png         # Task wiring schematic
│       │   │   └── README.md           # Task technical report
│       │   ├── TASK5B.2/                # Subtask: Software PWM Carrier Frequency Analysis
│       │   │   ├── main.c              # C source file
│       │   │   ├── STARTUP.A51         # 8051 Assembly startup
│       │   │   ├── TASK5B_2.uvproj       # Keil µVision project
│       │   │   ├── Objects/            # Build output directory
│       │   │   │   └── TASK5B_2.hex   # Compiled Intel HEX firmware
│       │   │   ├── circuit.png         # Task wiring schematic
│       │   │   └── README.md           # Task technical report
│       │   └── TASK5B.3/                # Subtask: Multi-LED Breathing & Brightness Level Controller
│       │       ├── main.c              # C source file
│       │       ├── STARTUP.A51         # 8051 Assembly startup
│       │       ├── TASK5B_3.uvproj       # Keil µVision project
│       │       ├── Objects/            # Build output directory
│       │       │   └── TASK5B_3.hex   # Compiled Intel HEX firmware
│       │       ├── circuit.png         # Task wiring schematic
│       │       └── README.md           # Task technical report
│       ├── TASK5C/                      # Dedicated Task: Stepper Motor Full-Step Sequence Generator
│       │   ├── main.c                  # C source file
│       │   ├── STARTUP.A51             # 8051 Assembly startup
│       │   ├── TASK5C.uvproj            # Keil µVision project
│       │   ├── Objects/                # Build output directory
│       │   │   └── TASK5C.hex          # Compiled Intel HEX firmware
│       │   ├── circuit.png             # Task wiring schematic
│       │   └── README.md               # Task technical report
│       ├── circuit.png             # CAT5 complete hardware schematic
│       └── README.md               # CAT5 evaluation overview
│
│   ├── CAT6/                            # Continuous Lab Evaluation-6: UART Driver and Serial Debugging
│       ├── TASK6A/                      # Dedicated Task: UART Non-Blocking String Transmission
│       │   ├── main.c                  # C source file
│       │   ├── STARTUP.A51             # 8051 Assembly startup
│       │   ├── TASK6A.uvproj            # Keil µVision project
│       │   ├── Objects/                # Build output directory
│       │   │   └── TASK6A.hex          # Compiled Intel HEX firmware
│       │   ├── circuit.png             # Task wiring schematic
│       │   └── README.md               # Task technical report
│       ├── TASK6B/                      # Dedicated Task: UART Terminal Echo & Circular Ring Buffer RX
│       │   ├── main.c                  # C source file
│       │   ├── STARTUP.A51             # 8051 Assembly startup
│       │   ├── TASK6B.uvproj            # Keil µVision project
│       │   ├── Objects/                # Build output directory
│       │   │   └── TASK6B.hex          # Compiled Intel HEX firmware
│       │   ├── circuit.png             # Task wiring schematic
│       │   └── README.md               # Task technical report
│       ├── circuit.png             # CAT6 complete hardware schematic
│       └── README.md               # CAT6 evaluation overview
│
│   └── CAT7/                            # Continuous Lab Evaluation-7: 16×2 LCD Driver Development & Menu Navigation
        ├── TASK7A/                      # Dedicated Task: HD44780 16×2 LCD 4-Bit Mode Driver Implementation
        │   ├── main.c                  # C source file
        │   ├── STARTUP.A51             # 8051 Assembly startup
        │   ├── TASK7A.uvproj            # Keil µVision project
        │   ├── Objects/                # Build output directory
        │   │   └── TASK7A.hex          # Compiled Intel HEX firmware
        │   ├── circuit.png             # Task wiring schematic
        │   └── README.md               # Task technical report
        ├── TASK7B/                      # Dedicated Task: Dynamic LCD Counter & Custom CGRAM Glyphs
        │   ├── main.c                  # C source file
        │   ├── STARTUP.A51             # 8051 Assembly startup
        │   ├── TASK7B.uvproj            # Keil µVision project
        │   ├── Objects/                # Build output directory
        │   │   └── TASK7B.hex          # Compiled Intel HEX firmware
        │   ├── circuit.png             # Task wiring schematic
        │   └── README.md               # Task technical report
        ├── TASK7C/                      # Dedicated Task: 4x4 Keypad Interactive LCD Menu Navigation
        │   ├── main.c                  # C source file
        │   ├── STARTUP.A51             # 8051 Assembly startup
        │   ├── TASK7C.uvproj            # Keil µVision project
        │   ├── Objects/                # Build output directory
        │   │   └── TASK7C.hex          # Compiled Intel HEX firmware
        │   ├── circuit.png             # Task wiring schematic
        │   └── README.md               # Task technical report
        ├── circuit.png             # CAT7 complete hardware schematic
        └── README.md               # CAT7 evaluation overview
│
└── STM32/                              # STM32 ARM Cortex-M Platform (17 Tasks across CAT 8 to 13)
    ├── CAT8/                            # Continuous Lab Evaluation-8: STM32 GPIO Bring-Up & Switch Control
    │   ├── TASK8A/                      # Dedicated Task: GPIO Direct Follow Mode (PC13 Button to PA5 LED)
    │   │   ├── TASK8A.ioc              # STM32CubeMX configuration file
    │   │   ├── .mxproject              # STM32CubeMX project metadata descriptor
    │   │   ├── Core/                   # HAL Core application layer (Inc/ & Src/)
    │   │   │   ├── Inc/main.h, stm32f4xx_it.h
    │   │   │   └── Src/main.c, stm32f4xx_it.c, system_stm32f4xx.c
    │   │   ├── Drivers/                # CMSIS & STM32F4xx HAL Driver libraries
    │   │   ├── MDK-ARM/                # Keil MDK-ARM µVision project folder
    │   │   │   ├── TASK8A.uvprojx      # Keil µVision project file
    │   │   │   └── startup_stm32f401xe.s # ARM Cortex-M4 vector table & startup
    │   │   ├── circuit.png             # Task hardware schematic diagram
    │   │   └── README.md               # Task technical report & inferences
    │   ├── TASK8B/                      # Dedicated Task: Debounced Push Button Toggle Mode
    │   │   ├── TASK8B.ioc              # STM32CubeMX configuration file
    │   │   ├── .mxproject              # STM32CubeMX project metadata descriptor
    │   │   ├── Core/                   # HAL Core application layer (Inc/ & Src/)
    │   │   │   ├── Inc/main.h, stm32f4xx_it.h
    │   │   │   └── Src/main.c, stm32f4xx_it.c, system_stm32f4xx.c
    │   │   ├── Drivers/                # CMSIS & STM32F4xx HAL Driver libraries
    │   │   ├── MDK-ARM/                # Keil MDK-ARM µVision project folder
    │   │   │   ├── TASK8B.uvprojx      # Keil µVision project file
    │   │   │   └── startup_stm32f401xe.s # ARM Cortex-M4 vector table & startup
    │   │   ├── circuit.png             # Task hardware schematic diagram
    │   │   └── README.md               # Task technical report & inferences
    │   ├── TASK8C/                      # Dedicated Task: Press Duration Classifier (Short vs Long Press)
    │   │   ├── TASK8C.ioc              # STM32CubeMX configuration file
    │   │   ├── .mxproject              # STM32CubeMX project metadata descriptor
    │   │   ├── Core/                   # HAL Core application layer (Inc/ & Src/)
    │   │   │   ├── Inc/main.h, stm32f4xx_it.h
    │   │   │   └── Src/main.c, stm32f4xx_it.c, system_stm32f4xx.c
    │   │   ├── Drivers/                # CMSIS & STM32F4xx HAL Driver libraries
    │   │   ├── MDK-ARM/                # Keil MDK-ARM µVision project folder
    │   │   │   ├── TASK8C.uvprojx      # Keil µVision project file
    │   │   │   └── startup_stm32f401xe.s # ARM Cortex-M4 vector table & startup
    │   │   ├── circuit.png             # Task hardware schematic diagram
    │   │   └── README.md               # Task technical report & inferences
    │   ├── circuit.png             # CAT8 complete hardware schematic
    │   └── README.md               # CAT8 evaluation overview
    │
    ├── CAT9/                            # Continuous Lab Evaluation-9: Timer Interrupts & Hardware PWM Generation
    │   ├── TASK9A/                      # Dedicated Task: Hardware Timer 2 Periodic Interrupt (1 Hz Blink)
    │   │   ├── TASK9A.ioc              # STM32CubeMX configuration file
    │   │   ├── .mxproject              # STM32CubeMX project metadata descriptor
    │   │   ├── Core/                   # HAL Core application layer (Inc/ & Src/)
    │   │   │   ├── Inc/main.h, stm32f4xx_it.h
    │   │   │   └── Src/main.c, stm32f4xx_it.c, system_stm32f4xx.c
    │   │   ├── Drivers/                # CMSIS & STM32F4xx HAL Driver libraries
    │   │   ├── MDK-ARM/                # Keil MDK-ARM µVision project folder
    │   │   │   ├── TASK9A.uvprojx      # Keil µVision project file
    │   │   │   └── startup_stm32f401xe.s # ARM Cortex-M4 vector table & startup
    │   │   ├── circuit.png             # Task hardware schematic diagram
    │   │   └── README.md               # Task technical report & inferences
    │   ├── TASK9B/                      # Dedicated Task: Hardware Timer PWM Generation with Variable Duty
    │   │   ├── TASK9B.ioc              # STM32CubeMX configuration file
    │   │   ├── .mxproject              # STM32CubeMX project metadata descriptor
    │   │   ├── Core/                   # HAL Core application layer (Inc/ & Src/)
    │   │   │   ├── Inc/main.h, stm32f4xx_it.h
    │   │   │   └── Src/main.c, stm32f4xx_it.c, system_stm32f4xx.c
    │   │   ├── Drivers/                # CMSIS & STM32F4xx HAL Driver libraries
    │   │   ├── MDK-ARM/                # Keil MDK-ARM µVision project folder
    │   │   │   ├── TASK9B.uvprojx      # Keil µVision project file
    │   │   │   └── startup_stm32f401xe.s # ARM Cortex-M4 vector table & startup
    │   │   ├── circuit.png             # Task hardware schematic diagram
    │   │   └── README.md               # Task technical report & inferences
    │   ├── circuit.png             # CAT9 complete hardware schematic
    │   └── README.md               # CAT9 evaluation overview
    │
    ├── CAT10/                           # Continuous Lab Evaluation-10: USART Serial Modes & DMA Streaming
    │   ├── TASK10A/                     # Dedicated Task: USART2 Polling String Transmission
    │   │   ├── TASK10A.ioc              # STM32CubeMX configuration file
    │   │   ├── .mxproject              # STM32CubeMX project metadata descriptor
    │   │   ├── Core/                   # HAL Core application layer (Inc/ & Src/)
    │   │   │   ├── Inc/main.h, stm32f4xx_it.h
    │   │   │   └── Src/main.c, stm32f4xx_it.c, system_stm32f4xx.c
    │   │   ├── Drivers/                # CMSIS & STM32F4xx HAL Driver libraries
    │   │   ├── MDK-ARM/                # Keil MDK-ARM µVision project folder
    │   │   │   ├── TASK10A.uvprojx      # Keil µVision project file
    │   │   │   └── startup_stm32f401xe.s # ARM Cortex-M4 vector table & startup
    │   │   ├── circuit.png             # Task hardware schematic diagram
    │   │   └── README.md               # Task technical report & inferences
    │   ├── TASK10B/                     # Dedicated Task: USART2 Interrupt-Driven Receive & Echo
    │   │   ├── TASK10B.ioc              # STM32CubeMX configuration file
    │   │   ├── .mxproject              # STM32CubeMX project metadata descriptor
    │   │   ├── Core/                   # HAL Core application layer (Inc/ & Src/)
    │   │   │   ├── Inc/main.h, stm32f4xx_it.h
    │   │   │   └── Src/main.c, stm32f4xx_it.c, system_stm32f4xx.c
    │   │   ├── Drivers/                # CMSIS & STM32F4xx HAL Driver libraries
    │   │   ├── MDK-ARM/                # Keil MDK-ARM µVision project folder
    │   │   │   ├── TASK10B.uvprojx      # Keil µVision project file
    │   │   │   └── startup_stm32f401xe.s # ARM Cortex-M4 vector table & startup
    │   │   ├── circuit.png             # Task hardware schematic diagram
    │   │   └── README.md               # Task technical report & inferences
    │   ├── TASK10C/                     # Dedicated Task: USART2 DMA Circular Telemetry Streaming
    │   │   ├── TASK10C.ioc              # STM32CubeMX configuration file
    │   │   ├── .mxproject              # STM32CubeMX project metadata descriptor
    │   │   ├── Core/                   # HAL Core application layer (Inc/ & Src/)
    │   │   │   ├── Inc/main.h, stm32f4xx_it.h
    │   │   │   └── Src/main.c, stm32f4xx_it.c, system_stm32f4xx.c
    │   │   ├── Drivers/                # CMSIS & STM32F4xx HAL Driver libraries
    │   │   ├── MDK-ARM/                # Keil MDK-ARM µVision project folder
    │   │   │   ├── TASK10C.uvprojx      # Keil µVision project file
    │   │   │   └── startup_stm32f401xe.s # ARM Cortex-M4 vector table & startup
    │   │   ├── circuit.png             # Task hardware schematic diagram
    │   │   └── README.md               # Task technical report & inferences
    │   ├── circuit.png             # CAT10 complete hardware schematic
    │   └── README.md               # CAT10 evaluation overview
    │
    ├── CAT11/                           # Continuous Lab Evaluation-10C: HTTP Server STM32–Wemos Wi-Fi Modem
    │   ├── TASK11A/                     # Dedicated Task: ESP8266 TCP Server Configuration via AT Commands
    │   │   ├── TASK11A.ioc              # STM32CubeMX configuration file
    │   │   ├── .mxproject              # STM32CubeMX project metadata descriptor
    │   │   ├── Core/                   # HAL Core application layer (Inc/ & Src/)
    │   │   │   ├── Inc/main.h, stm32f4xx_it.h
    │   │   │   └── Src/main.c, stm32f4xx_it.c, system_stm32f4xx.c
    │   │   ├── Drivers/                # CMSIS & STM32F4xx HAL Driver libraries
    │   │   ├── MDK-ARM/                # Keil MDK-ARM µVision project folder
    │   │   │   ├── TASK11A.uvprojx      # Keil µVision project file
    │   │   │   └── startup_stm32f401xe.s # ARM Cortex-M4 vector table & startup
    │   │   ├── circuit.png             # Task hardware schematic diagram
    │   │   └── README.md               # Task technical report & inferences
    │   ├── TASK11B/                     # Dedicated Task: HTTP Request Parser & Static HTML Response
    │   │   ├── TASK11B.ioc              # STM32CubeMX configuration file
    │   │   ├── .mxproject              # STM32CubeMX project metadata descriptor
    │   │   ├── Core/                   # HAL Core application layer (Inc/ & Src/)
    │   │   │   ├── Inc/main.h, stm32f4xx_it.h
    │   │   │   └── Src/main.c, stm32f4xx_it.c, system_stm32f4xx.c
    │   │   ├── Drivers/                # CMSIS & STM32F4xx HAL Driver libraries
    │   │   ├── MDK-ARM/                # Keil MDK-ARM µVision project folder
    │   │   │   ├── TASK11B.uvprojx      # Keil µVision project file
    │   │   │   └── startup_stm32f401xe.s # ARM Cortex-M4 vector table & startup
    │   │   ├── circuit.png             # Task hardware schematic diagram
    │   │   └── README.md               # Task technical report & inferences
    │   ├── TASK11C/                     # Dedicated Task: Node-RED HTTP Client Ingestion
    │   │   ├── TASK11C.ioc              # STM32CubeMX configuration file
    │   │   ├── .mxproject              # STM32CubeMX project metadata descriptor
    │   │   ├── Core/                   # HAL Core application layer (Inc/ & Src/)
    │   │   │   ├── Inc/main.h, stm32f4xx_it.h
    │   │   │   └── Src/main.c, stm32f4xx_it.c, system_stm32f4xx.c
    │   │   ├── Drivers/                # CMSIS & STM32F4xx HAL Driver libraries
    │   │   ├── MDK-ARM/                # Keil MDK-ARM µVision project folder
    │   │   │   ├── TASK11C.uvprojx      # Keil µVision project file
    │   │   │   └── startup_stm32f401xe.s # ARM Cortex-M4 vector table & startup
    │   │   ├── circuit.png             # Task hardware schematic diagram
    │   │   └── README.md               # Task technical report & inferences
    │   ├── circuit.png             # CAT11 complete hardware schematic
    │   └── README.md               # CAT11 evaluation overview
    │
    ├── CAT12/                           # Continuous Lab Evaluation-12: NUCLEO-F401RE GPIO & User Input Programming
    │   ├── TASK12A/                     # Dedicated Task: On-Board User LED LD2 Bring-Up (PA5 Fixed Blink)
    │   │   ├── TASK12A.ioc              # STM32CubeMX configuration file
    │   │   ├── .mxproject              # STM32CubeMX project metadata descriptor
    │   │   ├── Core/                   # HAL Core application layer (Inc/ & Src/)
    │   │   │   ├── Inc/main.h, stm32f4xx_it.h
    │   │   │   └── Src/main.c, stm32f4xx_it.c, system_stm32f4xx.c
    │   │   ├── Drivers/                # CMSIS & STM32F4xx HAL Driver libraries
    │   │   ├── MDK-ARM/                # Keil MDK-ARM µVision project folder
    │   │   │   ├── TASK12A.uvprojx      # Keil µVision project file
    │   │   │   └── startup_stm32f401xe.s # ARM Cortex-M4 vector table & startup
    │   │   ├── circuit.png             # Task hardware schematic diagram
    │   │   └── README.md               # Task technical report & inferences
    │   ├── TASK12B/                     # Dedicated Task: Push Button B1 Control with Latching State Remembrance
    │   │   ├── TASK12B.ioc              # STM32CubeMX configuration file
    │   │   ├── .mxproject              # STM32CubeMX project metadata descriptor
    │   │   ├── Core/                   # HAL Core application layer (Inc/ & Src/)
    │   │   │   ├── Inc/main.h, stm32f4xx_it.h
    │   │   │   └── Src/main.c, stm32f4xx_it.c, system_stm32f4xx.c
    │   │   ├── Drivers/                # CMSIS & STM32F4xx HAL Driver libraries
    │   │   ├── MDK-ARM/                # Keil MDK-ARM µVision project folder
    │   │   │   ├── TASK12B.uvprojx      # Keil µVision project file
    │   │   │   └── startup_stm32f401xe.s # ARM Cortex-M4 vector table & startup
    │   │   ├── circuit.png             # Task hardware schematic diagram
    │   │   └── README.md               # Task technical report & inferences
    │   ├── TASK12C/                     # Dedicated Task: Short-Press vs Long-Press Classifier
    │   │   ├── TASK12C.ioc              # STM32CubeMX configuration file
    │   │   ├── .mxproject              # STM32CubeMX project metadata descriptor
    │   │   ├── Core/                   # HAL Core application layer (Inc/ & Src/)
    │   │   │   ├── Inc/main.h, stm32f4xx_it.h
    │   │   │   └── Src/main.c, stm32f4xx_it.c, system_stm32f4xx.c
    │   │   ├── Drivers/                # CMSIS & STM32F4xx HAL Driver libraries
    │   │   ├── MDK-ARM/                # Keil MDK-ARM µVision project folder
    │   │   │   ├── TASK12C.uvprojx      # Keil µVision project file
    │   │   │   └── startup_stm32f401xe.s # ARM Cortex-M4 vector table & startup
    │   │   ├── circuit.png             # Task hardware schematic diagram
    │   │   └── README.md               # Task technical report & inferences
    │   ├── circuit.png             # CAT12 complete hardware schematic
    │   └── README.md               # CAT12 evaluation overview
    │
    ├── CAT13/                           # Continuous Lab Evaluation-13: BME280 Acquisition & HTTP Cloud Ingestion
    │   ├── TASK13A/                     # Dedicated Task: BME280 I2C Hardware Bring-Up & Bosch API Integration
    │   │   ├── TASK13A.ioc              # STM32CubeMX configuration file
    │   │   ├── .mxproject              # STM32CubeMX project metadata descriptor
    │   │   ├── Core/                   # HAL Core application layer (Inc/ & Src/)
    │   │   │   ├── Inc/bme280.h, bme280_defs.h, main.h, stm32f4xx_it.h
    │   │   │   └── Src/bme280.c, main.c, stm32f4xx_it.c, system_stm32f4xx.c
    │   │   ├── Drivers/                # CMSIS & STM32F4xx HAL Driver libraries
    │   │   ├── MDK-ARM/                # Keil MDK-ARM µVision project folder
    │   │   │   ├── TASK13A.uvprojx      # Keil µVision project file
    │   │   │   └── startup_stm32f401xe.s # ARM Cortex-M4 vector table & startup
    │   │   ├── circuit.png             # Task hardware schematic diagram
    │   │   └── README.md               # Task technical report & inferences
    │   ├── TASK13B/                     # Dedicated Task: Dynamic JSON Payload Generation & HTTP Header Formatting
    │   │   ├── TASK13B.ioc              # STM32CubeMX configuration file
    │   │   ├── .mxproject              # STM32CubeMX project metadata descriptor
    │   │   ├── Core/                   # HAL Core application layer (Inc/ & Src/)
    │   │   │   ├── Inc/bme280.h, bme280_defs.h, main.h, stm32f4xx_it.h
    │   │   │   └── Src/bme280.c, main.c, stm32f4xx_it.c, system_stm32f4xx.c
    │   │   ├── Drivers/                # CMSIS & STM32F4xx HAL Driver libraries
    │   │   ├── MDK-ARM/                # Keil MDK-ARM µVision project folder
    │   │   │   ├── TASK13B.uvprojx      # Keil µVision project file
    │   │   │   └── startup_stm32f401xe.s # ARM Cortex-M4 vector table & startup
    │   │   ├── circuit.png             # Task hardware schematic diagram
    │   │   └── README.md               # Task technical report & inferences
    │   ├── TASK13C/                     # Dedicated Task: Node-RED Cloud Ingestion Pipeline & Statistical Telemetry
    │   │   ├── TASK13C.ioc              # STM32CubeMX configuration file
    │   │   ├── .mxproject              # STM32CubeMX project metadata descriptor
    │   │   ├── Core/                   # HAL Core application layer (Inc/ & Src/)
    │   │   │   ├── Inc/bme280.h, bme280_defs.h, main.h, stm32f4xx_it.h
    │   │   │   └── Src/bme280.c, main.c, stm32f4xx_it.c, system_stm32f4xx.c
    │   │   ├── Drivers/                # CMSIS & STM32F4xx HAL Driver libraries
    │   │   ├── MDK-ARM/                # Keil MDK-ARM µVision project folder
    │   │   │   ├── TASK13C.uvprojx      # Keil µVision project file
    │   │   │   └── startup_stm32f401xe.s # ARM Cortex-M4 vector table & startup
    │   │   ├── circuit.png             # Task hardware schematic diagram
    │   │   └── README.md               # Task technical report & inferences
    │   ├── circuit.png             # CAT13 complete hardware schematic
    │   └── README.md               # CAT13 evaluation overview
    │
    └── CAT14/                           # Continuous Lab Evaluation-14: Environmental Sensing & MQTT Client API (ESPLib)
        ├── TASK14/                      # Dedicated Task: End-to-End Environmental Sensing (BME280) - MQTT Client (ESPLib)
        │   ├── TASK14.ioc              # STM32CubeMX configuration file
        │   ├── .mxproject              # STM32CubeMX project metadata descriptor
        │   ├── Core/                   # HAL Core application layer (Inc/ & Src/)
        │   │   ├── Inc/main.h, stm32f4xx_it.h
        │   │   └── Src/main.c, stm32f4xx_it.c, system_stm32f4xx.c
        │   ├── Drivers/                # CMSIS & STM32F4xx HAL Driver libraries
        │   ├── MDK-ARM/                # Keil MDK-ARM µVision project folder
        │   │   ├── TASK14.uvprojx      # Keil µVision project file
        │   │   └── startup_stm32f401xe.s # ARM Cortex-M4 vector table & startup
        │   ├── circuit.png             # Task hardware schematic diagram
        │   └── README.md               # Task technical report & inferences
        ├── TASK14A/                     # Dedicated Task: BME280 I2C Environmental Sensing & Compensation
        │   ├── TASK14A.ioc             # STM32CubeMX configuration file
        │   ├── .mxproject              # STM32CubeMX project metadata descriptor
        │   ├── Core/                   # HAL Core application layer (Inc/ & Src/)
        │   │   ├── Inc/main.h, stm32f4xx_it.h
        │   │   └── Src/main.c, stm32f4xx_it.c, system_stm32f4xx.c
        │   ├── Drivers/                # CMSIS & STM32F4xx HAL Driver libraries
        │   ├── MDK-ARM/                # Keil MDK-ARM µVision project folder
        │   │   ├── TASK14A.uvprojx     # Keil µVision project file
        │   │   └── startup_stm32f401xe.s # ARM Cortex-M4 vector table & startup
        │   ├── circuit.png             # Task hardware schematic diagram
        │   └── README.md               # Task technical report & inferences
        ├── TASK14B/                     # Dedicated Task: ESP8266 MQTT Client API & Cloud Telemetry
        │   ├── TASK14B.ioc             # STM32CubeMX configuration file
        │   ├── .mxproject              # STM32CubeMX project metadata descriptor
        │   ├── Core/                   # HAL Core application layer (Inc/ & Src/)
        │   │   ├── Inc/main.h, stm32f4xx_it.h
        │   │   └── Src/main.c, stm32f4xx_it.c, system_stm32f4xx.c
        │   ├── Drivers/                # CMSIS & STM32F4xx HAL Driver libraries
        │   ├── MDK-ARM/                # Keil MDK-ARM µVision project folder
        │   │   ├── TASK14B.uvprojx     # Keil µVision project file
        │   │   └── startup_stm32f401xe.s # ARM Cortex-M4 vector table & startup
        │   ├── circuit.png             # Task hardware schematic diagram
        │   └── README.md               # Task technical report & inferences
        ├── circuit.png             # CAT14 complete hardware schematic
        └── README.md               # CAT14 evaluation overview
```

---

## 3. Submission Guidelines

### 3.1 Folder Organization

- Separate directories are maintained for each hardware platform (8051/ and STM32/).
- Each Continuous Assessment evaluation has a dedicated parent folder (CAT2 through CAT14).
- Every individual task is isolated within its own dedicated subfolder (TASKxA, TASKxB, etc.).
- Uniform directory hierarchy and standardized naming are preserved across all 40 tasks.

### 3.2 Required Documentation

Every experiment and task folder contains a README.md file following the prescribed evaluation rubric:

| Field | Description |
|---|---|
| **EXP** | Continuous Assessment experiment identifier (e.g. CONTINUOUS ASSESMENT 2) |
| **DATE** | Date of experiment execution (DD/MM/YYYY) |
| **NAME OF EXP** | Official title of the experiment from the syllabus |
| **HARDWARE SETUP / PLATFORM** | Microcontroller development board, peripherals, and toolchain used |
| **TASK NO** | Experiment task identifier and title (e.g. TASK 2A : Hardware Board Bring-Up) |
| **Circuit Diagram** | Hardware connection summary and embedded link (![Circuit Diagram](circuit.png)) |
| **Core Logic / Pseudocode / Code Base** | Working principle, step-by-step pseudocode, and key register/HAL API explanation |
| **INFERENCE** | Technical observations, timing measurements, and conclusions |

### 3.3 Circuit Diagram Requirements

The circuit diagram must clearly indicate:

- Development board used (Atmel AT89S52, STM32 Blue Pill, STM32 NUCLEO-F401RE).
- Microcontroller IC and packaging.
- GPIO pins, bus connections, and communication lines used.
- External peripherals (LEDs, 7-segment display, 4x4 matrix keypad, LCD, stepper motor, BME280, ESP8266).
- Direct connections between components, power rails (+5V / +3.3V), and ground (GND).

All circuit schematics are saved inside each respective folder as circuit.png and embedded directly in the README.md.

### 3.4 Source Code and Project Files

Each task folder contains the complete, compilable source code and project configuration files required to open, understand, and reproduce the experiment:

**8051 Microcontroller (Bare-Metal):**
- Embedded C source files (*.c).
- Keil µVision project files (*.uvproj).
- Required startup files (STARTUP.A51).
- Compiled firmware binaries in Objects/ (*.hex).

**STM32 Microcontroller (ARM Cortex-M & HAL):**
- STM32CubeMX configuration file (*.ioc) and .mxproject descriptor.
- Application source and header files (Core/Src/ and Core/Inc/).
- Required HAL & CMSIS driver libraries (Drivers/).
- Keil MDK-ARM µVision project folder (MDK-ARM/*.uvprojx) and startup vector table (startup_*.s).

---

## 4. README Format

Every experiment and task strictly adheres to the standardized documentation format:

`markdown
# EXPERIMENT DETAILS

**EXP:** CONTINUOUS ASSESMENT <N>
**DATE:** <DD/MM/YYYY>
**NAME OF EXP:** <Experiment Title>
**HARDWARE SETUP / PLATFORM:** <Board & Peripherals>

---

## TASK <ID> : <Task Title>

### 1. Circuit Diagram
- **Development Board / Core:** ...
- **Microcontroller IC:** ...
- **GPIO Pin(s) / Peripherals:** ...
- **Power Supply / Interface:** ...

![Circuit Diagram](circuit.png)

### 2. Core Logic / Pseudocode / Code Base
**Working Principle:** ...
**Pseudocode:** ...
**Code Base:** ...

### 3. Inference
...
`

---

## 5. General Instructions

1. Maintain the prescribed folder structure across all platforms.
2. Ensure every task and evaluation has its own standalone README.md and circuit.png.
3. Use meaningful and consistent file and folder names conforming to course conventions.
4. Include all necessary project, startup, and source files.
5. Ensure circuit diagrams are clear, correctly labeled, and embedded.
6. Verify all projects build cleanly without errors.
7. Keep the GitHub repository public and accessible to the course evaluator.

---

## 6. Master Index of Continuous Lab Evaluations (CAT 2 to CAT 14 — 40 Tasks)

### 6.1 Course Evaluation Syllabus & Experiment Overview

| Exp Identifier | Date | Name of Experiment | Hardware Setup / Platform | Subdivisions / Dedicated Task Folders | Status |
|:---:|:---:|---|---|---|:---:|
| **[CAT 2](8051/CAT2/)** | 20/07/2026 | 8051 Tool Chain Setup & Hardware Bring-Up | AT89S52 + Keil µVision + USB-ISP | • [TASK 2A: Hardware Board Bring-Up](8051/CAT2/TASK2A/)<br>• [TASK 2B: 1 Hz LED Blink on Port 2](8051/CAT2/TASK2B/)<br>• [TASK 2C: Delay Library Function](8051/CAT2/TASK2C/) | **PASSED** |
| **[CAT 3](8051/CAT3/)** | 27/07/2026 | Timer-Based LED Pattern Generator & Button Controller | AT89S52 + 4 LEDs + Push-Button | • [TASK 3A: Mode Switch Controller](8051/CAT3/TASK3A/)<br>• [TASK 3B: Binary Counter](8051/CAT3/TASK3B/)<br>• [TASK 3C: Alternating Pattern](8051/CAT3/TASK3C/)<br>• [TASK 3D: All-LED Flash](8051/CAT3/TASK3D/) | **PASSED** |
| **[CAT 4](8051/CAT4/)** | 03/08/2026 | Human-Machine Interface using Keypad, LEDs & 7-Seg | AT89S52 + 4x4 Keypad + 7-Segment + 4 LEDs | • [TASK 4A: Keypad Scanning HMI](8051/CAT4/TASK4A/)<br>• [TASK 4B: 7-Segment Output](8051/CAT4/TASK4B/)<br>• [TASK 4C: Keypad LED Patterns](8051/CAT4/TASK4C/) | **PASSED** |
| **[CAT 5](8051/CAT5/)** | 10/08/2026 | Hardware Timer & Timing for Fading, Pulse, & Stepper | AT89S52 + Timer 0 + DSO + ULN2003 + Stepper | • [TASK 5A: 1ms Timer 0 ISR Driver](8051/CAT5/TASK5A/)<br>• [TASK 5B.1: PWM Triangular Wave Modulation](8051/CAT5/TASK5B/TASK5B.1/)<br>• [TASK 5B.2: PWM Carrier Frequency Analysis](8051/CAT5/TASK5B/TASK5B.2/)<br>• [TASK 5B.3: Multi-LED Breathing Controller](8051/CAT5/TASK5B/TASK5B.3/)<br>• [TASK 5C: Stepper Motor Full-Step Driver](8051/CAT5/TASK5C/) | **PASSED** |
| **[CAT 6](8051/CAT6/)** | 17/08/2026 | UART Driver and Serial Debugging | AT89S52 + USB-TTL Bridge + PuTTY Terminal | • [TASK 6A: UART String Non-Blocking TX](8051/CAT6/TASK6A/)<br>• [TASK 6B: Terminal Echo & Circular Ring Buffer](8051/CAT6/TASK6B/) | **PASSED** |
| **[CAT 7](8051/CAT7/)** | 24/08/2026 | 16×2 LCD Driver Development & Dynamic Display Control | AT89S52 + HD44780 16×2 LCD + 4×4 Keypad | • [TASK 7A: HD44780 LCD 4-Bit Driver](8051/CAT7/TASK7A/)<br>• [TASK 7B: Cursor Positioning & Dynamic Counter](8051/CAT7/TASK7B/)<br>• [TASK 7C: 4x4 Keypad Interactive Menu](8051/CAT7/TASK7C/) | **PASSED** |
| **[CAT 8](STM32/CAT8/)** | 21/09/2026 | STM32 GPIO Bring-Up and Switch-Controlled LED | STM32 Blue Pill (STM32F103C8T6) + Keil MDK | • [TASK 8A: GPIO Direct Follow Mode](STM32/CAT8/TASK8A/)<br>• [TASK 8B: Debounced Toggle Mode](STM32/CAT8/TASK8B/)<br>• [TASK 8C: Press Duration Classifier](STM32/CAT8/TASK8C/) | **PASSED** |
| **[CAT 9](STM32/CAT9/)** | 28/09/2026 | STM32 Hardware Timer Interrupts & PWM Generation | STM32 NUCLEO-F401RE + DSO | • [TASK 9A: Timer 2 Periodic Interrupt (1 Hz Blink)](STM32/CAT9/TASK9A/)<br>• [TASK 9B: Timer PWM Generation Variable Duty](STM32/CAT9/TASK9B/) | **PASSED** |
| **[CAT 10](STM32/CAT10/)** | 05/10/2026 | STM32 USART Serial Communication Modes | STM32 NUCLEO-F401RE + PuTTY Terminal | • [TASK 10A: USART2 Polling String Transmission](STM32/CAT10/TASK10A/)<br>• [TASK 10B: USART2 Interrupt-Driven Echo](STM32/CAT10/TASK10B/)<br>• [TASK 10C: USART2 DMA Circular Streaming](STM32/CAT10/TASK10C/) | **PASSED** |
| **[CAT 11](STM32/CAT11/)** | 12/10/2026 | HTTP Server: STM32–Wemos Wi-Fi Modem Using AT Commands | STM32 NUCLEO-F401RE + Wemos D1 (ESP8266) | • [TASK 11A: ESP8266 TCP Server Configuration](STM32/CAT11/TASK11A/)<br>• [TASK 11B: HTTP Request Parser & Static HTML Response](STM32/CAT11/TASK11B/)<br>• [TASK 11C: Node-RED HTTP Client Ingestion](STM32/CAT11/TASK11C/) | **PASSED** |
| **[CAT 12](STM32/CAT12/)** | 19/10/2026 | STM32F401RE Cortex-M4: GPIO & User Input Programming | STM32 NUCLEO-F401RE (STM32F401RET6) | • [TASK 12A: User LED LD2 Bring-Up (PA5)](STM32/CAT12/TASK12A/)<br>• [TASK 12B: Push Button B1 Latching State](STM32/CAT12/TASK12B/)<br>• [TASK 12C: Press Duration Classifier](STM32/CAT12/TASK12C/) | **PASSED** |
| **[CAT 13](STM32/CAT13/)** | 19/10/2026 | BME280 Data Acquisition & HTTP Cloud Ingestion | STM32 NUCLEO-F401RE + BME280 + ESP8266 | • [TASK 13A: BME280 Bosch Driver Integration](STM32/CAT13/TASK13A/)<br>• [TASK 13B: JSON Formulation & HTTP POST](STM32/CAT13/TASK13B/)<br>• [TASK 13C: Node-RED Pipeline & Analytics](STM32/CAT13/TASK13C/) | **PASSED** |
| **[CAT 14](STM32/CAT14/)** | 27/10/2026 | BME280 Interfacing (I2C) & MQTT Cloud Analytics | STM32 NUCLEO-F401RE + BME280 + ESP8266 + Node-RED | • [TASK 14: Integrated Smart Edge Node](STM32/CAT14/TASK14/)<br>• [TASK 14A: BME280 I2C Sensing](STM32/CAT14/TASK14A/)<br>• [TASK 14B: MQTT Cloud Analytics](STM32/CAT14/TASK14B/) | **PASSED** |

---

### 6.2 Task-Level Verification Matrix (40 Tasks)

#### Part I: 8051 Microcontroller (AT89S52 Bare-Metal — 20 Tasks)

| Task | Evaluated Directory | Circuit Diagram | Documentation | Firmware Hex | Evaluation Status |
|---|---|:---:|:---:|:---:|:---:|
| **CAT 2 - TASK 2A** | [8051/CAT2/TASK2A/](8051/CAT2/TASK2A/) | [circuit.png](8051/CAT2/TASK2A/circuit.png) | [README.md](8051/CAT2/TASK2A/README.md) | TASK2A.hex | **PASSED** |
| **CAT 2 - TASK 2B** | [8051/CAT2/TASK2B/](8051/CAT2/TASK2B/) | [circuit.png](8051/CAT2/TASK2B/circuit.png) | [README.md](8051/CAT2/TASK2B/README.md) | TASK2B.hex | **PASSED** |
| **CAT 2 - TASK 2C** | [8051/CAT2/TASK2C/](8051/CAT2/TASK2C/) | [circuit.png](8051/CAT2/TASK2C/circuit.png) | [README.md](8051/CAT2/TASK2C/README.md) | TASK2C.hex | **PASSED** |
| **CAT 3 - TASK 3A** | [8051/CAT3/TASK3A/](8051/CAT3/TASK3A/) | [circuit.png](8051/CAT3/TASK3A/circuit.png) | [README.md](8051/CAT3/TASK3A/README.md) | TASK3A.hex | **PASSED** |
| **CAT 3 - TASK 3B** | [8051/CAT3/TASK3B/](8051/CAT3/TASK3B/) | [circuit.png](8051/CAT3/TASK3B/circuit.png) | [README.md](8051/CAT3/TASK3B/README.md) | TASK3B.hex | **PASSED** |
| **CAT 3 - TASK 3C** | [8051/CAT3/TASK3C/](8051/CAT3/TASK3C/) | [circuit.png](8051/CAT3/TASK3C/circuit.png) | [README.md](8051/CAT3/TASK3C/README.md) | TASK3C.hex | **PASSED** |
| **CAT 3 - TASK 3D** | [8051/CAT3/TASK3D/](8051/CAT3/TASK3D/) | [circuit.png](8051/CAT3/TASK3D/circuit.png) | [README.md](8051/CAT3/TASK3D/README.md) | TASK3D.hex | **PASSED** |
| **CAT 4 - TASK 4A** | [8051/CAT4/TASK4A/](8051/CAT4/TASK4A/) | [circuit.png](8051/CAT4/TASK4A/circuit.png) | [README.md](8051/CAT4/TASK4A/README.md) | TASK4A.hex | **PASSED** |
| **CAT 4 - TASK 4B** | [8051/CAT4/TASK4B/](8051/CAT4/TASK4B/) | [circuit.png](8051/CAT4/TASK4B/circuit.png) | [README.md](8051/CAT4/TASK4B/README.md) | TASK4B.hex | **PASSED** |
| **CAT 4 - TASK 4C** | [8051/CAT4/TASK4C/](8051/CAT4/TASK4C/) | [circuit.png](8051/CAT4/TASK4C/circuit.png) | [README.md](8051/CAT4/TASK4C/README.md) | TASK4C.hex | **PASSED** |
| **CAT 5 - TASK 5A** | [8051/CAT5/TASK5A/](8051/CAT5/TASK5A/) | [circuit.png](8051/CAT5/TASK5A/circuit.png) | [README.md](8051/CAT5/TASK5A/README.md) | TASK5A.hex | **PASSED** |
| **CAT 5 - TASK 5B.1** | [8051/CAT5/TASK5B/TASK5B.1/](8051/CAT5/TASK5B/TASK5B.1/) | [circuit.png](8051/CAT5/TASK5B/TASK5B.1/circuit.png) | [README.md](8051/CAT5/TASK5B/TASK5B.1/README.md) | TASK5B_1.hex | **PASSED** |
| **CAT 5 - TASK 5B.2** | [8051/CAT5/TASK5B/TASK5B.2/](8051/CAT5/TASK5B/TASK5B.2/) | [circuit.png](8051/CAT5/TASK5B/TASK5B.2/circuit.png) | [README.md](8051/CAT5/TASK5B/TASK5B.2/README.md) | TASK5B_2.hex | **PASSED** |
| **CAT 5 - TASK 5B.3** | [8051/CAT5/TASK5B/TASK5B.3/](8051/CAT5/TASK5B/TASK5B.3/) | [circuit.png](8051/CAT5/TASK5B/TASK5B.3/circuit.png) | [README.md](8051/CAT5/TASK5B/TASK5B.3/README.md) | TASK5B_3.hex | **PASSED** |
| **CAT 5 - TASK 5C** | [8051/CAT5/TASK5C/](8051/CAT5/TASK5C/) | [circuit.png](8051/CAT5/TASK5C/circuit.png) | [README.md](8051/CAT5/TASK5C/README.md) | TASK5C.hex | **PASSED** |
| **CAT 6 - TASK 6A** | [8051/CAT6/TASK6A/](8051/CAT6/TASK6A/) | [circuit.png](8051/CAT6/TASK6A/circuit.png) | [README.md](8051/CAT6/TASK6A/README.md) | TASK6A.hex | **PASSED** |
| **CAT 6 - TASK 6B** | [8051/CAT6/TASK6B/](8051/CAT6/TASK6B/) | [circuit.png](8051/CAT6/TASK6B/circuit.png) | [README.md](8051/CAT6/TASK6B/README.md) | TASK6B.hex | **PASSED** |
| **CAT 7 - TASK 7A** | [8051/CAT7/TASK7A/](8051/CAT7/TASK7A/) | [circuit.png](8051/CAT7/TASK7A/circuit.png) | [README.md](8051/CAT7/TASK7A/README.md) | TASK7A.hex | **PASSED** |
| **CAT 7 - TASK 7B** | [8051/CAT7/TASK7B/](8051/CAT7/TASK7B/) | [circuit.png](8051/CAT7/TASK7B/circuit.png) | [README.md](8051/CAT7/TASK7B/README.md) | TASK7B.hex | **PASSED** |
| **CAT 7 - TASK 7C** | [8051/CAT7/TASK7C/](8051/CAT7/TASK7C/) | [circuit.png](8051/CAT7/TASK7C/circuit.png) | [README.md](8051/CAT7/TASK7C/README.md) | TASK7C.hex | **PASSED** |

#### Part II: STM32 Microcontroller (ARM Cortex-M & HAL — 20 Tasks)

| Task | Evaluated Directory | Circuit Diagram | Documentation | Project Files | Evaluation Status |
|---|---|:---:|:---:|:---:|:---:|
| **CAT 8 - TASK 8A** | [STM32/CAT8/TASK8A/](STM32/CAT8/TASK8A/) | [circuit.png](STM32/CAT8/TASK8A/circuit.png) | [README.md](STM32/CAT8/TASK8A/README.md) | TASK8A.ioc, MDK-ARM/ | **PASSED** |
| **CAT 8 - TASK 8B** | [STM32/CAT8/TASK8B/](STM32/CAT8/TASK8B/) | [circuit.png](STM32/CAT8/TASK8B/circuit.png) | [README.md](STM32/CAT8/TASK8B/README.md) | TASK8B.ioc, MDK-ARM/ | **PASSED** |
| **CAT 8 - TASK 8C** | [STM32/CAT8/TASK8C/](STM32/CAT8/TASK8C/) | [circuit.png](STM32/CAT8/TASK8C/circuit.png) | [README.md](STM32/CAT8/TASK8C/README.md) | TASK8C.ioc, MDK-ARM/ | **PASSED** |
| **CAT 9 - TASK 9A** | [STM32/CAT9/TASK9A/](STM32/CAT9/TASK9A/) | [circuit.png](STM32/CAT9/TASK9A/circuit.png) | [README.md](STM32/CAT9/TASK9A/README.md) | TASK9A.ioc, MDK-ARM/ | **PASSED** |
| **CAT 9 - TASK 9B** | [STM32/CAT9/TASK9B/](STM32/CAT9/TASK9B/) | [circuit.png](STM32/CAT9/TASK9B/circuit.png) | [README.md](STM32/CAT9/TASK9B/README.md) | TASK9B.ioc, MDK-ARM/ | **PASSED** |
| **CAT 10 - TASK 10A** | [STM32/CAT10/TASK10A/](STM32/CAT10/TASK10A/) | [circuit.png](STM32/CAT10/TASK10A/circuit.png) | [README.md](STM32/CAT10/TASK10A/README.md) | TASK10A.ioc, MDK-ARM/ | **PASSED** |
| **CAT 10 - TASK 10B** | [STM32/CAT10/TASK10B/](STM32/CAT10/TASK10B/) | [circuit.png](STM32/CAT10/TASK10B/circuit.png) | [README.md](STM32/CAT10/TASK10B/README.md) | TASK10B.ioc, MDK-ARM/ | **PASSED** |
| **CAT 10 - TASK 10C** | [STM32/CAT10/TASK10C/](STM32/CAT10/TASK10C/) | [circuit.png](STM32/CAT10/TASK10C/circuit.png) | [README.md](STM32/CAT10/TASK10C/README.md) | TASK10C.ioc, MDK-ARM/ | **PASSED** |
| **CAT 11 - TASK 11A** | [STM32/CAT11/TASK11A/](STM32/CAT11/TASK11A/) | [circuit.png](STM32/CAT11/TASK11A/circuit.png) | [README.md](STM32/CAT11/TASK11A/README.md) | TASK11A.ioc, MDK-ARM/ | **PASSED** |
| **CAT 11 - TASK 11B** | [STM32/CAT11/TASK11B/](STM32/CAT11/TASK11B/) | [circuit.png](STM32/CAT11/TASK11B/circuit.png) | [README.md](STM32/CAT11/TASK11B/README.md) | TASK11B.ioc, MDK-ARM/ | **PASSED** |
| **CAT 11 - TASK 11C** | [STM32/CAT11/TASK11C/](STM32/CAT11/TASK11C/) | [circuit.png](STM32/CAT11/TASK11C/circuit.png) | [README.md](STM32/CAT11/TASK11C/README.md) | TASK11C.ioc, MDK-ARM/ | **PASSED** |
| **CAT 12 - TASK 12A** | [STM32/CAT12/TASK12A/](STM32/CAT12/TASK12A/) | [circuit.png](STM32/CAT12/TASK12A/circuit.png) | [README.md](STM32/CAT12/TASK12A/README.md) | TASK12A.ioc, MDK-ARM/ | **PASSED** |
| **CAT 12 - TASK 12B** | [STM32/CAT12/TASK12B/](STM32/CAT12/TASK12B/) | [circuit.png](STM32/CAT12/TASK12B/circuit.png) | [README.md](STM32/CAT12/TASK12B/README.md) | TASK12B.ioc, MDK-ARM/ | **PASSED** |
| **CAT 12 - TASK 12C** | [STM32/CAT12/TASK12C/](STM32/CAT12/TASK12C/) | [circuit.png](STM32/CAT12/TASK12C/circuit.png) | [README.md](STM32/CAT12/TASK12C/README.md) | TASK12C.ioc, MDK-ARM/ | **PASSED** |
| **CAT 13 - TASK 13A** | [STM32/CAT13/TASK13A/](STM32/CAT13/TASK13A/) | [circuit.png](STM32/CAT13/TASK13A/circuit.png) | [README.md](STM32/CAT13/TASK13A/README.md) | TASK13A.ioc, MDK-ARM/ | **PASSED** |
| **CAT 13 - TASK 13B** | [STM32/CAT13/TASK13B/](STM32/CAT13/TASK13B/) | [circuit.png](STM32/CAT13/TASK13B/circuit.png) | [README.md](STM32/CAT13/TASK13B/README.md) | TASK13B.ioc, MDK-ARM/ | **PASSED** |
| **CAT 13 - TASK 13C** | [STM32/CAT13/TASK13C/](STM32/CAT13/TASK13C/) | [circuit.png](STM32/CAT13/TASK13C/circuit.png) | [README.md](STM32/CAT13/TASK13C/README.md) | TASK13C.ioc, MDK-ARM/ | **PASSED** |
| **CAT 14 - TASK 14** | [STM32/CAT14/TASK14/](STM32/CAT14/TASK14/) | [circuit.png](STM32/CAT14/TASK14/circuit.png) | [README.md](STM32/CAT14/TASK14/README.md) | TASK14.ioc, MDK-ARM/ | **PASSED** |
| **CAT 14 - TASK 14A** | [STM32/CAT14/TASK14A/](STM32/CAT14/TASK14A/) | [circuit.png](STM32/CAT14/TASK14A/circuit.png) | [README.md](STM32/CAT14/TASK14A/README.md) | TASK14A.ioc, MDK-ARM/ | **PASSED** |
| **CAT 14 - TASK 14B** | [STM32/CAT14/TASK14B/](STM32/CAT14/TASK14B/) | [circuit.png](STM32/CAT14/TASK14B/circuit.png) | [README.md](STM32/CAT14/TASK14B/README.md) | TASK14B.ioc, MDK-ARM/ | **PASSED** |
---

## 7. Hardware Platform Specifications & Network Configuration

### 7.1 Microcontroller Platforms
- **8051 Development System:** Microchip/Atmel AT89S52 (40-Pin DIP, 8-bit MCS-51 core @ 11.0592 MHz, $T_{mach} \approx 1.085\,\mu\text{s}$, 8 KB Flash).
- **STM32 Development Systems:** 
  - STM32 Blue Pill (`STM32F103C8T6`, ARM Cortex-M3 @ 72 MHz, 64 KB Flash, 20 KB SRAM).
  - STM32 NUCLEO-F401RE (`STM32F401RET6`, ARM Cortex-M4 with FPU @ 84 MHz, 512 KB Flash, 96 KB SRAM, integrated ST-LINK/V2-1 debugger).

### 7.2 Wi-Fi & MQTT Credentials (CAT 11, 13, 14)
- **Wi-Fi Access Point SSID:** `SNUC`
- **Wi-Fi WPA2 Passphrase:** `snu12345`
- **MQTT Public Broker:** `broker.emqx.io` (TCP Port 1883)
- **Primary MQTT Topics:**
  - Environmental Telemetry: `stm32/test/data`

