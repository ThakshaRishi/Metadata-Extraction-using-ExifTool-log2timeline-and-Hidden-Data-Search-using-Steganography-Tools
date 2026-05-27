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
  steghide embed -cf /home/bharathi/Downloads/png.jpeg -ef /home/bharathi/Downloads/hidden.txt
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

<img width="1182" height="871" alt="image" src="https://github.com/user-attachments/assets/14c5f49b-5765-4ddf-bf92-0791521d1822" />

### Data Embedding in Image

<img width="1422" height="249" alt="image" src="https://github.com/user-attachments/assets/1533ee9c-9f43-4c01-9127-e91483c6925f" />

### Extraction of hidden data

<img width="1323" height="203" alt="image" src="https://github.com/user-attachments/assets/35bcd0e4-bb15-4795-8d15-1a354f5bbd1d" />

### Using binwalk – for file analysis

<img width="939" height="198" alt="image" src="https://github.com/user-attachments/assets/4423c1be-6636-4f01-90f9-bd2f8ca67d6b" />


## RESULT:
Metadata was successfully extracted, timeline analysis was completed, and hidden data was identified using steganography tools.

