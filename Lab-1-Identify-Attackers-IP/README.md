Lab 1: Identify the Attacker's IP

Objective

Investigate network traffic using Wireshark to identify suspicious activity and determine the attacker's IP address.

Task 1: Packet Capture

Question: How many packets did Wireshark capture?

Observation: The initial packet capture displayed packets numbered from 1 to 309.

Answer: 309 packets.

Evidence

Screenshot of the initial Wireshark packet capture will be added here.

Status

Task 1 completed. Remaining tasks are in progress.

Learning Outcome

Learned how to observe packet numbers in Wireshark and understand the initial network traffic capture.

Task 2: Identify TCP SYN Packets

Objective

Identify packets that initiate TCP connections using the SYN flag.

Wireshark Filter

tcp.flags.syn == 1

Result

Answer: 73 packets

Analysis

The Wireshark display filter was used to isolate TCP packets with the SYN flag set. These packets are associated with the initiation of TCP connections.

Evidence

Screenshot of the filtered Wireshark traffic.

Status

Completed.

Task 3: Identify the Attacker's IP Address

Objective

Identify the IP address responsible for sending a large number of TCP SYN packets consecutively.

Wireshark Filter

tcp.flags.syn == 1

Result

Attacker's IP Address: "192.168.10.66"

Analysis

The network traffic was analyzed to identify the source IP address sending an unusually large number of TCP SYN packets in succession.

The IP address "192.168.10.66" was identified as the suspected attacker based on the repeated SYN packet activity.

Evidence

Screenshot showing the repeated TCP SYN packets originating from "192.168.10.66".

Status

Completed.
