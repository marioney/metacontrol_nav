# Metacontrol Navigation

This package contains launcher and configuration files for the navigation stack for the ridgeback robot.

## Launch Simulation
### Including ridgeback + yumi
```
$ roslaunch metacontrol_sim ridgeback_world.launch gui:=true
```
###  Only ridgeback base
```
$ roslaunch metacontrol_sim ridgeback_yumi_world.launch gui:=true
```

## Launch navigation

### Without map

```
$ roslaunch metacontrol_nav odom_navigation_<fast/standard/safe>.launch
```

### With map

* fake_localization can be used to lower computing requirements of the Simulation. This can be controlled by the `use_fake_localization` argument

```
$ roslaunch metacontrol_nav amcl_demo_<fast/standard/safe>.launch use_fake_localization:="true"

```
