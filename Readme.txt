The dataset consists of three motion types of the rendered image dataset.
The three rendering image data sets correspond to three kinds of camera object motion respectively, namely, object translation and rotation camera still, object only rotating camera still, and object still camera-free motion, including 13 cameras, 7 cameras, and 3 cameras respectively. 

Binocular and trinocular are obtained by using a combination of different cameras, for example, C-0/C-1 represents the use of camera 0 and camera 1 in the corresponding motion. Besides, we tested each camera on four different objects - Cat, Clown, Driller, Squirrel - in the Model folder. 

Besides, we provide the ground truth information of the object relative to the camera. At the same time, the relative pose between the cameras can be calculated by the actual pose of the object relative to different cameras.

The internal parameter K of the camera used for rendering data is
K=[700.03    0        320]
     [ 0       700.03    240]
     [ 0           0           1 ]

The truth file corresponding to each camera in the rendering data contains 300 rows of data, namely 300 frames. Each row has 12 parameters, which in turn are r11, r12, r13, r21, r22, r23, r31, r32, r33, tx, ty, tz. The meanings of each parameter are as follows
T = [r11  r12  r13  tx]
      [r21  r22  r23  ty]
      [r31  r32  r33  tz]
      [ 0      0     0     1]

For more information on the dataset, please read our article: