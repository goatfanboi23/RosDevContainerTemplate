# Template for creating ROS2 devcontainer
Adopted from [link](https://docs.ros.org/en/jazzy/How-To-Guides/Setup-ROS-2-with-VSCode-and-Docker-Container.html)
## Setup
### `ws/.devcontainer/devcontainer.json`
1. Replace field in `remoteUser: "user"` with host username
2. Replace field `USERNAME: "user"` with container username
### ws/src
1. Create src folder
2. Create ros package in src

## Post Setup
Follow the instructions in your IDE of choice on using Dev Containers
### Jetbrains specific
1. When Building colcon add the following `--cmake-args -DCMAKE_EXPORT_COMPILE_COMMANDS=ON`
2. Press File -> Open -> Select `/home/ws/build/compile_commands.json`
3. IDE will now not yell at you about packages not being in project target
