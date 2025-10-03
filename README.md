NAME:CHANDRU.P



REG NO:212223110007




# Metadata-Extraction-using-ExifTool-log2timeline-and-Hidden-Data-Search-using-Steganography-Tools
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
  exiftool image path
  exiftool png.jpeg
```
- **Embed data**
  ```
  steghide embed -cf (image path) -ef (text file path)
  steghide embed -cf /home/asinvardhini/Downloads/png.jpeg -ef /home/asinvardhini/Downloads/hidden.txt
  ```
- **Extract hidden data:**
  ```
  steghide extract -sf (imamge path)
  steghide extract -sf png.jpeg
  ```
- **Using binwalk – for file analysis**  
  ```bash
   binwalk png.jpeg
  ```
  
## OUTPUT:

### Extraction of Metadata using exiftool
<img width="400" alt="image" src="https://github.com/user-attachments/assets/e1e28e0a-e575-4021-b467-c6adb90c195e"/>


### Data Embedding in Image
<img width="400" alt="image" src="https://github.com/user-attachments/assets/3d1c5e74-ee2a-4c71-b340-584cdb3a777e"/>


### Extraction of hidden data
<img width="400" alt="image" src="https://github.com/user-attachments/assets/2aa71bb6-a239-435c-af34-5ad217673f1e"/>

### Using binwalk – for file analysis
<img width="400" alt="image" src="https://github.com/user-attachments/assets/eb0c5c2b-7aa6-4b0f-8e7d-9cd7bc01b52c"/>


## RESULT:
Metadata was successfully extracted, timeline analysis was completed, and hidden data was identified using steganography tools.

