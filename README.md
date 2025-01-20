# JHeapster - Rust-Powered JVM Heap Monitoring CLI

**JHeapster** is a lightweight **command-line interface (CLI)** tool written in **Rust**, utilizing **JNI** and **JVM TI** (Java Virtual Machine Tool Interface) to dynamically attach to a running JVM and provide real-time insights into heap memory usage and garbage collection (GC) performance.

This project is primarily a **personal learning tool** and **boilerplate** to demonstrate the use of **JNI** and **JVM TI** for JVM heap monitoring.



It is designed to provide basic heap memory metrics directly in the terminal, without exporting the data to files for the time being.

## Key Objectives !

- **Exploration of JVM Internals**: Dive into the internals of the **JVM** to understand memory management, garbage collection (GC), and performance optimization from a native code perspective.
- **JNI and JVM TI Integration**: Experiment with **JNI** (Java Native Interface) and **JVM TI** (Java Virtual Machine Tool Interface) to directly interact with a running JVM process and gather memory metrics in real-time.
- **Heap Memory and Garbage Collection (GC) Monitoring**: Explore how to monitor and analyze heap memory usage, as well as track and measure the performance impact of garbage collection cycles.
- **Bytecode Interaction**: Learn how to manipulate and interact with Java bytecodes from native Rust code to extend JVM functionality.
- **Personal Exploration Tool**: Build a personal project to better understand the inner workings of the JVM, including memory management, garbage collection, and native code interactions.
- **Real-time Terminal Output**: Focus on displaying heap memory and GC metrics directly in the terminal for hands-on exploration, without exporting data (for now).

## Key Features

- **Dynamic JVM Attachment**: Attach to a running JVM without requiring a restart, using **JNI** and **JVM TI**.
- **Heap Monitoring**: Collect and display real-time memory metrics including:
    - Total heap memory
    - Used heap memory
    - Free heap memory
    - Garbage collection (GC) cycles (minor and major)
    - GC impact on performance
- **Educational Project**: Learn and demonstrate the mechanics of **JNI** and **JVM TI** to interface with the JVM.
- **Terminal Output**: Metrics are displayed directly in the terminal for real-time monitoring, with no data export (for now).

## Getting Started

### Usage

#### Identify Target JVM

List all running JVM processes:
```bash
jps -l
```

Find the target JVM’s Process ID (PID).
Attach to JVM

Run JHeapster with the identified PID:
```bash
./jheapster --pid <PID>
```

This command will attach JHeapster to the running JVM process and start displaying heap metrics in the terminal.

### View Metrics

The tool will display real-time memory metrics directly in the terminal, including:

- Total heap memory
- Used heap memory
- Free heap memory
- Garbage collection cycles and their impact

# Licence
Apache License
Version 2.0, January 2004

Copyright (c) Allemand Sébastien

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

**Special Condition:**

This software is licensed for **personal use and non-commercial projects only**.
If you wish to use this software for **commercial purposes**, you **must contact the author** for explicit permission.
