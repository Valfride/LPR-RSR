# Dataset description

The proposed dataset was designed on Low Resolution (LR) License Plate (LP) images extracted from RodosSol-ALPR described in  and . This dataset comprises 20.000 images taken by static cameras at a pay rolls located in Brazil state of Espírito Santo. Among the 20.000 images, there are 5.000 images of each of the following combination of type and layout:

* Cars with brazilian LPs
* Cars with Mercosur LPs
* Motorcycles with brazilian LPs
* Motorcycles with Mercosur LPs

The brazilian layout consists of of three letters followed by four digits, while the initial pattern adopted in Brazil for Mercosur LPs consists of three letters, one digit, one letter and two digits. To the best of our knowledge,  RodoSol-ALPR is the largest public dataset in terms of both Brazilian and Mercosur LPs. Also, this dataset has great diversity egarding several factors such as of LP colors, lighting conditions, and character fonts.

For each image from the RodoSol-ALPR dataset, we first cropped the LP region using the annotations provided by the authors. Afterward, we used the same annotations to rectify each LP image so that it becomes more horizontal, tightly bounded, and easier to recognize. The rectified image is the HR image.

Then, multiple LR LP images generated  by applying intense Gaussian noise to each HR image. This process is repeated until the desired degradation for a given LR image is reached. The degradation level was measured by considering the SSIM score between the HR and LR images. 

Here are some Representative examples of the generated dataset:


# How to obtain the dataset


# Citation


