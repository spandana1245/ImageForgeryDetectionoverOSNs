Overview

This project implements a deep learning-based image forgery detection system using a ResNet-34 encoder-decoder architecture. The system is designed to detect and localize manipulated regions in digital images, making it suitable for real-world applications like online social networks, content moderation, and digital forensics.

Key Features

Model Architecture: ResNet-34 as encoder, with a lightweight decoder for segmentation.

Datasets Used:

NIST

Columbia

CASIA v2.0

DSO (GAN-based forgeries)

Performance Highlights:

NIST: 96.38% accuracy, 0.9591 AUC

Columbia: F1-score > 0.82, IoU = 0.7883

CASIA v2.0: High generalizability

DSO: Handles GAN manipulations with moderate success

Dataset Download

You can download the complete dataset used for training and evaluation from the following link:
https://drive.google.com/file/d/1uMNZdhX3bYAZNcVGlkCvrnj5lSLW1ld5/view

After downloading, extract and place the dataset into the data folder

Installation

Clone the repository

cd image-forgery-detection

Install the required dependencies

Usage

Launch the notebook:

jupyter notebook

Open imageforgerydetection.ipynb and run all cells.

Make sure to place datasets in the correct directory structure as expected by the notebook.

Model Architecture

The system uses a ResNet-34-based encoder-decoder framework for forgery segmentation. 

License

This project is licensed under the MIT License. See the LICENSE file for details.

Citation

If you use this code/dataset for your research, please consider citing the references of the original dataset:

@article{DSO,
  title={Exposing digital image forgeries by illumination color classification},
  author={T. Carvalho and C. Riess and E. Angelopoulou and H. Pedrini and A. Rezende Rocha},
  journal={IEEE Trans. Inf. Forensics and Security},
  volume={8},
  number={7},
  pages={1182--1194},
  year={2013},
  publisher={IEEE}
}

@inproceedings{Columbia,
  title={Detecting image splicing using geometry invariants and camera characteristics consistency},
  author={Y. Hsu and S. Chang},
  booktitle={IEEE Inter. Conf. Multim. Expo},
  pages={549--552},
  year={2006},
  organization={IEEE}
}

@misc{NIST,
  title = {Nist nimble 2016 datasets},
  howpublished = {\url{https://www.nist.gov/itl/iad/mig/nimble-challenge-2017-evaluation/}},
}

@inproceedings{CASIA,
  title={Casia image tampering detection evaluation database},
  author={J. Dong and W. Wang and T. Tan},
  booktitle={IEEE China Summit Inter. Conf. Signal Info. Proc.},
  pages={422--426},
  year={2013},
  organization={IEEE}
}

Acknowledgments

NIST Media Forensics Challenge

CASIA and Columbia research groups

OpenCV, PyTorch, and Scikit-learn developers
