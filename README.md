# upstart_ssh

ignore the lnt_urdf deciption.(i added here temp to vis the axes of l_T arm)

reference:
1.https://husarion.com/core2/tutorials/ros-tutorials/5-running-ros-on-multiple-machines/#5-running-ros-on-multiple-machines-introduction
2.http://wiki.ros.org/ROS/Tutorials/MultipleMachines 

setps:

1. start the ssh service in rpi by: sudo service ssh restart
2. check it by:sudo srvice ssh active
3. from your system log into pi by: pi@ip_address
4. you can find the ip address of rpi by7 either hostanme -I or ifconfig 
5. set the following environment varibales:
        export ROS_MASTER_URI=http://xxx.xxx.xxx.xxx:11311
        export ROS_IP=xxx.xxx.xxx.xxx (for NUC)
        
        export ROS_MASTER_URI=http://xxx.xxx.xxx.xxx:11311
        export ROS_IP=yyy.yyy.yyy.yyy (for RPI)
6. Now launch the file dummy.launch
7. To make it automatically execetute this launch file when the systems boots up pass this file to upstart pacakge.
        
      
       
        
        
