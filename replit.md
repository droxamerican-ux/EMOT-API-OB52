# EMOT-API-OB52

## Overview
This is a Python console bot application (EMOT-API-OB52) for game automation using protobuf communication. It handles TCP connections for chat and online functionality.

## Project Structure
- `main.py` - Main entry point with async TCP connections
- `xC4.py` - Cryptographic utilities (AES encryption/decryption, protobuf handling)
- `xHeaders.py` - HTTP headers and API request functions
- `Pb2/` - Protobuf compiled Python files for message serialization

## Running the Application
The application runs as a console application using `python main.py`. It will:
1. Attempt to authenticate via external APIs
2. Establish TCP connections for chat and online features
3. Continuously run with automatic reconnection on errors

## Dependencies
- aiohttp - Async HTTP client
- pycryptodome - AES encryption
- protobuf & protobuf-decoder - Protocol buffer handling
- requests - HTTP client
- pyjwt - JWT token handling
- cfonts - Console fonts for display
- psutil, pytz, urllib3 - Utilities

## Notes
- This is a console-only application (no web interface)
- Runtime errors about TCP connections are normal if authentication credentials are invalid or API is unavailable
- The app will continuously retry on connection failures
