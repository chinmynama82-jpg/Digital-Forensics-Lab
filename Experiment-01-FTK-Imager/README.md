# FTK Imager – Digital Evidence Acquisition

## 🔍 Overview

A hands-on digital forensics practical focused on the acquisition and preservation of digital evidence using **AccessData FTK Imager**.

This experiment explores how forensic investigators collect volatile and non-volatile data and validate the integrity of the acquired evidence.

## 🎯 Focus Areas

* RAM acquisition
* Disk imaging
* Forensic image formats
* Evidence documentation
* Hash-based integrity verification

## 🛠️ Tool Used

**AccessData FTK Imager**

## 🔬 Practical Work

### Memory Acquisition

Captured volatile memory from a live Windows system using the memory acquisition functionality of FTK Imager.

The resulting memory dump can be preserved for further forensic examination.

### Disk Acquisition

Created a forensic image from the selected storage source using FTK Imager's disk imaging functionality.

The acquisition process was configured with appropriate case information, destination details, and image format.

### Integrity Validation

Enabled post-acquisition verification and examined the generated hash values to validate the integrity of the acquired evidence.

## 📦 Image Formats

The practical explored commonly used forensic image formats:

* RAW / DD
* E01
* SMART
* AFF

## 🔐 Evidence Integrity

Hash verification was used as an integrity check between the source evidence and the acquired forensic image.

```text
Evidence Source
      ↓
Acquisition
      ↓
Forensic Image
      ↓
Hash Calculation
      ↓
Hash Comparison
      ↓
Integrity Validation
```

## 📸 Practical Evidence

Screenshots documenting the major stages of the practical are stored in the `screenshots` directory.

## 🧠 Skills Demonstrated

`Digital Forensics` · `FTK Imager` · `Memory Acquisition` · `Disk Imaging` · `Hash Verification` · `Evidence Preservation`

## ⚠️ Note

This repository is intended for educational purposes. No confidential or personally identifiable forensic evidence is included.
