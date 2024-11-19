# EEG Data Streaming with Go and C++

## Project Overview
This project integrates Go and C++ using CGO to connect with EEG headsets and retrieve data streams using `liblsl` (Lab Streaming Layer). It demonstrates how to discover, connect to, and pull data from available EEG streams, printing the output for analysis or further processing.

## Features
- Discover all available EEG streams on the network.
- Connect to a selected stream and pull real-time data.
- Print detailed stream information, including channel labels and types.
- Display received data in a labeled, easy-to-read format.

## Technologies Used
- **Go**: Used as the main language for running the program and calling C++ functions.
- **C++**: Handles the complex task of resolving streams and pulling data using `liblsl`.
- **CGO**: Enables Go to call C++ functions and link necessary libraries.
- **liblsl**: A library for real-time data streaming and synchronization.
- **POSIX Threads**: Used for multi-threading when needed.

## Installation and Setup

### Prerequisites
- Go installed (version 1.16 or higher).
- A C++ compiler (e.g., `g++`).
- `liblsl` installed on your system.
- `libpthread` library (usually included with standard Linux/Unix systems).

### Installation Steps
1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/eeg-streaming.git
   cd eeg-streaming
