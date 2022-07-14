# Install-Ros
Install Ros OS 
i have downloaded three apps the first one is virtualbox witch is a simulator, and the second is Ubuntu is free and open-source software for Linux 
and the last one is ROS 
the main two problem that i have faced in installing is that the size is limeted to 10GB and when i start installing in the Terminal shows me the error of space not enough, the second one is that i have to install ROS acourding to the Ubuntu version 
and the installing simpliy copy and paste the command that i have search for in the internet for the ROS
and will add an image that show ROS OS that has been installed 

that's it for the steps to install ROS on my PC knoow the steps for installing ROS to Jetson Nano 

First Open a new terminal 

Set up the Jetson Nano to accept software from packages.ros.org:
$ sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'

Add a new apt key:
$ sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654

Update the Debian packages index:
$ sudo apt update

Install the ROS Desktop package, including support for rqt, rvizand other useful robotics packages:
$ sudo apt install ros-melodic-desktop

$ echo "source /opt/ros/melodic/setup.bash" >> ~/.bashrc 
$ source ~/.bashrc

Install and initialize rosdep. rosdep enables you to easily install system dependencies for source code you want to compile and is required to run some core components in ROS:

$ sudo apt install python-rosdep python-rosinstall python-rosinstall-generator python-wstool build-essential
$ sudo rosdep init 
$ rosdep update

and that's it
