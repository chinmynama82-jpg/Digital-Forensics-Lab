# TestDisk Forensic Recovery Experiment

## Experiment Title

**Recover deleted or damaged files from a storage device using TestDisk**

## Aim

To analyse a storage device using TestDisk, identify the
required partition, verify its file structure, and perform
partition recovery operations.

## Tool Used

- TestDisk 7.2
- Windows
- 2 GB Virtual Test Disk
- NTFS File System

## Objective

The objective of this experiment is to understand how TestDisk
can be used to:

- Analyse a storage device
- Identify partitions
- Search for lost or damaged partitions
- Verify detected partitions
- List files from a partition
- Recover partition information
- Verify the file system structure

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
<img width="1148" height="677" alt="Screenshot 2026-08-25 213719" src="https://github.com/user-attachments/assets/96751c3e-a601-46ec-838e-3eddcf573971" />

### Step 2: Select the Storage Device

The available storage devices were displayed by TestDisk.

The **2 GB virtual test disk** was selected and
**Proceed** was chosen.
<img width="1127" height="692" alt="Screenshot 2026-08-25 214037" src="https://github.com/user-attachments/assets/2d120f75-a36a-4704-b04d-d483e3d1efef" />


### Step 3: Select Partition Table Type

The **Intel/PC (MBR)** partition table type was selected
for the virtual test disk.
<img width="1132" height="642" alt="Screenshot 2026-08-25 214111" src="https://github.com/user-attachments/assets/dca39a5e-c25b-44d6-9a2c-e6647b101547" />


### Step 4: Analyse the Disk

The **Analyse** option was selected to examine the current
partition structure and search for partitions.
<img width="1137" height="642" alt="Screenshot 2026-08-25 214139" src="https://github.com/user-attachments/assets/f5420b7e-7983-448c-a0a5-75b338ddd858" />


### Step 5: Perform Quick Search

The **Quick Search** option was selected.

TestDisk scanned the virtual disk and identified the
NTFS partition.
<img width="1108" height="650" alt="Screenshot 2026-08-25 214206" src="https://github.com/user-attachments/assets/b45c7578-cdf0-401c-ba26-488e4a22c404" />


### Step 6: Verify the Partition

The detected partition was displayed as:

`L HPFS - NTFS [TestDiskLab]`

The partition was selected for verification.
<img width="1131" height="662" alt="Screenshot 2026-08-25 214247" src="https://github.com/user-attachments/assets/19af069d-a48a-43b3-9ade-68c0d8cb7f3b" />



### Step 7: List Files

The **P** key was used to list the files present in the
detected partition.

TestDisk displayed the directory structure and available
files in the partition.
<img width="1118" height="656" alt="Screenshot 2026-08-25 214446" src="https://github.com/user-attachments/assets/0eebae8e-2ed1-4538-b7c2-7f3a41f6a836" />


### Step 8: Perform Deeper Search

The **Deeper Search** option was performed to conduct a
more thorough search of the storage device.

The detected partition was verified again.
<img width="1113" height="640" alt="Screenshot 2026-08-25 214513" src="https://github.com/user-attachments/assets/47513e8f-1a9d-4430-bf15-109861d9255e" />



### Step 9: Write Partition Information

After verifying the correct partition, the **Write** option
was selected.

TestDisk displayed a confirmation message asking whether
the partition table should be written.

The operation was confirmed using **Y**.
<img width="1097" height="632" alt="Screenshot 2026-08-25 214916" src="https://github.com/user-attachments/assets/e4fcd525-feb3-42e8-aa99-119d4fd894de" />



### Step 10: Exit TestDisk

After the partition information was written successfully,
the TestDisk application was exited using the Quit option.

<img width="1102" height="637" alt="Screenshot 2026-08-25 214944" src="https://github.com/user-attachments/assets/097ee1d9-4e61-4c23-9429-528015cc6804" />

# Final Output

The final TestDisk file-listing screen was used to verify
that the detected NTFS partition and its file structure
were accessible.
<img width="1106" height="643" alt="Screenshot 2026-08-25 214617" src="https://github.com/user-attachments/assets/1189f01a-c0d3-450b-92bf-bff28d9aced2" />


## Result

**TestDisk successfully analysed the virtual storage device,
identified the NTFS partition, verified its file structure,
and completed the partition recovery workflow.**

## Conclusion

TestDisk is a useful open-source forensic recovery utility
for analysing storage devices, identifying partitions,
searching for lost partitions, listing files, and recovering
partition information.

The experiment was safely performed using a virtual test disk
to avoid modifying the actual laptop storage.

