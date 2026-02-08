# Image Denoising and Hybrid Images (Week 1)

Small Python scripts for a computer vision lab on filtering, denoising, and hybrid images.

## Files
- `image_denoising.py` - Noise generation and denoising with Gaussian, median, and bilateral filters.
- `hybrid_images.py` - Create a hybrid image using low-pass and high-pass filtering plus Fourier visualization.
- `utils.py` - Utility functions (noise, Gaussian kernel, affine fit, bilateral filter).

## Requirements
- Python 3.8+
- numpy
- scipy
- matplotlib
- scikit-image

Install (example):
```
pip install numpy scipy matplotlib scikit-image
```

## Input Images
Place these image files in the same folder before running:
- `einsteinpic.jpg`
- `man.jpg`
- `wolf.jpg`

## Run
```
python image_denoising.py
python hybrid_images.py
```

## Output (example)
Running `image_denoising.py` displays a 2x4 figure titled "Filtering results":
- Row 1 (salt & pepper noise): noisy input, Gaussian filter, median filter, bilateral filter.
- Row 2 (Gaussian noise): noisy input, Gaussian filter, median filter, bilateral filter.

![Filtering results](denoised%20image.png)

## Notes
- `hybrid_images.py` uses hard-coded feature points for alignment. Adjust those points if you change the input images.
- Try different `sigmaA` and `sigmaB` values to explore hybrid image behavior.
