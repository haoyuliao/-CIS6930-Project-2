# CIS6930-Project-2
* This Project tries to do deep colorization to transfer from the grayscale image into RGB scale image.

## Environmental setting recommendation
* Recommend to use Anaconda 64-bit to build the environment for applying CUDA to run GPU and used the Jupyter notebook from Anaconda to build Pytorch programs. 
* Recommend to use Anaconda with the Jupyter notebook to run our programs with the same environmental setting.

* Below are folders containing each file are expressed (Folder-> Each file).
## Programs 
* The main programs are the RegressorColorizing.ipynb and ColorizingSigmoidChangeFM.ipynb for the project.
 1. face_images: a dataset of 750 images.
 2. ColorizingRelu.ipynb: Input L*, and output matrix a* and b* with ReLU last layer. Then, colorizing the images.
 3. ColorizingSigmoid.ipynb: Input L*, and output matrix a* and b* with Sigmoid last layer. Then, colorizing the images.
 4. ColorizingSigmoidChangeFM.ipynb: Input L*, output matrix a* and b* with Sigmoid last layer, and change each layers' feature maps. Then, colorizing the images.
 5. ColorizingTanh.ipynb: Input L*, output matrix a* and b* with Tanh last layer. Then, colorizing the images.
 6. RegressorColorizing.ipynb:  Input L* and predicted mean scalar a* and b* by regressor. Output matrix a* and b* with Sigmoid last layer. (3 input factors L*, scalar a*, and b*; 2 output factors matrix a* and b*)
 7. Regressor.ipynb: Input L*, prediction mean scalar a* and b*.
 8. ImplementTrainedModel4Colorizing.ipynb: Implement trained parameters to color images without training again. Only for ColorizingSigmoid, ColorizingSigmoidChangeFM, and ColorizingRelu trained model. Please select a correct net model for corresponded trained parameters.
 9. ImplementTrainedModel4CombRegClo.ipynb: Implement trained parameters to color images without training again. Only for RegressorColorizing trained model.

## TrainedModel 
* These archives are trained models and can be applied by ImplementTrainedModel4Colorizing.ipynb and ImplementTrainedModel4CombRegClo.ipynb to redrawing images.
 1. ColorizingReludWithLR0.1EP1000.pth: Trained model of ColorizingRelu.ipynb program.
 2. ColorizingSigmoidWithLR0.1EP1000.pth: Trained model of ColorizingSigmoid.ipynb program.
 3. ColorizingSigmoidChangeFMTrainTestLogEP1000.pth: Trained model of ColorizingSigmoidChangeFM.ipynb program.
 4. ColorizingTanhdWithLR0.1EP1000.pth: Trained model of ColorizingTanh.ipynb program.
 5. ColorizingCombWithLR0.1EP1000: Trained model of RegressorColorizing.ipynb program for colorizing model.
 6. RegCombWithLR0.1EP1000.pth: Trained model of RegressorColorizing.ipynb program for regression model.
 7. RegWithLR0.1EP1000.pth: Trained model of Regressor.ipynb program.

## TrainTestImagesRes
* Test results are the same images.
 1. ColorizingRelu-*-*.png: Training and testing image results of ColorizingRelu.ipynb.
 2. ColorizingSigmoid-*-*.png: Training and testing image results of ColorizingSigmoid.ipynb.
 3. ColorizingSigmoidChangeFM-*-*.png: Training and testing image results of ColorizingSigmoidChangeFM.ipynb.
 4. ColorizingTanh-*-*.png: Training and testing image results of ColorizingTanh.ipynb.
 5. ColorizingComb-*-*.png: Training and testing image results of RegressorColorizing.ipynb for colorizing model.
 
## TrainTestLog
* First to last the second line are training records, and the last line is testing records.
 1. ColorizingReluTrainTestLog1000.txt: The training and testing log of ColorizingRelu.ipynb.
 2. ColorizingSigmoidTrainTestLog1000.txt: The training and testing log of ColorizingSigmoid.ipynb.
 3. ColorizingSigmoidChangeFMTrainTestLogEP1000.txt: The training and testing log of ColorizingSigmoidChangeFM.ipynb. 
 4. ColorizingTanhTrainTestLogEP1000.txt: The training and testing log of ColorizingTanh.ipynb.
 5. ColorizingCombTrainTestLogEP1000.txt: The training and testing log of RegressorColorizing.ipynb program for colorizing model.
 6. RegCombTrainTestLogEP1000.txt: The training and testing log of RegressorColorizing.ipynb program for the regression model.
 7. RegTrainTestLog1000.txt: The training and testing log of Regressor.ipynb program.
