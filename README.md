# GenericConv: A generic model for image scene classification using few-shot learning

### Datasets

**MiniSun** 

The MiniSun dataset contains 100 classes randomly chosen from sun397 with 100 images of size 84×84 pixels per class. It is split into 64 base classes, 16 validation classes and 20 novel classes.

**MiniPlaces**

The MiniPlaces dataset contains 100 classes randomly chosen from Places with 600 images of size 84×84 pixels per class. It is split into 64 base classes, 16 validation classes and 20 novel classes.

**MIT-Indoor 67 dataset**

The MIT-Indoor 67 dataset contains 67 indoor categories and a total of 15620 images. The number of images varies across categories, but there are at least 100 images per category. All images are in jpg format. The images provided here are for research purposes only.

### Pipeline 

![](https://raw.githubusercontent.com/MohmedSoudy/A-generic-approach-for-image-scene-classification-using-few-shot-learning/main/Figure%203.jpeg)

### Proposed model 

![](https://raw.githubusercontent.com/MohmedSoudy/A-generic-approach-for-image-scene-classification-using-few-shot-learning/main/Figure%204.jpeg)

### Results 

|                  | MiniSun          |                  |          
|------------------|------------------|------------------|
| **k-way**        | **5**            |**5**             |
| **n-shot**       | **5**            |**1**             |
| MobileNetV2      | 20.16 ± 0.011    |                  |
| Conv4            | 39.14 ± 0.015    | 26.03  ± 0.013   |
| Conv6            | 33.42 ± 0.015    | 24.58  ± 0.012   |
| Conv8            | 29.32 ± 0.012    | 21.48  ± 0.011   |
| MobileBlock1     | 40.12 ± 0.015    | 30.86 ± 0.01     |
| MobileConv       | 47.5 ± 0.0158    | 30.72  ± 0.013   |
| Generic-Conv     |**52.16 ± 0.015** |**32.72 ± 0.014** |


|                  | MiniPlaces       |                  |          
|------------------|------------------|------------------|
| **k-way**        | **5**            |**5**             |
| **n-shot**       | **5**            |**1**             |
| Conv4            | 27.9   ± 0.014   | 29.62 ± 0.013    |
| Conv6            | 19.84  ± 0.007   | 21.42 ± 0.009    |
| Conv8            | 25.2   ± 0.011   | 21.14 ± 0.004    |
| MobileBlock1     | 20.1 ± 0.001     | --------------   |
| MobileConv       | 34.64 ± 0.014    | 26.36 ± 0.013    |
| Generic-Conv     |**35.86 ± 0.014** | 23.80 ± 0.012    |

|                  | MIT-Indoor       |                  |          
|------------------|------------------|------------------|
| **k-way**        | **5**            |**5**             |
| **n-shot**       | **5**            |**1**             |
| Conv4            | 28.7 ± 0.013     | 22.0 ± 0.012     |
| Conv6            | 20.16 ± 0.003    | 20.0 ± 0.0014    |
| Conv8            | 22.18 ± 0.005    | 20.10 ± 0.003    |
| MobileBlock1     | 34.1 ± 0.014     | 24.6 ± 0.012     |
| MobileConv       | 33.18  ± 0.014   | 23.82  ± 0.012   |
| Generic-Conv     |**37.26 ± 0.014** |**24.82 ± 0.013** |
