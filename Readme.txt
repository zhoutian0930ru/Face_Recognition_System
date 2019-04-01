1. Prerequisite:
  Python 3.6 with the tensorflow environment:
	You can set up the environment by following steps:
	* create an independent python 3.6 environment, then activate it
	* install the tensorflow program for python with following commands:
	pip install --ignore-installed --upgrade https://storage.googleapis.com/tensorflow/linux/cpu/tensorflow-1.6.0-cp36-cp36m-linux_x86_64.whl
	
  Installing OpenCV and Dlib packages:
	Moreover, all the packages related to those two modules should be installed (Just following the instructions in the terminal)
	
  Access to the PC camera:
	If using a virtual machine, make sure the Video Capture function works (Via USB driver etc.)
	
  LFW dataset:
	Facial images of people could be obtained at: http://vis-www.cs.umass.edu/lfw/person/Sylvester_Stallone.html
	
2. Commands in terminal；
	* activate the source environment with tensorflow (eg. source activate tensorflow)
	* cheese
		-- To make sure the camera works. If cheese not installed, install it first. 
	* run the capture program: python get_host_faces.py (Users can change the number of pictures of themselves as they want)
	* run the program to set labels and to do the face alignment for pictures in the dataset: python set_other_faces.py
	* run the training program to generate the metadata: python train.py
	* run the recognition program after successfully training: python recognition.py
	* See what happens!
	