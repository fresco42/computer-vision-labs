# Computer Vision Labs

Hands-on lab work from the **AI & Computer Vision** course (Media Technology B.Sc., [USTP](https://www.ustp.at), summer term 2026).
Nine Jupyter notebooks progressing from NumPy fundamentals to classical image processing, feature detection and deep learning–based image classification. All notebooks are committed **with outputs**, so results render directly on GitHub.

## Labs

| # | Lab | Topics | Key tools |
|---|-----|--------|-----------|
| 01 | [Python Basics](labs/01-python-basics/python_basics.ipynb) | Python syntax, data types, functions | Python |
| 02 | [NumPy Basics](labs/02-numpy-basics/numpy_basics.ipynb) | Arrays, indexing, slicing, reshaping, vectorized ops | NumPy |
| 03 | [Basic Image Processing](labs/03-basic-image-processing/basic_image_processing.ipynb) | Pixel manipulation, geometric transforms, pixel-wise arithmetic, thresholding, background extraction from image sequences | NumPy, scikit-image, imageio |
| 04 | [Histogram-based Image Retrieval](labs/04-histogram-image-retrieval/histogram_retrieval.ipynb) | RGB colour histograms as feature vectors, similarity search, top-k retrieval | NumPy, Matplotlib |
| 05 | [Convolution & Denoising](labs/05-convolution-denoising/convolution_denoising.ipynb) | 2D convolution, boundary modes, Gaussian/box smoothing, median filter for salt-and-pepper noise | SciPy |
| 06 | [Edge Detection](labs/06-edge-detection/edge_detection.ipynb) | Gradient filters, oriented edges, sharpening, Canny edge detector, custom effect filter | SciPy, scikit-image |
| 07 | [Harris Corner Detection](labs/07-harris-corner-detection/corner_detection.ipynb) | Sobel operator, Harris corner detector implemented from scratch, comparison with library implementation | NumPy, SciPy, scikit-image |
| 08 | [ORB Feature Matching](labs/08-orb-feature-matching/feature_matching.ipynb) | ORB keypoints & descriptors, brute-force matching, match visualisation | OpenCV |
| 09 | [Deep Learning Image Classification](labs/09-deep-learning-classification/image_classification.ipynb) 🚧 | MLP vs. CNN for car detection, preprocessing & standardisation, overfitting, evaluation | TensorFlow / Keras, scikit-learn |

🚧 **Lab 09 is work in progress:** the MLP part is complete; the CNN training-history plot and the data-augmentation exercise are still pending.

## Repository structure

```
computer-vision-labs/
├── labs/            # one folder per lab, each with a single notebook
├── data/            # datasets (not tracked, see DATA.md)
├── DATA.md          # where to get the data and how to place it
└── requirements.txt
```

## Setup

Requires **Python 3.10–3.13** (TensorFlow does not support newer Python versions yet).

```bash
python -m venv .venv
source .venv/bin/activate        # Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter lab
```

Images and datasets are not part of this repository. See [DATA.md](DATA.md) for the expected layout under `data/`.

## Notes

Exercise descriptions and starter code were provided by the course instructors; the solutions are my own work.

**Author:** Daniel Przala
