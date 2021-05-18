#############GREETINGS ON BEHALF OF CNN SPEEDUP WITH SPARSITY TEAM#########
The present github repo/model can be used in two ways:
1. Download/clone the repo to your local server/PC/edge computer
2. Use the Google Colab notebook version of this repo
#############For Path 1####################################################
a. Install all the required libraries as mentioned in requirements.txt file
b. If you wish to change the sparsity percent (by default it is kept 30% because it is optimal), got to:
	test.py>In prune section, change the second argument of prune(model,0.3) between 0 to 0.9 
	meaning varying Sparsity percent between 0 to 90 percent
c. Once done, SAVE the file
d. The images to be tested/ detected should be added in
	data>images> HERE
	(by default the surveillance feed from Sentry.ai is used)
e. Open the command prompt and navigate to your directory (If Windows)
e. For detection run the following:
	python detect.py –source 0                 #webcam detection
	python detect.py –source file.jpg     	   #image detection
	python detect.py –source file.mp4          #video detection
f. For testing run the following:
	python test.py
#############For Path 2#################################################### 
It is the most easiest way to have a quick sneak into the inferences of this model
Run the cells in the order followed
The Github repository will get automatically uploaded in the colab engine. 
By default, the testing is done on COCO128 dataset from kaggle and COCO val2017 dataset

############ENJOY THE SPEED BOOST :) ######################################
In case of issues contact the contributors! 