# Facial Keypoints Detection

# Description
The objective of this task is to predict keypoint positions on face images. This can be used as a building block in several applications, such as:
- tracking image and video,
- analyzing facial expressions,
- detecting dysmorphic facial signs for medical diagnosis,
- biometrics / face recognition

Detecing facial keypoints is a very challenging problem.  Facial features vary greatly from one individual to another, and even for a single individual, there is a large amount of variation due to 3D pose, size, position, viewing angle, and illumination conditions. Computer vision research has come a long way in addressing these difficulties, but there remain many opportunities for improvement.

This getting-started competition provides a benchmark data set and an R tutorial to get you going on analysing face images.

# Evaluation
Submissions are scored on the root mean squared error. RMSE is very common and is a suitable general-purpose error metric. Compared to the Mean Absolute Error, RMSE punishes large errors:
<img width="185" height="65" alt="rmse" src="https://github.com/user-attachments/assets/3a5f8ebc-0679-4465-bf49-4b501591b4c5" />

where y hat is the predicted value and y is the original value.

# Submission Instructions
Please download the file submissionFileFormat.csv from the data page. This file lists the points whose locations need to be detected.

Submission file columns:
- Row Id: Integer id for the row.
- Image Id: Integer id for the image. There are 1783 images in the test set.
- Feature Name: String identifying the facial keypoint, e.g., left_eye_center_x, left_eye_center_y, mouth_bottom_center_lip_x, nose_tip_y.
- Location: x- or y-coordinate of the specified feature. This is the value to be predicted.

# Submission File
Note that you will not be detecting all 30 features (x and y coordinates for 15 facial keypoints) for each image. Some images require fewer keypoints to be detected. Please see the file submissionFileFormat.csv for details. The format looks like this:
<img width="452" height="109" alt="submission" src="https://github.com/user-attachments/assets/c08103d7-d274-4785-85ea-649a63cb93d2" />
