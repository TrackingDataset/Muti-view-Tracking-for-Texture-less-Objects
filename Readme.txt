The synthetic dataset has 3 modes, including 1) Object moves freely with fixed cameras, 2) Object rotates only with fixed cameras, and 3) Cameras move freely. For the detailed description, please refer to the manuscript and supplementary material.

Binocular tracking, triple-view, and multi-view tracking are combined with different cameras. For example, C-0/C-1 represents the use of camera 0 and camera 1 in the corresponding mode. Besides, we have 4 models in each mode, i.e., Cat, Clown, Driller, and Squirrel. 

Furthermore, we provide the ground truth of the object pose relative to the cameras. Simultaneously, the relative pose between the cameras can be calculated by the object pose in corresponding cameras.

The intrinsic parameter K of cameras is:
K=[700.03    0        320]
  [ 0       700.03    240]
  [ 0        0         1 ]

In ground truth file, each row has 12 parameter (r11, r12, r13, r21, r22, r23, r31, r32, r33, tx, ty, tz). The extrinsic parameter T is:
T = [r11  r12  r13  tx]
    [r21  r22  r23  ty]
    [r31  r32  r33  tz]
    [ 0    0    0    1]
    
