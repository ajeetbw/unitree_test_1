# Unitree Robot SDK Version 2
Unitree robot sdk version 2 is a comprehensive software development kit designed to provide a robust and efficient way to interact with Unitree robots. This SDK is built on top of a range of cutting-edge technologies and provides a wide range of features and tools to support the development of robotic applications.

## Project Description
The Unitree Robot SDK Version 2 is designed to provide a unified interface for interacting with Unitree robots, allowing developers to create a wide range of applications, from simple robotic tasks to complex autonomous systems. The SDK provides a set of APIs and tools that enable developers to control and interact with the robot's hardware and software components, including motors, sensors, and control systems.

## Tech Stack
The Unitree Robot SDK Version 2 is built using a range of technologies, including:
* **Programming Languages:** C++, Python
* **Frameworks:** CMake, Eigen, Boost
* **Libraries:** YAML-CPP, Spdlog, Fmt
* **Operating Systems:** Ubuntu 20.04 LTS (aarch64 and x86_64)

## Installation and Startup
To install and start using the Unitree Robot SDK Version 2, follow these steps:
### Environment Setup
Before building or running the SDK, ensure the following dependencies are installed:
* CMake (version 3.10 or higher)
* GCC (version 9.4.0)
* Make
You can install the required packages on Ubuntu 20.04 with:
```bash
apt-get update
apt-get install -y cmake g++ build-essential libyaml-cpp-dev libeigen3-dev libboost-all-dev libspdlog-dev libfmt-dev
```
### Build Examples
To build the examples inside this repository:
```bash
mkdir build
cd build
cmake ..
make
```
### Installation
To build your own application with the SDK, you can install the unitree_sdk2 to your system directory:
```bash
mkdir build
cd build
cmake ..
sudo make install
```
Or install unitree_sdk2 to a specified directory:
```bash
mkdir build
cd build
cmake .. -DCMAKE_INSTALL_PREFIX=/opt/unitree_robotics
sudo make install
```

## Basic Usage
The Unitree Robot SDK Version 2 provides a range of APIs and tools for interacting with the robot. For example, you can use the `params.json` file to configure the robot's parameters, such as the `dt`, `kp`, and `kd` values:
```json
{
    "dt": 0.01,
    "kp": 40.0,
    "kd": 1.0,
    "init_pos": [
        0.0,
        0.9,
        -1.8,
        0.0,
        0.9,
        -1.8,
        0.0,
        0.9,
        -1.8,
        0.0,
        0.9,
        -1.8
    ]
}
```
You can also use the `PR Mode` interface to control the robot's parallel mechanism, such as the ankle joints of the H1_2 robot.

## Contributing
The Unitree Robot SDK Version 2 is an open-source project, and we welcome contributions from the community. To contribute, please fork the repository and submit a pull request with your changes. Please ensure that your code is well-documented and follows the project's coding standards.

## Licensing
The Unitree Robot SDK Version 2 is licensed under the [MIT License](https://opensource.org/licenses/MIT). By contributing to the project, you agree to release your contributions under the same license.