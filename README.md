# BOMR_2020


## Obstacle Avoidance
### Sensors
7 proximity sensor (5-front 2-back)  
Range : up to 14 cm (below 3cm, the distance calculation is not precise)  
Dynamic range : 36,51dB [D=20log(10)(Range/Δx)]
Update ferquency = 10 Hz (Generate prox event)  
Resolution = ~0.003 cm  
Accuracy = ~97.84%  

For 2 cm threshold : sensor value (prox.horizontal) = ~4000  


### Algorithm
Inputs : occupancy grid, path  
Outputs : new occupancy grid, new path  

1) Check sensors < threshold  
2) If nothing, return occupancy grid, path  
3) Else compute where it is (regarding to the robot)  
4) Calcuate new path  
5) Update and return new occupancy grid and new path  
