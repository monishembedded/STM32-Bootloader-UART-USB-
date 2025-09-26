# STM32-Bootloader-UART-USB-
 # STM32 Bootloader (UART/USB + CRC)

This project implements a reliable bootloader for STM32 (tested on STM32F103C8T6).
Features:
- UART/USB firmware update
- CRC integrity check
- Flash erase & write
- Jump to main application

## Repository Structure
- `bootloader/` → Bootloader source code
- `application/` → Example application code
- `tools/` → Python uploader script
- `docs/` → Documentation + diagrams

## Bootloader Flow
1. Bootloader starts on reset
2. Waits for update command
3. If received → Downloads new firmware via UART/USB
4. Verifies CRC
5. Writes firmware to Flash
6. Jumps to main application

## Getting Started
- Flash `bootloader` first
- Use Python script to upload new firmware
- Bootloader will run and jump to your application

