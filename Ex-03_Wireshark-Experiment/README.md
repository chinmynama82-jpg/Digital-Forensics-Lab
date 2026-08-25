# Ex. No. 03 – Wireshark Network Traffic Analysis

## Aim

To capture and analyse network packets using Wireshark and
identify HTTP traffic and POST requests from the captured
network communication.

## Tool Used

- Wireshark
- Windows
- Wi-Fi Network Interface

## Objective

The objectives of this experiment are:

- To capture network traffic using Wireshark.
- To identify different network protocols.
- To filter HTTP packets.
- To analyse HTTP requests.
- To examine a POST request and its packet details.

# Procedure

## Step 1: Start Wireshark Packet Capture

Wireshark was opened and packet capturing was started on the
Wi-Fi network interface.

The captured packets were displayed in the packet list with
information such as source, destination, protocol, length,
and packet details.

<img width="1918" height="1079" alt="image" src="https://github.com/user-attachments/assets/0e39be35-63e9-4dfe-8ad1-7bb6692b6977" />




---

## Step 2: Apply HTTP Display Filter

The HTTP display filter was entered in the Wireshark filter bar:

```text
http
```

The filter displayed the HTTP packets captured during the
network communication.

<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/8f397010-ee00-4616-a6e1-ea84c5f327ac" />

---

## Step 3: Identify the HTTP POST Request

The captured HTTP traffic was examined to identify a POST
request.

The packet list showed a POST request to:

```text
/login.xml
```

The selected packet contained HTTP request information.
<img width="1542" height="856" alt="image" src="https://github.com/user-attachments/assets/bce50872-6325-4b71-a250-9530106ffe9d" />


---

## Step 4: Inspect POST Request Details

The POST packet was opened to inspect its detailed HTTP
information.

The packet details showed:

- Ethernet information
- IP information
- TCP information
- HTTP information
- Form-encoded request data

The captured request was examined as part of the controlled
laboratory experiment.

<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/8ec80f31-681b-4450-8f85-d126f758cee8" />



---

# Observation

Wireshark successfully captured network packets from the
selected Wi-Fi interface.

After applying the `http` filter, HTTP packets were isolated
from the captured traffic.

A POST request to `/login.xml` was identified and its HTTP
packet details were inspected.

# Result

**Wireshark was successfully used to capture network traffic,
filter HTTP packets, identify a POST request, and analyse its
packet-level information.**

# Conclusion

This experiment demonstrated how Wireshark can be used for
network traffic analysis and digital forensic investigation.

The captured packets can be examined at different protocol
layers to understand the communication between network hosts.

