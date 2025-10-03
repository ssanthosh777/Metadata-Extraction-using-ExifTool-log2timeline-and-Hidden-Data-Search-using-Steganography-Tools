# Metadata-Extraction-using-ExifTool-log2timeline-and-Hidden-Data-Search-using-Steganography-Tools
## NAME: SANTHOSH S
## REG.NO: 212224100052
## AIM:
To extract metadata, perform timeline analysis, and search for hidden data using forensic tools like ExifTool, log2timeline, and steganography detection tools.

## DESIGN STEPS:
### Step 1:
Use exiftool to extract metadata from files such as images, documents, and videos.

### Step 2:
Use log2timeline and plaso to create and analyze event timelines from system logs and file metadata.

### Step 3:
Apply steganography detection tools like steghide, zsteg, or binwalk to uncover hidden data in media files.

## PROGRAM:
Metadata and Timeline Forensics, Steganography Analysis Steps
- **Installation :**
```bash
   sudo apt update
   sudo apt install exiftool -y
   sudo apt install plaso -y
   sudo apt install steghide -y
   sudo apt install binwalk -y
 ```
- **Extract metadata from a file:**
```bash
  exiftool /<image path>/image1.jpeg
```
- **Embed data**
  ```
  steghide embed -cf /<image path>/image.jpeg -ef /<text file path>/hidden.txt
  ```
- **Extract hidden data:**
  ```
  steghide extract -sf /<image path>/image1.jpeg
  ```
- **Using binwalk – for file analysis**  
  ```bash
   binwalk /<image path>/image1.jpeg
  ```
  
## OUTPUT:

### Extraction of Metadata using exiftool
<img width="647" height="457" alt="1" src="https://github.com/user-attachments/assets/129ee2bd-9e5e-48f9-8e26-327f3bac9029" />



### Data Embedding in Image
<img width="641" height="148" alt="2" src="https://github.com/user-attachments/assets/246190fa-9c40-4759-a04c-1dbf0b97e08b" />



### Extraction of hidden data
<img width="624" height="91" alt="3" src="https://github.com/user-attachments/assets/e9ab1935-291d-447e-9df8-fc1f66f15305" />


### Using binwalk – for file analysis
<img width="627" height="146" alt="4" src="https://github.com/user-attachments/assets/dc1c0c1a-cf12-4638-94f3-11e3b300a799" />



## RESULT:
Metadata was successfully extracted, timeline analysis was completed, and hidden data was identified using steganography tools.

