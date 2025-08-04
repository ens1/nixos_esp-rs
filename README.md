# ESP32 Rust Development Environment with Nix

This repository contains a `shell.nix` file that sets up a complete development environment for building and flashing Rust applications on ESP32 microcontrollers. It uses the Nix package manager to ensure a reproducible and consistent environment across different machines.

## Prerequisites

Before you begin, you must have the [Nix package manager](https://nixos.org/download.html) installed on your system (Linux or macOS).

## How to Use

1. **Clone the repository** or place the `shell.nix` file in your project's root directory.

2. **Open your terminal** and navigate to the project directory.

3. **Start the development shell** by running the following command:

   ```bash
   nix-shell
   
   
This command will download all the specified dependencies and configure the environment. The first time you run it, it may take a while. Subsequent runs will be much faster as the dependencies will be cached.

Once inside the shell, you'll have access to all the necessary tools like rustc, cargo, espflash, and the ESP-IDF toolchain.
