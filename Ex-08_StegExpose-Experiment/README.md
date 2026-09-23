# Ex.No. 8 — Use StegExpose to Detect Hidden Data in Images

## Aim

To use **StegExpose** to analyze digital images and detect possible hidden data using statistical steganalysis techniques.

## Objective

The objective of this experiment is to examine images for possible steganographic content using StegExpose. The tool analyzes the statistical properties of images and generates a **Fusion score** to determine whether an image is above the steganography detection threshold.

## Software and Tools Required

- Java Runtime Environment (JRE)
- StegExpose
- Windows Command Prompt
- Test Images
  
## Procedure

### Step 1: Verify Java Installation

Java was verified using the following command:

```cmd
java -version
```

The installed Java version was successfully displayed in Command Prompt.

<img width="1412" height="222" alt="image" src="https://github.com/user-attachments/assets/1bd3b663-6f3c-436a-acce-5c06269ae191" />


## Step 2: Download and Set Up StegExpose

The StegExpose tool was downloaded and the `StegExpose.jar` file was placed in the experiment directory:

```text
C:\DF_Experiment_8
```
<img width="1917" height="680" alt="image" src="https://github.com/user-attachments/assets/cc7dc15a-e5fc-42bc-841b-e72c9e532325" />

## Step 3: Select Images for Analysis

A folder named `testFolder` was created inside the experiment directory:

```text
C:\DF_Experiment_8\testFolder
```

The following images were placed inside the folder for analysis:

- `clean_image.png`
- `image 2.png`
- `images 3.png`

These images were selected as test samples for StegExpose analysis.

<img width="1165" height="600" alt="image" src="https://github.com/user-attachments/assets/082b5ef0-d34d-4964-ac37-3daed9b212c1" />

## Step 4: Open Command Prompt

Command Prompt was opened to execute StegExpose.

The working directory was changed to the experiment folder using:

```cmd
cd C:\DF_Experiment_8
```

The Command Prompt was then ready to execute the StegExpose analysis command.
<img width="1108" height="332" alt="image" src="https://github.com/user-attachments/assets/db180b31-c581-4e63-964d-bdc38dd680c4" />

## Step 5: Run StegExpose

StegExpose was executed on the folder containing the test images using the following command:

```cmd
java -jar StegExpose.jar testFolder
```

The command analyzes the images stored in the `testFolder` directory.

<img width="923" height="167" alt="Screenshot 2026-09-23 181624" src="https://github.com/user-attachments/assets/0dac2adc-7bec-4c00-9287-bb52b1e3d1bc" />

## Step 6: Generate and View the Analysis Report

A CSV report was generated using the following command:

```cmd
java -jar StegExpose.jar testFolder default default results.csv
```

The generated report was displayed using:

```cmd
type results.csv
```

The report contains the statistical analysis results produced by StegExpose.


<img width="931" height="291" alt="image" src="https://github.com/user-attachments/assets/dc27550c-093f-45d7-a8ec-2e1e782db44a" />


## Step 7: Analyze the Output

The generated `results.csv` file was examined to identify the statistical analysis results produced by StegExpose.

The following parameters were obtained:


### Observation

Both processed images were reported as:

```text
Above stego threshold? = FALSE
```

The Fusion (mean) scores obtained were:

- `image 2.png` → **0.066712**
- `images 3.png` → **0.018933**

The `clean_image.png` file does not appear in the generated CSV report. Therefore, no result is reported for that image.


<img width="1256" height="492" alt="image" src="https://github.com/user-attachments/assets/52292395-df5a-4332-a95a-8a6fd723b752" />

## Result

StegExpose was successfully used to analyze the test images for possible steganographic content.

The default StegExpose detection threshold of **0.2** was used for the analysis. The obtained results are:

| Image | Fusion Score | Threshold | Interpretation | Above Stego Threshold? |
|---|---:|---:|---|---|
| `clean_image.png` | Not generated | 0.2 | Clean test image | — |
| `image 2.png` | **0.066712** | 0.2 | Clean — below 0.2 | **FALSE** |
| `images 3.png` | **0.018933** | 0.2 | Clean — below 0.2 | **FALSE** |

The Fusion scores for `image 2.png` and `images 3.png` are below the default threshold of **0.2**. According to the threshold interpretation used in this experiment, scores below 0.2 fall within the **clean image** range.

The StegExpose report therefore shows:

```text
Above stego threshold? = FALSE












