# Disaster Relief Robot

The environment set up in this scenario is a bathroom with one person standing at the sink and another person laying down unconscious on the floor. The environment has 4 walls surrounding it, a door, toilets, a few sinks on the wall, and walls between each toilet. The person collapsed on the floor is next to a toilet and the other person is standing at the sink.  

This robot is used to detect the people in a disaster scenario. In this demonstration, both people are detected by the robot and a message is printed out, “I found a person!” This is to show how the robot can be used to locate victims in a disaster scenario like a bomb threat, collapsed building, gas leak, fire, etc. The sensors are used to navigate around the environment and to detect the people. When the robot senses an obstacle (like the walls of the bathroom) it slowly backs up, turns, and then moves forward in a different direction.  

The robot uses the BubbleRob tutorial robot and has three sensors total. One of them is the visual sensor for the environment used to navigate around obstacles. The other two are used to detect the people and print out the statement “I found a person!” when a person is detected. The two added visual sensors for finding people have a much wider range and scope so that they can more easily detect humans the robot drives near. The two added sensors have been adjusted to identify the human entity obstacles. The human obstacles have been modified so that they are detectable by the sensor.   

The robot uses the proximity sensor to detect objects in front of it and back up slowly at an angle then go forward again.  It does not store this information in a map, which make it unfortunately not very efficient and it will go over the same spot in the future attempting to detect humans. The robot also uses its other two visual sensors to detect humans. It prints out that it has found a human when a human enters its visual sensor.   

Reasoning: The robot uses its sensors to detect the environment and maneuver around any obstacles it senses. When it bumps into the wall, it backs up and changes direction to maneuver around it. When it does back up, it does so at a slower speed. When it senses a person, the statement “I found a person!” is printed to the console. 
	
 
 Knowledge representation: The robot uses all of its sensors to collect information about the environment. The visual sensor is used to navigate around the environment. The other two sensors are used to detect people. These sensors are distance based from the robot and detect the information the closer the obstacle is to the range of the sensor.
	
 
 Uncertainty: The robot’s visual sensor and maneuverability allows it to navigate any environment it was placed in where it could wheel around. If the obstacles and people were moved around, the robot would still back up at an angle and move in a different direction. This would keep occurring while the robot is moving around and allow it to explore as much of the area as possible.
	
 
 Intelligence: The functions of the sensors, wheels, and motors allows the robot to achieve its goal of finding people and maneuvering around the environment. The wheels and motors are what allows the robot to maneuver. The sensors allows the robot to navigate the environment and detect any people it finds.


# Further Improvements: 

Reinforced Learning: Reinforced learning could be used with this robot to learn how to navigate through rooms better. Right now the robot backs up at the same degree before turning. This leads to the robot navigating the environment very slowly. The robot could learn what the best angles are before bumping into another obstacle to then cover the most distance in an environment.


Advanced Search Algorithms: Advanced search algorithms would allow the robot to have multiple things it could store and search for when attempting to detect humans. Right now, the robot searches for a Bill model to then state it found a human. Advanced search could be used to detect different things like pieces of clothing, skin, etc. This would allow multiple things to be detected and while it may trigger a human is detected more frequently, it would make sure humans could also be missed less in its detection.


The robot could also be improved to go over obstacles better. If a collapsed building were to occur, it would need to be equipped with a stabilizer, four wheels to navigate over fallen objects, etc. It could also use some water-proofing to make sure none of the sensors get damaged.
