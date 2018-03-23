# Volnet
Disparity Estimate for Stereo images

The network Volnet is a convolution network that estimates disparity levels between two images
The network was trained using Sceneflow data set 
@InProceedings{MIFDB16,
  author    = "N.Mayer and E.Ilg and P.H{\"a}usser and P.Fischer and D.Cremers and A.Dosovitskiy and T.Brox",
  title     = "A Large Dataset to Train Convolutional Networks for Disparity, Optical Flow, and Scene Flow Estimation",
  booktitle = "IEEE International Conference on Computer Vision and Pattern Recognition (CVPR)",
  year      = "2016",
  note      = "arXiv:1512.02134",
  url       = "http://lmb.informatik.uni-freiburg.de/Publications/2016/MIFDB16"
}

To Run the network follow the following procedure:
1. Download the stereo dataset from the https://lmb.informatik.uni-freiburg.de/resources/datasets/SceneFlowDatasets.en.html
2. Arrange the data as expected in the code (sorry some insight into code is required here)
3. Execute all cells all the way until Training data
4. the networks works very well for disparity levels of upto 16. Still need to try the network for higher resolutions
5. For higher resolutions the training has to happen over several hours or even days which is why the current code is restrained to 16 levels of disparity
