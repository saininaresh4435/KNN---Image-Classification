 KNN---Image-Classification approach-
Firstly I import important libraries.
After that I use cv2.VideoCapture() function to get image frames from the video.Then I use vidcap.read() this function to read the  image and by using cv2.imwrite(name,image) we can write the image to a folder.I store all image into different folder from 0 to 51 for different video for both class jogging and walking.
After that I load all the image for all videos for both class and store them into img_jogging and img_walking dictionary
After that this image dictionary is converted into numpy array.
After that I append both the image folder into a single dataset X along axis=0.
Then calculate mean of X dataset along axis=1.
After that I create numpy array of zero corresponding to Jogging and ones corresponding to walking.
Append both the numpy array along axis=0 and get Y data.
After that to get the final dataset we append both X and Y along axis=1.
Random suffle the dataset by using predefiend function.
By using train_test_split we can split the data set into training and test set.
Then we can fit  KNeighborsClassifier() by using train dataset for different values of k.
Finally we can predict the value corresponding to x_test data set and can get accuracy_score of the model. 
