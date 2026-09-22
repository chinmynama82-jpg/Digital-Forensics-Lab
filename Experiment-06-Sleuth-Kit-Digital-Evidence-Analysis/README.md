# Experiment 6 – Use Sleuth Kit to Analyze Digital Evidence

## Aim

To analyze a forensic disk image using The Sleuth Kit and examine the partition structure, file system, files, metadata, and recover a file from the digital evidence.

## Tools Required

- The Sleuth Kit 4.14.0
- Windows Command Prompt
- Windows File Explorer
- Forensic Disk Image (`4Dell Latitude CPI.E01`)

## Evidence Used

**Evidence File:** `4Dell Latitude CPI.E01`

## Steps

### Step 1 – Identify Partition Structure

The `mmls` command was used to identify the partition structure of the forensic disk image.

**Command:**

cmd
mmls "C:\Users\ASUS\Downloads\4Dell Latitude CPI.E01"

<img width="1481" height="762" alt="Screenshot 2026-09-22 201054" src="https://github.com/user-attachments/assets/553438ad-cc59-427a-80b1-67158003d610" />

Step 2 – Analyze File System

The fsstat command was used to obtain detailed information about the file system.

Command:

fsstat -o 63 "C:\Users\ASUS\Downloads\4Dell Latitude CPI.E01"


<img width="1901" height="1015" alt="Screenshot 2026-09-22 201145" src="https://github.com/user-attachments/assets/643c2205-6c1a-482a-b9d8-6accd7ef675f" />

Step 3 – List Files and Directories

The fls command was used to list files and directories available in the forensic disk image.

Command:

fls -o 63 -r "C:\Users\ASUS\Downloads\4Dell Latitude CPI.E01"

The command displayed the files and directories present in the file system. The required file airplane.bmp was identified from the file listing.

<img width="1901" height="1018" alt="Screenshot 2026-09-22 201410" src="https://github.com/user-attachments/assets/660cad84-7ffc-40fd-bd0d-d36d7242c985" />


### Step 4 – Analyze File Metadata

The `istat` command was used to examine the metadata of the identified file through its Master File Table (MFT) entry.

**Command:**

```cmd
istat -o 63 "C:\Users\ASUS\Downloads\4Dell Latitude CPI.E01" 5665

### Step 5 – Recover the Identified File

The `icat` command was used to recover the identified file from the forensic disk image using its MFT entry number.

**Command:**

```cmd
icat -o 63 "C:\Users\ASUS\Downloads\4Dell Latitude CPI.E01" 5665 > "C:\Users\ASUS\Downloads\DF_Output\airplane.bmp"

<img width="941" height="81" alt="Screenshot 2026-09-22 201542" src="https://github.com/user-attachments/assets/b01057ab-9746-4887-be58-e7fb41bc9914" />


Step 6 – Verify the Recovered File

The recovered airplane.bmp file was located in the DF_Output folder and opened using Windows File Explorer.

The image was displayed successfully, confirming that the file was recovered from the forensic disk image.

<img width="1486" height="758" alt="Screenshot 2026-09-22 202035" src="https://github.com/user-attachments/assets/ee377998-b639-40b1-847f-03fb7a303ac5" />
<img width="960" height="1017" alt="Screenshot 2026-09-22 202117" src="https://github.com/user-attachments/assets/919994ae-4ff6-49ff-ab24-1b139b3b33fb" />

Result

The forensic disk image was successfully analyzed using The Sleuth Kit. The partition structure and NTFS file system were examined, files and directories were listed, file metadata was analyzed, and airplane.bmp was successfully recovered.
