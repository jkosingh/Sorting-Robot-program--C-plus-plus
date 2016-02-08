# C++-Sorting-Robot-program-

 This robot will work in a plant where juice is placed into glass bottles.  This plant uses many types of bottle. The robot you are programming separates 3 kinds of bottles from the container of bottles to be recycled.  It looks for small bottles made of clear glass, medium sized bottles made of green glass, and large bottles made of brown glass.  The small bottles weigh 38g ± 3g, the medium bottles weight 55g ± 5g, and the large bottles weigh 82g ± 8g. 
 
 
The robot sorts recycled bottles that have just been washed for the first time to remove dirt and other solids that might be in or on the bottles. The washed bottles arrive at the robot on a conveyor belt. The robot sorts the bottles.  The robot sorts bottles into the following groups, broken bottles (or fragments of bottles), green bottles (weighing 55g ± 5g), clear bottles (weighing 38g ± 3g), brown bottles (weighing 82g ± 8g) and bottles of all other sizes and/or colors.  The bottles (and fragments) to be sorted arrive on a conveyor belt.  The robot will pick up one bottle or bottle fragment, analyze it then, based on the results of the analysis, place it on the correct conveyer belt or place it in a waste container.

The robot places broken bottles in a waste container.  The waste container can hold a maximum weight of broken glass. When the container is full the robot signals that it needs to be replaced.  The robot places large brown bottles on one conveyor belt, medium green bottles on a second conveyor belt and the small clear bottles a third conveyor belt. These sorted bottles (the three types it is programmed to find) go to another washing and sterilizing facility before they are filled with juice. The remaining unbroken bottles are placed on a fourth conveyor belt and sent to another sorting robot in another part of the factory.

The robot will pick up a bottle (or a fragment of a bottle) from the incoming conveyor belt. As it picks up the bottle the robot is able to weigh the bottle. To weigh the bottle the robot measures the change in length of a spring, the heavier the bottle the longer the spring gets. The robot also has a light and a light sensor so that it can shine the light through the bottle at the sensor. Each of these sensors produces an integer value between 0 and 255.  You will read the integer values that would be produced by the sensors from your input file. The readings from the sensors can be used to determine the weight and color of the bottle respectively (see details below). The robot also uses image processing to determine if the bottle is broken. The result from the image processing gives a value “broken” or “usable”. 

the program also keeps track of which way the robot is facing.  The robot grasps a bottle or fragment, lifts it, then rotates to the appropriate conveyor (or the waste container) and lowers the bottle and releases it.  After releasing the bottle (or fragment) the robot rotates back (opposite direction) to the incoming conveyor belt. The physical setup of the robot and the conveyor belts is shown below.
 
