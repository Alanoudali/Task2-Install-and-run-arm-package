# Task2-Install-and-run-arm-package
Welcome to the Task2-Install-and-run-arm-package wiki! After installing ROS, we follow the following commands to run the arm package

mkdir -p ~/catkin_ws/src

cd ~/catkin_ws/

catkin_make

cd ~/catkin_ws/src

git clone https://github.com/smart-methods/arduino_robot_arm.git

cd ~/catkin_ws

rosdep install --from-paths src --ignore-src -r -y

sudo apt-get install ros-kinetic-moveit

sudo apt-get install ros-kinetic-joint-state-publisher ros-kinetic-joint-state-publisher-gui

sudo apt-get install ros-kinetic-gazebo-ros-control joint-state-publisher

sudo apt-get install ros-kinetic-ros-controllers ros-kinetic-ros-control

sudo nano ~/.bashrc

at the end of the (bashrc) file add the follwing line

(source /home/anoud/catkin_ws/devel/setup.bash)

then

ctrl + o

source ~/.bashrc

When this command is inserted, the package is opened and the program is run

roslaunch robot_arm_pkg check_motors.launch ‏‏لقطة الشاشة (720) ‏‏لقطة الشاشة (722)
