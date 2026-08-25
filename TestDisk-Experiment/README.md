# TestDisk Forensic Recovery Experiment

## Experiment Title

**Recover deleted or damaged files from a storage device using TestDisk**

## Aim

To analyse a storage device using TestDisk, identify the
NTFS partition, search the partition structure, and perform
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
- Identify an NTFS partition
- Search for partitions
- Verify the detected partition
- Perform deeper partition search
- Write partition information

## Safety Precaution

The experiment was performed on a **2 GB virtual test disk**
instead of the actual laptop storage.

This was done to avoid accidental modification or data loss
on the actual system disk.

# Procedure

### Step 1: Start TestDisk

The TestDisk application was opened and the **Create** option
was selected to create a new log file.

**Output:**

![TestDisk Start](screenshots/01_TestDisk_Start.png)

---

### Step 2: Select the Test Disk

TestDisk displayed the available storage devices.

The **2 GB virtual test disk** was selected and
**Proceed** was chosen.

**Output:**

![Disk Selection](screenshots/02_Disk_Selection.png)

---

### Step 3: Select Partition Table Type

TestDisk detected the partition table type.

The **Intel/PC** partition table type was selected for the
virtual test disk.

**Output:**

![Partition Table](screenshots/03_Partition_Table.png)

---

### Step 4: Analyse the Partition Structure

The **Analyse** option was selected to examine the partition
structure of the virtual disk.

**Output:**

![Analyse](screenshots/04_Analyse.png)

---

### Step 5: Search and Identify the Partition

The **Quick Search** option was used to search for partitions.

The NTFS partition **TestDiskLab** was detected.

The partition was then verified using the available
TestDisk options.

**Output:**

![Quick Search](screenshots/05_Quick_Search.png)

---

### Step 6: Perform Deeper Search

The **Deeper Search** option was performed to conduct a more
thorough search of the virtual disk.

The detected partition was verified again.

**Output:**

![Deeper Search](screenshots/06_Deeper_Search.png)

---

## Final Output

The TestDisk partition recovery procedure was completed on
the 2 GB virtual test disk.

## Result

**TestDisk successfully analysed the virtual disk, identified
the NTFS partition, performed partition searching, and
completed the partition recovery operation.**

## Conclusion

The experiment demonstrated the use of TestDisk for analysing
a storage device and recovering/validating partition
information in a controlled forensic environment.

The practical was performed on a virtual test disk to prevent
accidental modification of the actual laptop storage.
