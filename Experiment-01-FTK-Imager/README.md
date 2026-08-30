EXPERIMENT – 01
Evidence Acquisition Using AccessData FTK Imager
AIM

To acquire volatile memory and create a forensic image of a physical storage device using AccessData FTK Imager, followed by verification of the acquired evidence.

SOFTWARE REQUIRED
AccessData FTK Imager
Windows Operating System
Adequate storage space for the acquired evidence image
PROCEDURE
Step 1: Open FTK Imager

Launch AccessData FTK Imager with the required administrative privileges.

From the File menu, select Capture Memory to begin volatile memory acquisition.

<img width="1455" height="743" alt="Screenshot 2026-08-30 115157" src="https://github.com/user-attachments/assets/3be890fb-d48d-4adb-8aef-d0104dc3bc44" />
<img width="342" height="495" alt="Screenshot 2026-08-30 115213" src="https://github.com/user-attachments/assets/29fd53ce-c1d1-40f6-b932-03c4eb2cb5d4" />


Step 2: Configure Memory Capture

In the Memory Capture window, specify the destination folder and filename for the RAM dump. Select the required options and ensure that sufficient storage space is available.
<img width="442" height="381" alt="image" src="https://github.com/user-attachments/assets/71c61049-aa50-4d66-bc5c-a6497daa1f39" />


Step 3: Start Memory Acquisition

Click Capture Memory to start collecting the contents of physical memory. Wait until the acquisition completes successfully and record the output filename and location.

<img width="610" height="318" alt="Screenshot 2026-08-30 115436" src="https://github.com/user-attachments/assets/e3aac298-16b5-4eb5-ba57-b9828bb937f2" />


Step 4: Open Disk Imaging

After completing the memory acquisition, select:

File → Create Disk Image

The disk imaging wizard opens for source selection, image configuration and verification.

<img width="1112" height="716" alt="Screenshot 2026-08-30 120600" src="https://github.com/user-attachments/assets/a2bd564d-7fb9-411b-bcc6-26d2130d11d1" />

## Step 5: Select and Configure the Evidence Source

In the Evidence Source Selection window, select **Logical Drive**.

For this experiment, **Logical Drive** was selected instead of **Physical Drive** because the objective was to acquire the specific logical volume (**D:\**) rather than the entire physical storage device. This avoids acquiring unnecessary data from other partitions or areas of the physical disk and reduces the required storage space and acquisition time.

Next, select **D:\ (New Volume [NTFS])** from the available logical drives and click **Finish** to continue.

<img width="602" height="455" alt="Screenshot 2026-08-30 121342" src="https://github.com/user-attachments/assets/17b8eed1-df9f-4b61-a78c-07e410bbcb23" />
<img width="637" height="442" alt="Screenshot 2026-08-30 121323" src="https://github.com/user-attachments/assets/3aa1711d-274d-4a9e-8c11-1ddafc2461ad" />

---

## Step 6: Configure Evidence Information

In the Evidence Item Information window, enter the required information such as case number, evidence number, unique description, examiner name, and notes where applicable.

This information helps identify and document the acquired forensic evidence.

<img width="557" height="445" alt="Screenshot 2026-08-30 121747" src="https://github.com/user-attachments/assets/99bd5ef6-845f-4a49-9526-4fe97a4fdab9" />

---

## Step 7: Select the Image Type and Configure Destination

Select **Raw (dd)** as the forensic image format.

Specify the destination folder and configure the image settings. For this experiment, the following settings were used:

- **Image Filename:** `memdump_EX01`
- **Image Fragment Size:** `1500 MB`
- **Compression:** `0`
- **Verify images after they are created:** Enabled

The image is divided into multiple segments because a fragment size of **1500 MB** was selected.

<img width="542" height="467" alt="Screenshot 2026-08-30 122355" src="https://github.com/user-attachments/assets/316e29dc-f65b-498f-82a0-2e9a3702759c" />

---

## Step 8: Review and Start Disk Acquisition

Review the configured source drive, image format, destination folder, image filename, fragment size, and verification option.

After confirming the settings, click **Start** to begin the forensic image acquisition.

<img width="535" height="500" alt="Screenshot 2026-08-30 122456" src="https://github.com/user-attachments/assets/93539efe-2eb6-45a9-8d3f-bce1d28f0eea" />

---

## Step 9: Monitor Image Acquisition

FTK Imager creates the forensic image of the selected **D:\ logical drive** and displays the acquisition progress.

The acquisition is allowed to continue without interruption until the image creation process is completed successfully.

<img width="598" height="406" alt="Screenshot 2026-08-30 122538" src="https://github.com/user-attachments/assets/80b4b6ce-8075-4d9c-9984-a057f3e2ce22" />
<img width="521" height="396" alt="Screenshot 2026-08-30 123141" src="https://github.com/user-attachments/assets/93fedcb2-ef31-4b95-be62-97135de87d3e" />


---

## Step 10: Verify the Acquired Image and Hash Results

After the image acquisition is completed, FTK Imager verifies the acquired forensic image.

The following verification results were obtained:

- **MD5 Verify Result:** Match
- **SHA1 Verify Result:** Match
- **Bad Blocks:** No bad blocks found in image

The matching MD5 and SHA1 results confirm the integrity of the acquired forensic image.

<img width="605" height="518" alt="Screenshot 2026-08-30 123537" src="https://github.com/user-attachments/assets/a88b41b2-e5c6-487f-906c-49c9501fe513" />

---

## Step 11: View Image Summary and Generated Files

After successful acquisition and verification, the **Image Summary** displays information about the created forensic image.

The image was divided into multiple segments according to the configured fragment size. The generated image files include:

- `memdump_EX01.001`
- `memdump_EX01.002`
- `memdump_EX01.003`
- and subsequent image segments.

These image segments together represent the acquired forensic image.
<img width="455" height="538" alt="Screenshot 2026-08-30 123642" src="https://github.com/user-attachments/assets/591de631-bd39-4984-8a58-916024c2f5eb" />
<img width="470" height="540" alt="Screenshot 2026-08-30 123650" src="https://github.com/user-attachments/assets/2025b9eb-38c7-40b0-9001-728eaac9d6db" />
<img width="470" height="547" alt="Screenshot 2026-08-30 123657" src="https://github.com/user-attachments/assets/6dec8222-e1c6-49c6-b6f0-3ee59c16223e" />
<img width="482" height="377" alt="Screenshot 2026-08-30 123726" src="https://github.com/user-attachments/assets/02febf40-a023-4e84-b9f9-6be54c127148" />

<img width="1917" height="983" alt="Screenshot 2026-08-30 123959" src="https://github.com/user-attachments/assets/1edf983e-1a5f-441c-a519-80bdbc0fdf70" />


---

# Result

The volatile memory acquisition and logical-drive forensic imaging procedures were successfully performed using **AccessData FTK Imager**.
<img width="1917" height="983" alt="Screenshot 2026-08-30 123959" src="https://github.com/user-attachments/assets/1edf983e-1a5f-441c-a519-80bdbc0fdf70" />


The forensic image of the **D:\ logical drive** was successfully created and verified. The **MD5 and SHA1 hash verification results were Match**, and **no bad blocks were found in the image**, confirming the integrity of the acquired evidence.
