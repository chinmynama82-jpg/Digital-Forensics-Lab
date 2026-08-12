# Experiment 1: Evidence Acquisition Using AccessData FTK Imager

## Aim

To acquire volatile memory and create a forensic image of a physical storage device using AccessData FTK Imager, followed by verification of the acquired evidence.

## Software Required

* AccessData FTK Imager 3.1.2.0
* Windows operating system

## Procedure

### Step 1: Open FTK Imager

Launch **AccessData FTK Imager** on the system.

From the **File** menu, select **Capture Memory** to begin volatile memory acquisition.

**Screenshot:** Capture Memory option

---

### Step 2: Configure Memory Capture

In the **Memory Capture** window, specify the destination location and filename for the memory dump.

The available options can be configured according to the acquisition requirement, including the pagefile and AD1 file options.

**Screenshot:** Memory Capture settings

---

### Step 3: Start Memory Acquisition

Click **Capture Memory** to start collecting the system's volatile memory.

Wait while FTK Imager acquires the RAM and displays the progress of the operation.

**Screenshot:** Memory acquisition progress

---

### Step 4: Open Disk Imaging

After the memory acquisition workflow, open the disk imaging function.

From the **File** menu, select **Create Disk Image**.

**Screenshot:** Create Disk Image option

---

### Step 5: Select the Evidence Source

Select the appropriate source type for the disk acquisition.

Choose **Physical Drive** when the complete physical storage device is required for acquisition.

**Screenshot:** Evidence source selection

---

### Step 6: Select the Physical Drive

Select the required physical drive from the list of available drives.

Click **Finish** to continue with the image creation process.

**Screenshot:** Physical drive selection

---

### Step 7: Configure the Forensic Image

Enter the required evidence and case information.

Select the required image format and enable **Verify images after they are created** so that the acquired image can be checked after creation.

**Screenshot:** Image configuration

---

### Step 8: Specify the Image Destination

Select the location where the forensic image will be stored.

Enter the image filename and configure the fragment size according to the storage requirement.

**Screenshot:** Image destination settings

---

### Step 9: Start the Disk Acquisition

Review the configured settings and start the acquisition.

FTK Imager creates the forensic image of the selected physical drive and displays the acquisition progress.

---

### Step 10: Verify the Acquired Evidence

After the acquisition is completed, check the generated acquisition information and hash values.

The verification process is used to confirm the integrity of the acquired forensic image.

## Result

The volatile memory acquisition and physical disk imaging procedures were successfully performed using **AccessData FTK Imager**. The acquired evidence was verified using hash values to confirm its integrity.
