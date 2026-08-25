# TestDisk Forensic Recovery Experiment

## Experiment Title

**Recover deleted or damaged files from a storage device using TestDisk**

## Aim

To recover and verify a missing or damaged partition and its
files from a storage device using TestDisk.

## Tool Used

- TestDisk 7.2
- Windows
- 2 GB Virtual Test Disk
- NTFS File System

## Objective

The objective of this experiment is to understand how TestDisk
can be used to:

- Analyse a storage device
- Identify missing partitions
- Search for lost partitions
- Verify detected partitions
- List files from a partition
- Recover partition information
- Verify recovered files

## Safety Precaution

The experiment was performed on a **2 GB virtual test disk**
instead of the actual laptop storage.

This was done to avoid accidental modification or data loss
on the actual system disk.

# Procedure

### Step 1: Launch TestDisk


The TestDisk application was extracted and `testdisk_win`
was executed as Administrator.

The **Create** option was selected to create a new log file.
<img width="1208" height="727" alt="Screenshot 2026-08-25 203604" src="https://github.com/user-attachments/assets/5140642c-968f-403b-9612-1f93349b7c24" />

### Step 2: Select the Storage Device

The available storage devices were displayed by TestDisk.

The **2 GB virtual test disk** was selected and
**Proceed** was chosen.
<img width="1127" height="692" alt="Screenshot 2026-08-25 214037" src="https://github.com/user-attachments/assets/1f5ae055-d3bc-4155-9558-8d27f6967709" />

### Step 3: Select Partition Table Type

The **Intel/PC (MBR)** partition table type was selected
for the virtual test disk.
<img width="1132" height="642" alt="Screenshot 2026-08-25 214111" src="https://github.com/user-attachments/assets/0f601e83-1b18-4454-9ad7-d4804cdf51f8" />

### Step 4: Analyse the Disk

The **Analyse** option was selected to examine the current
partition structure and search for missing partitions.
<img width="1137" height="642" alt="Screenshot 2026-08-25 214139" src="https://github.com/user-attachments/assets/3f0285e6-4d7a-4ac6-8003-ec3d8631dda7" />


### Step 5: Perform Quick Search

The **Quick Search** option was selected.

TestDisk scanned the virtual disk and identified the
NTFS partition.
<img width="1108" height="650" alt="Screenshot 2026-08-25 214206" src="https://github.com/user-attachments/assets/426ee8ce-e134-4349-aa57-670a23088ecf" />


### Step 6: Verify the Partition

The detected partition was displayed as:

`L HPFS - NTFS [TestDiskLab]`
<img width="1131" height="662" alt="Screenshot 2026-08-25 214247" src="https://github.com/user-attachments/assets/f28668d3-f671-44d2-86e8-c8a9be9ef6a0" />


The partition was selected for verification.

### Step 7: List Files

The **P** key was used to list the files present in the
detected partition.

The evidence/test file:

`Evidence1.txt.txt`
<img width="1917" height="1078" alt="Screenshot 2026-08-25 213528" src="https://github.com/user-attachments/assets/618269e9-54a3-4cf2-9113-4836a8f0ff03" />

was successfully displayed.

### Step 8: Perform Deeper Search

The **Deeper Search** option was performed to conduct a
more thorough search of the storage device.

The detected partition was verified again.
<img width="1113" height="640" alt="Screenshot 2026-08-25 214513" src="https://github.com/user-attachments/assets/54c360a5-2433-43f0-aabd-9eeaa83c17ff" />

### Step 9: Write Partition Information

After verifying the correct partition, the **Write** option
was selected.

TestDisk displayed a confirmation message asking whether
the partition table should be written.

The operation was confirmed using **Y**.
<img width="1097" height="632" alt="Screenshot 2026-08-25 214916" src="https://github.com/user-attachments/assets/89ec068a-8013-435f-9a44-64c4bf9aa85f" />

### Step 10: Exit TestDisk

After the partition information was written successfully,
the TestDisk application was exited using the Quit option.

# Final Output

The TestDisk directory listing displayed:

`Evidence1.txt.txt`

This confirmed that the NTFS partition was successfully
identified and its file structure was accessible.
<img width="1176" height="657" alt="Screenshot 2026-08-25 214317" src="https://github.com/user-attachments/assets/051412cf-5d42-4c60-be24-7f324a2cae78" />

## Result

**TestDisk successfully analysed the virtual storage device,
identified the NTFS partition, and displayed the evidence/test
file `Evidence1.txt.txt`.**

## Conclusion

TestDisk is a useful open-source forensic recovery utility
for analysing storage devices, identifying lost partitions,
listing files, and recovering partition information.

The experiment was safely performed using a virtual test disk
to avoid modifying the actual laptop storage.

