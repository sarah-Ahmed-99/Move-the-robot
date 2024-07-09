# Move-the-robot
Here are the steps to control servo motors to produce a walking motion for a robot:
## 1. Define the motion variables:
   - STEP_ANGLE: The angle of motion per step (e.g., 20 degrees)
   - DELAY_TIME: The delay time between steps (e.g., 100 milliseconds)
## 2. Define the servo control functions:
   - moveLeft(servo1, servo2, angle): Move the robot's left and right servos to create a left step
   - moveRight(servo1, servo2, angle): Move the robot's left and right servos to create a right step
   - stopMotors(servo1, servo2): Stop the robot's motors
## 3. Define the walkRobot(servo1, servo2) function:
   - Move the robot's left leg by calling moveLeft(servo1, servo2, STEP_ANGLE)
   - Delay for DELAY_TIME milliseconds
   - Stop the motors by calling stopMotors(servo1, servo2)
   - Delay for DELAY_TIME milliseconds
   - Move the robot's right leg by calling moveRight(servo1, servo2, STEP_ANGLE)
   - Delay for DELAY_TIME milliseconds
   - Stop the motors by calling stopMotors(servo1, servo2)
   - Delay for DELAY_TIME milliseconds
##  4. Create the servo1 and servo2 objects to represent the servo motors and attach them.
## 5. Execute the walking motion in an infinite loop by calling the walkRobot(servo1, servo2) function.
