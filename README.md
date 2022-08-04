# AI_1_B

Downloading Ros on Jetson nano:
First, we need to choose a ROS version that we want, for me I chose Kinetic. Then we shall write the following code to install ROS:
sudo sh -c 'echo "deb  http://packages.ros.org/ros/ubuntu  $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'

Add a new apt key:

sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654

sudo apt update

sudo apt install ros-kinetic-desktop

sudo rosdep init

rosdep update

echo "source /opt/ros/kinetic/setup.bash" >> ~/.bashrc

source ~/.bashrc

rosversion -d


// after that the terminal will show the word kinetic, which means ROS has been installed successfully and ready to use for jetson nano.

Now we can connect Jetson nano to our device and start our work easily. 
