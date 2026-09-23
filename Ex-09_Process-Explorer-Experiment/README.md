# Ex.No.9 – Use Process Explorer to Identify Suspicious Processes

## Aim

To use Microsoft Sysinternals Process Explorer to examine running Windows processes and identify potentially suspicious processes by checking process details, executable path, digital signature, registered services, CPU usage, and memory usage.

## Tools Required

- Windows 10/11
- Microsoft Sysinternals Process Explorer

## Procedure

### Step 1: Launch Process Explorer

The Microsoft Sysinternals Process Explorer was downloaded and extracted. The `procexp64.exe` application was opened to display the running processes on the system.

---

### Step 2: View Running Processes

The Process Explorer main window displayed the running processes in a hierarchical process tree.

The following details were visible:

- Process Name
- CPU Usage
- Private Bytes
- Working Set
- Process ID (PID)
- Description
- Company Name

<img width="982" height="742" alt="image" src="https://github.com/user-attachments/assets/7dff9c8c-9b9e-4f3c-98b3-5648a9bf6f8e" />


---

### Step 3: Select a Process

The `svchost.exe` process with **PID 1888** was selected for examination.

The process was displayed under `services.exe`.

---

### Step 4: Check Process Properties

The Properties window of `svchost.exe` was opened.

The following information was observed:

- **Process:** `svchost.exe`
- **PID:** `1888`
- **Description:** Host Process for Windows Services
- **Version:** `10.0.26100.8737`
- **Path:** `C:\Windows\System32\svchost.exe`
- **Command Line:** `C:\Windows\system32\svchost.exe -k DcomLaunch -p`
- **Parent:** `services.exe (1732)`

<img width="558" height="760" alt="image" src="https://github.com/user-attachments/assets/9f516cd6-7b2e-43ad-8b09-1684b9e9ddac" />


---

### Step 5: Verify Digital Signature

The process was verified using the **Verify** option in the Properties window.

The result displayed:

**(Verified) Microsoft Windows Publisher**

This indicates that the selected executable was verified as being published by Microsoft Windows.

<img width="556" height="761" alt="image" src="https://github.com/user-attachments/assets/de4d6d06-9cff-4c21-8511-6b4d53755364" />

---

### Step 6: Check Registered Services

The **Services** tab was opened to examine the services registered under the selected `svchost.exe` process.

The following services were observed:

| Service | Display Name | Path |
|---|---|---|
| BrokerInfrastructure | Background Tasks Infrastructure Service | `C:\Windows\System32\psmsrv.dll` |
| DcomLaunch | DCOM Server Process Launcher | `C:\Windows\system32\rpcss.dll` |
| PlugPlay | Plug and Play | `C:\Windows\system32\umpnpmgr.dll` |
| Power | Power | `C:\Windows\system32\umpo.dll` |
| SystemEventsBroker | System Events Broker | `C:\Windows\System32\SystemEventsBrokerServer.dll` |

<img width="831" height="287" alt="image" src="https://github.com/user-attachments/assets/d75e18e0-4de2-458f-b3fa-0380b27d2818" />


---

### Step 7: Observe CPU and Memory Usage

The Process Explorer main window was examined to observe the resource usage of the selected process.

The observed values for `svchost.exe` were approximately:

- **CPU:** `<0.01%`
- **Private Bytes:** `13,024 K`
- **Working Set:** `41,516 K`
- **PID:** `1888`
- **Description:** Host Process for Windows Services
- **Company Name:** Microsoft Corporation

<img width="1037" height="738" alt="image" src="https://github.com/user-attachments/assets/9a5f577e-6c30-45e4-a5c2-06b688becbee" />


---

### Step 8: Analyze the Process

The selected `svchost.exe` process was analyzed based on its process name, executable path, digital signature, company name, registered services, CPU usage, and memory usage.

The executable was located in:

`C:\Windows\System32\svchost.exe`

The process was verified as:

**Microsoft Windows Publisher**

The process was associated with standard Windows services and no obvious suspicious indicators were observed during the examination.

---
### Step 9: Process Control Options

The Process Explorer context menu was opened for the selected process. The following options were available:

- Kill Process
- Kill Process Tree
- Restart
- Suspend
- Create Dump

<img width="978" height="406" alt="Screenshot 2026-09-23 200516" src="https://github.com/user-attachments/assets/bcbb6817-abc0-4104-9f17-724e780e8578" />


The **Kill Process** option was not used because the examined `svchost.exe` process did not show any obvious malicious or suspicious indicators. The process had a valid Microsoft Windows publisher signature, was located in the Windows System32 directory, and was associated with standard Windows services. Therefore, terminating the process was not necessary for this experiment.


## Observation

The `svchost.exe` process with PID 1888 was examined using Microsoft Sysinternals Process Explorer. The process path, digital signature, company information, registered services, CPU usage, and memory usage were checked.

The process was located in the Windows System32 directory and was verified as **Microsoft Windows Publisher**.

## Result

Microsoft Sysinternals Process Explorer was successfully used to examine a running Windows process and identify potential suspicious indicators. The examined `svchost.exe` process showed characteristics consistent with a legitimate Windows system process, and no obvious suspicious indicators were observed during the examination.
