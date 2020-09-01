# Poject
ROS hand position detected 

First , do catkin_make 

Then extract hand.zip into new catkin src file . 

Then downlaod the weight cofig file fllow this link
because the files size too big , so I have upload on google drive) :https://drive.google.com/drive/folders/1qie3u_3w_yUqcw8JA9Fwz5sjGJIckCMb?usp=sharing

There are 4 files in side config file , which are train_final.weight , train_cfg , pose_iter_1020000.caffemodel and pose_deploy.prototxt.
for train_final.weight and train_cfg you need to seeting up src into taker.py , for pose_iter_1020000.caffemodel and pose_deploy.prototxt you need sett up src inside pose.py

once you finished src setting , now do : chmod +x talker.py, chmod +x listener1.py  and chmod +x listener1.py.

TO lunch the talker and listener1 and 2 , do fllowing setps :
cd ~/tracing_hands 
source ./devel/setup.bash
start a new terminal :roscore

start a new terminal :cd ~/tracing_hands
source ./devel/setup.bash
rosrun tracing_hands talker.py

start a new terminal :cd ~/tracing_hands
source ./devel/setup.bash
rosrun tracing_hands listener1.py

start a new terminal :cd ~/tracing_hands
source ./devel/setup.bash
rosrun tracing_hands listener2.py

