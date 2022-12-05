# Group-465
Group members: Mariam Khan, Vi Nguyen, Beth Haessler

Project Description: Final Project for 465 (Secure Transportation Systems)

Details: We decided to slightly switch gears from our original idea (Blindness of car's systems due to loss of camera data and function) to swapping the data streams of the LiDAR detectors (front receives back stream and back receives front stream). This will have the same affect we originally proposed of blinding the car's systems just in a different way. 

*First attempt at disrupting the Lidar Sensors*

  We discovered in our research that is was possible to show all of the processes running in the docker container. We then decided to look into these to see if this might be able to help us find a way to disrupt the sensors. We then went back to researching and found that we could end processes running in docker if we knew their PID, or the id of the process. 
  We then looked through our docker PIDs using the command ps -aux which shows all the running processes in Linux, and decided to try ending the ray_ground_classifier to see if we could see a difference in the Autoware visualization (results shown below). After noting the changes, we decided to try and kill the velodyne_node process (the before and after of that are also shown below) 
   
   **Before ending ray_ground_classifier node**
   
   **After ending ray_ground_classifier node**
   
   
   **Before ending velodyne node**
   
   **After ending velodyne node**
   
