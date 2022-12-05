# Group-465
Group members: Mariam Khan, Vi Nguyen, Beth Haessler

Project Description: Final Project for 465 (Secure Transportation Systems)

Details: We decided to slightly switch gears from our original idea (Blindness of car's systems due to loss of camera data and function) to swapping the data streams of the LiDAR detectors (front receives back stream and back receives front stream). This will have the same affect we originally proposed of blinding the car's systems just in a different way. 

*First attempt at disrupting the Lidar Sensors*
  We discovered in our research that is was possible to show all of the processes running in the docker container. We then decided to look into these to see if this might be able to help us find a way to disrupt the sensors. We then went back to researching and found that we could end processes running in docker if we knew their PID (short name for IDK what). 
   we ten looked through our docker PIDs using the command [], and decided to try ending the Ray_Ground_Classifier jsut to see if we could see a difference (which is shown below). After noting this we decided to try and end the Velodyne_Node process (the before and afters of that are also shown below) 
   
   **Before ending ray ground**
   
   **After ending ray groufnd**
   
   
   **Before ending Veladyne Node**
   
   **aftrer ending veladyne node**
   
   
