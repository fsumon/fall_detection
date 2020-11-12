# fall_detection
Fall detection models 
HAR-UP original dataset file is trimmed to filter only selected 10 wearable sensors data. Those sensor are as below,
AnkleAccelerometer
AnkleAngularVelocity
RightPocketAccelerometer
RightPocketAngularVelocity
BeltAccelerometer
BeltAngularVelocity
NeckAccelerometer
NeckAngularVelocity
WristAccelerometer
WristAngularVelocity
Then the RMS values of the triaxis of the sensors are generated and saved into the "HAR_UP_Fall_Detection_v3.csv" file.
To get the RMS the following forumula is used for each sensor,
 RMS = SQRT ( x^2+y^2+z^2)
Target file is "Fall_Detection_Target4.txt"
Subject 5,8,9 are removed from the files as  RightPocketAccelerometer and RightPocketAngularVelocity values are ZERO for those participants (missing values)
LSTM network is used to build the models.
