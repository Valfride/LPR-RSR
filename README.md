# Dataset description

The proposed dataset was designed on Low Resolution (LR) License Plate (LP) images extracted from RodosSol-ALPR described in [GitHub](https://github.com/raysonlaroca/rodosol-alpr-dataset). This dataset comprises 20.000 images taken by static cameras at a pay rolls located in Brazil state of Espírito Santo. Among the 20.000 images, there are 5.000 images of each of the following combination of type and layout:

* Cars with brazilian LPs
* Cars with Mercosur LPs
* Motorcycles with brazilian LPs
* Motorcycles with Mercosur LPs

The brazilian layout consists of of three letters followed by four digits, while the initial pattern adopted in Brazil for Mercosur LPs consists of three letters, one digit, one letter and two digits. To the best of our knowledge,  RodoSol-ALPR is the largest public dataset in terms of both Brazilian and Mercosur LPs. Also, this dataset has great diversity egarding several factors such as of LP colors, lighting conditions, and character fonts.

For each image from the RodoSol-ALPR dataset, we first cropped the LP region using the annotations provided by the authors. Afterward, we used the same annotations to rectify each LP image so that it becomes more horizontal, tightly bounded, and easier to recognize. The rectified image is the HR image.

Then, multiple LR LP images generated  by applying intense Gaussian noise to each HR image. This process is repeated until the desired degradation for a given LR image is reached. The degradation level was measured by considering the Structural Similarity Index measure (SSIM) score between the HR and LR images. 

Here are some Representative examples of the generated dataset:
<img src="./media/image.png"/>
Note: In the image from left to right: 1 (original image), 0.75, 0.5, 0.25 and 0.1 SSIM scores.
<br>


# How to obtain the dataset


# Citation

If you use our dataset or the RodoSol-ALPR dataset in your research, please cite:

* R. Laroca, E. V. Cardoso, D. R. Lucio, V. Estevam, and D. Menotti, “On the Cross-dataset Generalization in License Plate Recognition” in International Conference on Computer Vision Theory and Applications (VISAPP), Feb 2022, pp. 166-178. [[arXiv]](https://arxiv.org/abs/2201.00267) [[SciTePress]](https://doi.org/10.5220/0010846800003124)

```
This work citation
```

and

```
@inproceedings{laroca2022cross,
  title = {On the Cross-dataset Generalization in License Plate Recognition},
  author = {R. {Laroca} and E. V. {Cardoso} and D. R. {Lucio} and V. {Estevam} and D. {Menotti}},
  year = {2022},
  month = {Feb},
  booktitle = {International Conference on Computer Vision Theory and Applications (VISAPP)},
  volume = {},
  number = {},
  pages = {166-178},
  doi = {10.5220/0010846800003124},
  isbn = {978-989-758-555-5},
  issn = {2184-4321}
}
```




Additionally, consider showing your support by starring (:star:) this and [RodoSol-ALPR](https://github.com/raysonlaroca/rodosol-alpr-dataset) repositories.

