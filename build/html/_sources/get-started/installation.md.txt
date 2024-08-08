# Installation


:::{note}  
**altair_ws**, based on ROS 2  
To start development, first install the **workspace requrements**
:::

:::{important}
**Workspace Requirements**

* Ubuntu 24.04 LTS - Nobble Numbat
* ROS 2 Jazzy Jalisco
* Dynamixel SDK
:::

## **Workspace Setup**

* Cloning The repo

   ```console
   git clone https://github.com/Altair-GMRT/altair-os/
   ```

* additional dependencies (sudo apt install):

   ``` console
   sudo apt install ros-jazzy-yaml-cpp-vendor ros-jazzy-eigen3-cmake-module ros-jazzy-eigen-stl-containers ros-jazzy-tf2 ros-jazzy-tf2-ros ros-jazzy-tf2-eigen
   ```

* ROS 2 Jazzy Jalisco Installation  
   https://docs.ros.org/en/jazzy/Installation/Alternatives/Ubuntu-Install-Binary.html

* Dynamixel SDK Installation  

   ```console
   sudo apt install make cmake  
   ```

   ```console
   git clone https://github.com/ROBOTIS-GIT/DynamixelSDK.git
   ```

   ```console
   cd DynamixelSDK/c++/build/linux64 && make && sudo make install
   ```
   

## **Build**

Go to the root folder of altair_ws, 'before the src folder', then  

   ```console
   colcon build
   ```

or to build selected single package

   ```console
   colcon build --packages-select "package-name"
   ```
