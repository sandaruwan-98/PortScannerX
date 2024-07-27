# PortScannerX

PortScannerX is a Python-based tool designed to scan all ports (from 1 to 65535) on a specified target IP address and identify open ports. This tool utilizes threading to speed up the scanning process.

## How It Works

1. **Import Necessary Libraries**:
    - `socket`: For creating network connections.
    - `threading`: For concurrent execution of port scans.

2. **Port Scanning Function**:
    - `scan_port(ip, port, open_ports)`: Attempts to connect to the given port on the specified IP address. If the connection is successful, the port is added to the `open_ports` list.

3. **Port Range Scanning Function**:
    - `scan_ports(ip, start_port, end_port)`: Iterates through the specified range of ports, starts a new thread for each port, and limits the number of active threads to avoid overwhelming the system.

4. **Main Execution Block**:
    - Prompts the user for the target IP address.
    - Calls `scan_ports` to perform the scan and prints the open ports.

## Features

- Scans all ports (1-65535) on a specified IP address.
- Identifies open ports using socket connections.
- Utilizes threading for faster scanning.
- Limits the number of active threads to optimize system performance.

## Usage

1. Clone the repository:

2. Navigate to the project directory:

3. Run the script:

4. Enter the target IP address when prompted.

5. View the list of open ports.

## Requirements

- Python 3.x

## Contributing

Feel free to submit pull requests or open issues to improve this project.

## Author

Nipun Sandaruwan
