# MP4 to PSP Video Converter (C++)

## Overview
This C++ program converts videos into a format compatible with the **PlayStation Portable (PSP)** using **FFmpeg**. The user selects a resolution, and the program ensures that only `.mp4` or `.avi` formats are used for the output file.

## Features
✅ **User Input Handling:** Asks for an input video and output filename.  
✅ **Format Restriction:** Only allows `.mp4` or `.avi` for output.  
✅ **Resolution Selection:** Provides three PSP-compatible resolutions:
   - **320x240 (Low Quality)**  
   - **480x272 (PSP Native Resolution)**  
   - **720x480 (Max Quality)**  
✅ **FFmpeg Integration:** Uses `system()` to execute an FFmpeg command.  
✅ **Metadata Removal:** Ensures no extra metadata is included in the output file.  

## How It Works
1. The user **enters the input video filename**.
2. The program asks for an **output filename**, ensuring it ends in `.mp4` or `.avi`.
3. A **menu appears for selecting resolution**.
4. The program constructs and **executes an FFmpeg command** to convert the video.
5. Once conversion is done, it **displays success or failure**.

## Requirements
- **FFmpeg** installed and added to `PATH`.
- **MinGW-w64** (if compiling on Windows).
- C++ compiler (`g++` recommended).

## Compilation & Usage
### **Compiling the Program**
```sh
g++ -o mp4-to-pspformat.exe main.cpp
```

### **Running the Program**
```sh
mp4-to-pspformat.exe
```
Then follow the on-screen prompts.

## Example Usage
```
Enter input video filename: myvideo.mp4
Enter output video filename (only .mp4 or .avi allowed): output.mp4
Select resolution:
1. 320x240 (Low)
2. 480x272 (PSP Native)
3. 720x480 (Max)
Enter choice (1-3): 2
Conversion complete: output.mp4
```

