# PrivacyBlur - Video Face Blurring

## Overview
SFCAM is a Python-based project that processes videos to detect and blur people's faces for privacy protection. The project uses OpenCV's Haar Cascade to identify faces in video frames and applies Gaussian blur to anonymize them.

## Project Structure
```
SFCAM/
├── input/               # Folder for input video files
│   └── videos.mp4       # Example input video file
├── output/              # Folder for output video files
│   └── (empty)          # Processed videos will be saved here
├── script.py            # Python script to process videos
├── requirements.txt     # List of dependencies for the script
└── README.md            # Documentation for the project
```

## Requirements
- Python 3.6+
- OpenCV library

## Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/aloautiq/PrivacyBlur.git
   cd PrivacyBlur
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
1. Place your input videos in the `input/` folder.
2. Run the script:
   ```bash
   python script.py
   ```
3. Processed videos will be saved in the `output/` folder with filenames prefixed by `blurred_`.

## How It Works
1. The script reads video files from the `input/` directory.
2. It uses OpenCV's Haar Cascade to detect faces in each frame.
3. Detected faces are blurred using Gaussian blur.
4. The processed frames are saved to a new video file in the `output/` directory.

## Notes
- This script uses OpenCV's Haar Cascade for face detection, which works best with clear and well-lit videos.
- Ensure the input video file is in `.mp4` format for compatibility.
- Adjust the Gaussian blur intensity in the script if needed by modifying the `cv2.GaussianBlur` parameters.

## Limitations
- Haar Cascade may not detect faces in poor lighting or extreme angles.
- Processing time depends on video resolution and length.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Contribution
Contributions are welcome! Please fork the repository, make changes, and submit a pull request.

---
Developed with ❤️ using Python and OpenCV.
