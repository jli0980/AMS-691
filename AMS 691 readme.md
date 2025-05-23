README: How to Run the Code

This project simulates synthetic brain tumors in multi-modal MRI data using a 2D cellular automata model based on the Pixel2Cancer framework.

Requirements:
Python 3.8+
numpy
h5py
opencv-python
tqdm

Install dependencies with:
pip install numpy h5py opencv-python tqdm

Dataset:
Download the BraTS 2020 dataset from Kaggle (https://www.kaggle.com/datasets/awsaf49/brats2020-training-data?resource=download) and extract the HDF5 .h5 files to a local folder.

Running the Code:
Open the ipynb file in vs code or colab.
Set the correct paths for your downloaded data and ipynb file.
Run the cells in chronological order.

Load each HDF5 MRI volume.
Quantify tissue types in each slice.
Simulate tumor growth slice-by-slice.
Blend synthetic tumors into each modality.
Save the synthetic MRI volume and tumor mask in the output directory.

Outputs:
Each synthetic HDF5 file will contain the following (in the synthetic tumor folder)

image: Multi-modal synthetic MRI

mask: Binary tumor mask (1 = tumor, 0 = background)

These files can be used for training tumor segmentation models.
