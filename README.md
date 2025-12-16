# Photo Adapter for Google Colab

This Colab notebook allows you to adapt any uploaded photo to meet standard requirements for IDs, profiles, or other applications.

## Features

- Supports JPG, JPEG, PNG input files.
- Ensures minimum resolution of 295x413 pixels.
- Compresses file to ~100–200 KB.
- Saves as JPEG (with option to modify code for PNG if needed).
- Automatic resizing if the photo is smaller than required.
- Download the adapted photo directly from Colab.

## How to Use

1. Open the notebook in Google Colab.
2. Run the first cell to install required libraries.
3. Run the second cell to upload your photo.
4. The notebook will automatically:
    - Resize the image if smaller than 295x413 pixels.
    - Compress it to ~150 KB.
    - Save it as `adapted_photo.jpg`.
5. Download your adapted photo when prompted.

## Requirements

- Python 3.x
- Google Colab
- Pillow library (`pip install pillow`)

## Notes

- The code currently converts all images to JPEG. You can modify the format in the code to preserve PNG if needed.
- You can adjust `target_size_kb` for different file size limits.
- Minimum width and height can be changed in the function parameters.
