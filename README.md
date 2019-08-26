## EY Nextwave Data Science Challenge April 2019

### Task
Predict whether a car would be in the city center of their last trajectory after 15:00, given their prior trajectories, and their last known coordinate and time_start/time_end of this last trajectory 

### Methodology
Initial baseline attempt:

Being in the city center at the start of their trajectory after 15:00 was a strong indicator that they would remain in the city center; many of the observations had trajectories taking place over 0 seconds

Best attempt:

Used XGBoost, added the last 2 positions (i.e. the prior trajectory coordinates) + the origin coordinate; many of the devices had a small number of trajectories in their overall journey.  This likely allowed the model to effectively learn a set of rules / non-linear decision boundary

Next time:

Methods such as Dynamic Time Warping, ConvNets could also be tested
