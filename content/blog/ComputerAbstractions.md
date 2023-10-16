---
title: "Computer Abstractions"
date: 2023-10-07T7:27:00-04:00
draft: false
---

Starting with a blank computer consisting solely of hardware, let’s break down what is inherently provided, what’s managed by external utilities, and what needs to be implemented manually:

### Provided by Hardware:

1. **CPU**: Executes instructions (machine code).
2. **Memory**: Stores data and instructions.
3. **I/O Ports**: Interfaces for communication with external devices/peripherals.
4. **Buses**: Allows communication between different hardware components.
5. **Clock**: Provides timing signals to synchronize operations.

### Managed by Firmware/BIOS:

1. **Boot Sequence**: Initializes hardware components and loads the operating system.
2. **Device Configuration**: Sets up basic configurations for hardware components.
3. **Hardware Abstraction**: Offers an interface for the operating system to interact with hardware without knowing the specifics.
4. **Interrupt Handling**: Manages hardware interrupts and passes them to the operating system.

### Operating System (OS):

1. **Device Drivers**: Facilitates communication between the OS and specific hardware devices.
2. **Memory Management**: Allocates and deallocates memory spaces as required by different processes.
3. **File System**: Organizes and manages files on storage devices.
4. **Process Management**: Manages the execution of processes, including scheduling, prioritization, and multitasking.
5. **Security & Permissions**: Controls access to system resources.
6. **Networking Stack**: Manages network communications and protocols.

### User/Developer:

1. **Application Development**: Creating software applications using programming languages and development tools.
2. **Middleware/Services**: Developing or utilizing additional software components that facilitate communication and input/output between different software applications.
3. **Database Management**: Implementing and managing databases to store, organize, and retrieve data.
4. **User Interface**: Designing and implementing the user interface for software applications.
5. **Business Logic**: Implementing the core functionality and logic of the application.
6. **Security**: Ensuring the application and data are secure from unauthorized access and vulnerabilities.

### Embedded Systems/FPGAs:

In the case of starting with a blank FPGA or an embedded system without an OS, additional layers must be implemented manually:

1. **Hardware Configuration**: Defining the hardware logic (using HDLs like Verilog/VHDL) for FPGAs or configuring microcontroller peripherals.
2. **Bare-Metal Programming**: Writing software directly interacting with hardware (without OS) for embedded systems.
3. **Real-Time Operating System (RTOS)**: Optionally, implementing or using an RTOS for managing tasks in real-time.

The user/developer is responsible for implementing specific functionalities and applications, building upon the foundations provided by hardware, firmware, OS, and any additional libraries or tools utilized. In the context of FPGAs and embedded systems, the developer has more responsibilities as they are closer to the hardware level.