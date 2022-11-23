# gazebo_world

## Latest How to is here 

[Latest Tutorial](https://github.com/FahrulID/catatan_belajar_ros/blob/main/HOW_TO_ADD_CUSTOM_WORLD_GAZEBO.md)
## How to World in Gazebo
- Copy the temp_world folder to ```~/PX4-Autopilot/Tools/sitl_gazebo/models ```
- Change the .mesh name in template.world to the mesh u want to use
- Copy the template.world to ```~/PX4-Autopilot/Tools/sitl_gazebo/worlds ```
- Add the world name in ```~/PX4-Autopilot/platforms/posix/cmake/sitl_target.cmake``` in line set worlds (in this case, 'template' from template.world is the name)
- Launch the world ```make px4_sitl gazebo___template```
