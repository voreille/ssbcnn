# Local rotation invariance in 3D CNNs
Implementation of the 3D Locally Rotation Invariant CNNs developed in "3D Solid Spherical Bispectrum CNNs for Biomedical Texture Analysis", Valentin Oreiller, Vincent Andrearczyk, Julien Fageot, John O. Prior, Adrien Depeursinge. Paper submitted to IEEE TMI.

# How to use it
To obtain LRI, the first convolution of a 3D CNN can be replaced by one of the LRI variants: 
- sse_conv3d and bispectrum_conv3d are defined in ./sh_networks_utils.py is obtained by calculating invariants in the form of Solid Spherical Energy (SSE) or Solid Spherical Bispectrum (SSB) from the response to convolutions with spherical harmonics.

Example usage is provided on a basic synthetic texture dataset in ./synthetic_experiments/


# Installation and Requirements
The environment needed to run the experiments must include Tensorflow 1.14.0

The list of python dependecies is provided in requirements.txt and can be installed by running:
pip install -r requirements.txt
