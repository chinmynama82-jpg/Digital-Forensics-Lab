# Ex.No.05 – Use Autopsy to Create a Case and Import Evidence

## Experiment Name

**Use Autopsy to Create a Case and Import Evidence**

## Aim

To use Autopsy to create a forensic case and import digital evidence for analysis.

## Tool Used

- Autopsy

## Evidence Used

- `4Dell Latitude CPi.E01`
- `4Dell Latitude CPi.E02`

## Procedure

### 1. Installation

Install and open Autopsy on the system.
<img width="1052" height="722" alt="Screenshot 2026-08-26 214628" src="https://github.com/user-attachments/assets/28ae2555-3837-4dbe-8862-4b63bc8f9622" />

### 2. Starting a New Case

1. Open Autopsy.
2. Click **New Case**.
3. Enter the case name and case location.
4. Enter the case number and examiner details.
5. Click **Next**.
<img width="698" height="388" alt="image" src="https://github.com/user-attachments/assets/4fa66bd0-53dc-4933-95c4-69df8d5d08a6" />

### 3. Adding a Data Source

1. Select **Disk Image or VM File**.
2. Browse and select the forensic image.
3. Import `4Dell Latitude CPi.E01`.
4. Keep the related `4Dell Latitude CPi.E02` file with the evidence set.
5. Configure the required ingest modules.
6. Start the analysis.
<img width="1197" height="747" alt="Screenshot 2026-08-26 215124" src="https://github.com/user-attachments/assets/69ed3167-a655-4c54-b7ba-b030d51d621a" />

### 4. Initial Analysis and Overview

After ingest processing, examine the artifacts available in Autopsy.

The following areas can be explored:

- File System
- Web History
- Email
- Other forensic artifacts
<img width="1753" height="946" alt="Screenshot 2026-08-26 230454" src="https://github.com/user-attachments/assets/b7a86a76-5862-426c-b042-6a7cd6222317" />


### 5. Detailed Analysis

#### Keyword Search

Use Keyword Search to search for specific keywords in the evidence.

#### File Analysis

Navigate through files and folders under File System or File Types and examine the available files.

#### Timeline Analysis

Use the Timeline module to visualize forensic events based on timestamps.

#### Hash Analysis

Use Hash Lookup/Hash Analysis to compare file hashes with known databases.

<img width="1112" height="705" alt="Screenshot 2026-08-26 230552" src="https://github.com/user-attachments/assets/58356118-b3e3-40b2-83f7-45f63d6b9577" />
<img width="1307" height="780" alt="Screenshot 2026-08-26 230635" src="https://github.com/user-attachments/assets/603db688-ee71-441f-b450-fe42e2d77e3b" />
<img width="1281" height="852" alt="Screenshot 2026-08-26 232349" src="https://github.com/user-attachments/assets/31342845-b683-4af1-8c25-1276c48941e9" />

### 6. Reporting

1. Click **Generate Report**.
2. Select **HTML Report**.
3. Select the data source and required results.
4. Generate the report.
5. Review and save the generated report.
<img width="1085" height="676" alt="Screenshot 2026-08-26 232526" src="https://github.com/user-attachments/assets/2f85f417-c8c2-4246-8919-86c92242654e" />
<img width="1067" height="662" alt="Screenshot 2026-08-26 232600" src="https://github.com/user-attachments/assets/22a8bd77-7323-4bec-bb50-5d9be85aedd7" />
<img width="878" height="546" alt="Screenshot 2026-08-26 232657" src="https://github.com/user-attachments/assets/5ed73979-0dfb-4c8d-af1c-4711ad0f4454" />
<img width="1911" height="1006" alt="Screenshot 2026-08-27 000308" src="https://github.com/user-attachments/assets/21d4e103-023c-4fbd-a02f-839605f21380" />
<img width="1891" height="1013" alt="Screenshot 2026-08-27 000333" src="https://github.com/user-attachments/assets/023065f7-662c-4926-90b3-205a981bd67b" />

## Observations

### Web History

The imported forensic image contained:

**887 Web History records**

### Analysis Results

The analysis results included:

- Encryption Suspected
- Extension Mismatch Detected
- Interesting Items
- Web Categories

### Timeline Analysis

Timeline Analysis was performed to visualize forensic events according to their timestamps.

### Report

An **HTML forensic report** was successfully generated.


## Result

The forensic image was successfully imported into Autopsy and analyzed. Web History and other forensic artifacts were examined, Timeline Analysis was performed, and an HTML forensic report was successfully generated.

## Conclusion

Autopsy was successfully used to create a forensic case, import digital evidence, analyze forensic artifacts, perform timeline analysis, and generate a forensic report.
