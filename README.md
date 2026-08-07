# Ros-
# ROS 2 Humble Installation on Ubuntu 22.04

## Step 1: Update Ubuntu
sudo apt update && sudo apt upgrade -y

## Step 2: Install Required Packages
sudo apt install software-properties-common curl -y

## Step 3: Add the ROS 2 GPG Key
sudo curl -sSL https://raw.githubusercontent.com/ros/rosdistro/master/ros.key -o /usr/share/keyrings/ros-archive-keyring.gpg

## Step 4: Add the ROS 2 Repository
echo "deb [arch=amd64 signed-by=/usr/share/keyrings/ros-archive-keyring.gpg] http://packages.ros.org/ros2/ubuntu jammy main" | sudo tee /etc/apt/sources.list.d/ros2.list > /dev/null

## Step 5: Update the Package List
sudo apt update

## Step 6: Install ROS 2 Humble Desktop
sudo apt install ros-humble-desktop -y

## Step 7: Configure ROS 2 Environment
echo "source /opt/ros/humble/setup.bash" >> ~/.bashrc

## Step 8: Apply the Configuration
source ~/.bashrc

## Step 9: Check ROS 2 Version
ros2 --version

## Step 10: Check ROS 2 Distribution
echo $ROS_DISTRO

Expected Output:
humble

## Conclusion
ROS 2 Humble was successfully installed and configured on Ubuntu 22.04.
