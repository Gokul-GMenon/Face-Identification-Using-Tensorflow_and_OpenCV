# Face-Detection-Using-Tensorflow_and_OpenCV
A face detection model has been build using transfer learning on the MobileNet architecture. The model has then been implemented using openCV to detect faces in live streams.

## Working
The model has been trained on the face of a single person(40-50 images should be enough, ideally as diverese as possible). The model then uses this database to train and reach near 100% accuracy in 5 epochs at maxium. We then import the model in detector.ipynb and use the stock face detector of openCV to detect the face and crop that part out. We pass this cropped image to the predictor and obtain results. Also, the openCV face detector is used to draw a bounding box around the face.

## How to make it work
- Copy sample images of the target and paste it into 'Dataset/Me'.
- Copy sample images of other faces and paste it into 'Dataset/NOT-Me'.
- Train the model in model_train.ipynb for sufficient epochs.
- Run the 'detector.ipynb' file and remember to fill in your name in the 'class_names' list variable
- Enjoy!!


##### NOTE: Best if the images in both datasets are as diverese (in conditions) as possible
