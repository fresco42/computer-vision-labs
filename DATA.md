# Data

Datasets and test images are **not** tracked in this repository (size and licensing).
The notebooks expect the following layout relative to the repository root:

```
data/
├── test_images/               # labs 03–08
│   ├── einstein.jpg, catDog.jpg, SaltAndPepper.gif, tiger.bmp, ...
│   ├── fruits/{train,test}/   # lab 04
│   └── sequence/Bootstrap/    # lab 03
└── car_classification/        # lab 09
    ├── TrainImages/           # pos-*.pgm / neg-*.pgm
    └── TestImages/
```

| Folder | Used in | Source |
|--------|---------|--------|
| `test_images/` | Labs 03–08 | Test image collection provided with the course |
| `test_images/fruits/` | Lab 04 | Fruit image set provided with the course |
| `car_classification/` | Lab 09 | Based on the [UIUC Image Database for Car Detection](https://cogcomp.seas.upenn.edu/Data/Car/) (Agarwal & Roth), restructured for the course |

Notebooks reference images via relative paths such as `../../data/test_images/einstein.jpg`, so run them from their own lab folder (default in Jupyter).
