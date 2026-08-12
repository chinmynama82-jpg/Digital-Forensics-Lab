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

<img width="1296" height="761" alt="image" src="https://github.com/user-attachments/assets/6a30cf85-4340-40cc-9f45-0a41b393c9d0" />

---

### Step 2: Configure Memory Capture

In the **Memory Capture** window, specify the destination location and filename for the memory dump.

The available options can be configured according to the acquisition requirement, including the pagefile and AD1 file options.

**Screenshot:** Memory Capture settings

<img width="1600" height="840" alt="image" src="https://github.com/user-attachments/assets/c2a22144-9745-42b9-91ed-64623c60e841" />


---

### Step 3: Start Memory Acquisition

Click **Capture Memory** to start collecting the system's volatile memory.

Wait while FTK Imager acquires the RAM and displays the progress of the operation.

**Screenshot:** Memory acquisition progress
<img width="1917" height="1002" alt="image" src="https://github.com/user-attachments/assets/4e4e7f7e-12f8-45a4-98ed-e803782ad5ca" />


---

### Step 4: Open Disk Imaging

After the memory acquisition workflow, open the disk imaging function.

From the **File** menu, select **Create Disk Image**.

**Screenshot:** Create Disk Image option
<img width="1600" height="803" alt="WhatsApp Image 2026-08-12 at 10 07 25 PM" src="https://github.com/user-attachments/assets/5c117dd8-7c14-4a99-98e9-1a34581dada3" />


---

### Step 5: Select the Evidence Source

Select the appropriate source type for the disk acquisition.

Choose **Physical Drive** when the complete physical storage device is required for acquisition.

**Screenshot:** Evidence source selection
<img width="1600" height="833" alt="WhatsApp Image 2026-08-12 at 10 07 39 PM" src="https://github.com/user-attachments/assets/0ce1c716-b402-4d5d-80a4-30e7421a87e8" />


---

### Step 6: Select the Physical Drive

Select the required physical drive from the list of available drives.

Click **Finish** to continue with the image creation process.

**Screenshot:** Physical drive selection
<img width="1600" height="831" alt="WhatsApp Image 2026-08-12 at 10 08 19 PM" src="https://github.com/user-attachments/assets/b2327810-87a3-45ef-b084-ea105b9bbed8" />


---

### Step 7: Configure the Forensic Image

Enter the required evidence and case information.

Select the required image format and enable **Verify images after they are created** so that the acquired image can be checked after creation.

**Screenshot:** Image configuration
<img width="1600" height="831" alt="WhatsApp Image 2026-08-12 at 10 08 31 PM" src="https://github.com/user-attachments/assets/40645799-2213-40ca-9aed-9763e419dd1b" />


---

### Step 8: Specify the Image Destination

Select the location where the forensic image will be stored.

Enter the image filename and configure the fragment size according to the storage requirement.

**Screenshot:** Image destination settings

<img width="1600" height="836" alt="WhatsApp Image 2026-08-12 at 10 09 38 PM" src="https://github.com/user-attachments/assets/8549a8d2-1b32-4021-b98a-909334430c83" />

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
