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
#### If it is your first time building:
1. Select File -> Open -> Select `/home/ws/build/compile_commands.json`
2. Select Call Tools -> Compilation Database -> Change Project Root `/home/ws`
3. IDE will now not yell at you about files being out of project scope
#### More information can be found at [link](https://www.jetbrains.com/help/clion/compilation-database.html#compdb_load)
