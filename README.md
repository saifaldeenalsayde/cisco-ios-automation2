Multi-Router Interface & OSPF Configuration Tool
This Python script automates the process of configuring multiple interfaces and OSPF settings across Cisco IOS devices using Netmiko. It also generates Excel reports of the interface status and OSPF brief information using Pandas and TextFSM.

🚀 Features
Interactive CLI: Prompts for credentials and configuration details per router.

Dynamic Interface Config: Allows adding multiple interfaces (Physical or Loopback) in one session.

Smart OSPF Logic: Automatically handles passive-interface and network commands based on interface type.

Auto-Reporting: Exports show ip interface brief and show ip ospf interface brief to Excel files for documentation.

Error Handling: Manages SSH authentication and timeout exceptions gracefully.

🛠 Prerequisites
Before running the script, ensure you have the following installed:

Python 3.x

Netmiko

Pandas

Openpyxl (for Excel export)

TextFSM (for parsing command output)

pip install netmiko pandas openpyxl textfsm
📋 How to Use

Run the script:

Follow the prompts: Input your credentials and the configuration details when asked.

📂 Output
The script generates two Excel files:

int br to[router].xlsx: Contains the interface status brief.

ospf int_report.xlsx: Contains the OSPF interface brief.

Note: Make sure the destination paths (e.g., D:\int br inventory\) exist on your machine or modify them in the script.
