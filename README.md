<a id="readme-top"></a>


[![LinkedIn][linkedin-shield]][linkedin-url]

<h3 align="center">U-Net for Image Reconstruction with Knowledge Distillation</h3>

  <p align="center">
    A PyTorch implementation of U-Net for simultaneous image reconstruction and segmentation using knowledge distillation and composite loss functions.
    <br />
    <br />
    <br />
  </p>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    <li><a href="#installation">Installation</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>

## About The Project
This project implements a sophisticated U-Net architecture that simultaneously performs image reconstruction and segmentation using a novel composite loss function. The model leverages knowledge distillation by incorporating features from a pre-trained VGG11 teacher network to guide the learning process. A key innovation is the multi-component loss function that combines reconstruction error (MSE), feature distillation loss, and fuzzy normalized cut loss for segmentation regularization. Trained on CIFAR-10, the system demonstrates strong performance with a PSNR of 23.23 dB and SSIM of 0.859, showcasing effective dual-task learning where a single model learns to both reconstruct input images and produce segmentation masks through an end-to-end differentiable pipeline.


### Features

- **Dual-task U-Net**: Performs both segmentation and reconstruction
- **Knowledge Distillation**: Uses pre-trained VGG11 as teacher model
- **Composite Loss**: Combines reconstruction, distillation, and fuzzy normalized cut losses
- **Multi-modal Output**: Generates both segmentation masks and reconstructed images

### Results
(After 10 epochs)
**Test Metrics:**
- PSNR: 23.23 dB
- SSIM: 0.859
- MSE: 0.0048

<p align="right">(<a href="#readme-top">back to top</a>)</p>


## Built With
* Python
   + Numpy
   + Pandas
   + Scikit-Learn
   + Matplotlib
   + Pytorch

<p align="right">(<a href="#readme-top">back to top</a>)</p>



## Installation
1. First intall jupyter notebook from the link below if you haven't already.
   + https://jupyter.org/install
2. Make sure you have all the libraries mentioned in Built With section installed; If not first run your environment then use the following commands:
+ ```console
  pip install torch torchvision torchmetrics
  ```

3. Run the notebook.
<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTACT -->
## Contact
Mohammad Mofidi
* Email: mohammad.mofidi.k@gmail.com
* Linkedin: https://www.linkedin.com/in/mohammad-mofidi-khajeh-2715832b8/
* Instagram: https://www.instagram.com/_mohammadmofidi/


<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->

[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/mohammad-mofidi-khajeh-2715832b8/












  
