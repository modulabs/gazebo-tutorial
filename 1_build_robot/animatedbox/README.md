## Animated Box

### Build the plugin
    $ mkdir build
    $ cd build
    $ cmake ..
    $ make

### Make sure Gazebo can know this plugin path
    $ export GAZEBO_PLUGIN_PATH='pwd':$GAZEBO_PLUGIN_PATH

### Run

#### Simulate with gazebo

Run gazebo
    $ gazebo animated_box.world

#### Connect to a simulation with your own executable
    $ gazebo animated_box.world & ./build/independent_listener

#### Run the simulation and connect with your own executable
    $ ./build/integrated_main animated_box.world
To view the simulation
    $ gzclient

### Reference
1. [Gazebo: Tutorial: Animated Box](http://gazebosim.org/tutorials?tut=animated_box&cat=build_robot)