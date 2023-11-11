# HW3_MotionEstimationAndCompensation

**NYCU Video Compression HW3**

- Motion estimation (ME)
  - Block size: 8x8
  - Search range: [+-8]
  - Full search block matching algorithm
  - Integer precision
- Motion compensation (MC)
  - Save the reconstructed frame (after MC) and the residual
- Search range:
  - Compare the results (in PSNR and runtime) with different search ranges ([+-8], [+-16], [+-32]).
- Three-step search
  - Compare the results (in PSNR and runtime) with the Full search algorithm.

## Introduction
- This repository contains Python code for motion estimation and compensation in video processing. 
- The implemented algorithms include the Three-Step Search and Full Search methods. 
- The goal is to estimate motion vectors between consecutive frames and compensate for motion to reconstruct frames.


## Project Structure
The project includes the following files:

```main.py``` - This is the main script that loads two grayscale images, performs motion estimation and compensation for various search ranges and methods, calculates PSNR, and saves the reconstructed frames and residuals.

```one_gray.png``` and ```two_gray.png```: - Sample grayscale images used for motion estimation and compensation.

## Dependencies
To run this project, you need to have the following libraries installed:

- Python
- NumPy
- OpenCV

## Usage
### Clone Repository
```
git clone https://github.com/ting0602/HW3_MotionEstimationAndCompensation.git
```

### Run the Code
```
python main.py
```

### Results
- The output includes:
  - reconstructed frames (reconstructed_{method}_{search_range}.png)
  - residuals (residual_{method}_{search_range}.png)
  - PSNR values and execution times


