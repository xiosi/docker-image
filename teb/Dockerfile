FROM ros:kinetic-ros-core
RUN sed -i "s/archive.ubuntu.com/mirrors.ustc.edu.cn/g" /etc/apt/sources.list
RUN echo "deb http://mirrors.ustc.edu.cn/ros/ubuntu/ xenial main" > /etc/apt/sources.list.d/ros-latest.list
RUN apt-get update && apt-get install -y  software-properties-common ros-kinetic-teb-local-planner \
    ros-kinetic-rqt ros-kinetic-rqt-common-plugins ros-kinetic-turtlesim \
    ros-kinetic-teb-local-planner-tutorials ros-kinetic-rviz \
    && apt-get clean

#sudo apt-get install ros-indigo-rqt ros-indigo-rqt-common-plugins ros-indigo-turtlesim
#net_tools