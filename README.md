
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

# Installation :
```
   sudo apt update
   sudo apt install exiftool -y
   sudo apt install plaso -y
   sudo apt install steghide -y
   sudo apt install binwalk -y
```
# Extract metadata from a file:
```
  exiftool image path
  exiftool png.jpeg
```
# Embed data
```
steghide embed -cf (image path) -ef (text file path)
steghide embed -cf /home/bharathi/Downloads/png.jpeg -ef /home/bharathi/Downloads/hidden.txt
```
# Extract hidden data:
```
steghide extract -sf (imamge path)
steghide extract -sf png.jpeg
```
Using binwalk – for file analysis
```
 binwalk png.jpeg
```
## OUTPUT:
Extracted Metadata, Timeline Events, and Hidden Data Detection Results
# Extracted Metadata
![copy 1](https://github.com/user-attachments/assets/e53ea3dc-f02f-4076-8793-d7b7c6a915c3)

# Embed data and extraction of hidden data:
![image](https://github.com/user-attachments/assets/f19651ab-4e2d-4bae-83b8-0713b55aa88e)

# using binwalk for analysis:
![image](https://github.com/user-attachments/assets/8c3eea51-5070-4f40-85fd-c9d9488500cc)



## RESULT:
Metadata was successfully extracted, timeline analysis was completed, and hidden data was identified using steganography tools.

