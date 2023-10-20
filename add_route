#!/usr/bin/env python3

import subprocess

destination_network_1 = "192.168.10.0/24"
destination_network_2 = "192.168.20.0/24"
destination_network_3 = "192.168.30.0/24"

gateway_ip = "10.8.8.1"

command_1 = ["sudo", "route", "-n", "add", destination_network_1, gateway_ip]
command_2 = ["sudo", "route", "-n", "add", destination_network_2, gateway_ip]
command_3 = ["sudo", "route", "-n", "add", destination_network_3, gateway_ip]

try:
    subprocess.run(command_1, check=True)
    print("Route added network_1 successfully.")
    subprocess.run(command_2, check=True)
    print("Route added network_2 successfully.")
    subprocess.run(command_3, check=True)
    print("Route added network_3 successfully.")

except subprocess.CalledProcessError as e:
    print(f"Error: {e}")
