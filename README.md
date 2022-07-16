# Install-Ros-
How install Ros 
First step : installing VirtualBox
VirtualBox is open-source software for virtualizing the x86 computing architecture. It acts as a hypervisor, creating a VM (virtual machine) where the user can run another OS (operating system).
Downloading VirtualBox :
https://www.virtualbox.org/wiki/Downloads

Second step: installing Ubuntu
Is an open source.
Downloading Ubuntu :
https://ubuntu.com/download

Third step: 
Set up a VirtualBox and modify setting.
Now go to the terminal :
sudo apt-get update
sudo apt-get upgrade
sudo apt install build-essential dkms linux-headers-$(uname -r)
sudo apt install curl


curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -
sudo apt-get update
ROS distributions are linked to Ubuntu versions:

Ubuntu 20.04 -> Noetic
sudo apt-get install ros-noetic-desktop-full
echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc

source ~/.bashrc
sudo apt install python3-rosdep python3-rosinstall python3-rosinstall-generator python3-wstool build-essential

sudo apt install python3-rosdep
sudo rosdep init
rosdep update
mkdir -p ~/catkin_ws/src
cd ~/catkin_ws/
catkin_make
cd ~/catkin_ws/src

