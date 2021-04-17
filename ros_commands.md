## ROS Commands:
* create a new package with dependencies
```
catkin_create_pkg <package_name> [depend1] [depend2] [depend3]
```
* Review first-order dependencies 
```
 rospack depends1 <package_name> 
 #for indirect dependencies
 rospack depends <package_name> 
```
* Source your environment setup file
```
source /opt/ros/%YOUR_ROS_DISTRO%/setup.bash
```
* Start up a ROS Master, a ROS Parameter Server and a rosout logging node
```
roscore
```
* Display information about the ROS nodes that are currently running
```
rosnode
```
* Use the package name to directly run a node within a package
```
rosrun [package_name] [node_name]
```
* Create a dynamic graph of what's going on in the system
```
rosrun rqt_graph rqt_graph
rqt_graph
```
* Get information about ROS topics
```
rostopic -h
```
* Get message type of any topic being published
```
rostopic type [topic]
```
* Look at the details of the message
```
 rosmsg show [message]
```
* Publishe data on to a topic currently advertised
```
 rostopic pub [topic] [msg_type] [args]
```
* Report the rate at which data is published
```
 rostopic hz [topic]
```
* Display a scrolling time plot of the data published on topics.
```
 rosrun rqt_plot rqt_plot
```
* ROS Services: allow nodes to send a request and receive a response
```
rosservice type [service]
rosservice call [service] [args]
```
* ROS Parameters: allow to store and manipulate data on the ROS Parameter Server
```
rosparam list
rosparam set [param_name]
rosparam get [param_name]
rosparam dump [file_name] [namespace] #write all the parameters to a file
rosparam load [file_name] [namespace]
```
* For debuging:
```
rosrun rqt_console rqt_console
rosrun rqt_logger_level rqt_logger_level
```
* Start nodes as defined in a launch file
```
roslaunch [package] [filename.launch]
```

* E dit a file directly within a package by using the package name rather than having to type the entire path to the package:
```
rosed [package_name] [filename]
```









