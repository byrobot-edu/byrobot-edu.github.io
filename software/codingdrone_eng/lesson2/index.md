<br>

<div align="center">
    <h1>Lesson 2. Let's fly a coding drone</h1>
</div>

<br>

---

<br>


<div align="center">
    <h1>[Outline]</h1>
</div>

<br>

In this lecture, you will learn how to control a coding drone and fly it yourself.<br>
Before learning how to fly, let's learn how a drone flies and the principles of flight.<br>
How do drones fly forward, backward, left and right, and take off and land? To understand the flying principle of a drone, you must first understand how the drone's propeller is constructed. <br>
Let's find out by looking at the following picture.



<br>
<div align="center">
<img src="images/image19.png">
</div>
<br>

Next, let's learn about the flying principle of how a drone can fly forward, backward, and rotate.<Br>
How drones fly <font color="red"><b> By adjusting the speed of each motor, the rotation speed of the propeller is different.</b></font> It is easy to understand if you know the facts

<Br>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center"><img src="images/image20.png"></div>
            </td>
            <td>
                <div align="center"><img src="images/image21.png"></div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="left">All propellers rotate rapidly at the same speed to generate a large lift, and when the lift is greater than gravity, it rises. When taking off, take off in the same way.</div>
            </td>
            <td>
                <div align="left">lowly rotate all propellers at the same speed to reduce lift, and when lift is less than gravity, you will descend. When you land, you land in the same way.</div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center"><img src="images/image22.png"></div>
            </td>
            <td>
                <div align="center"><img src="images/image23.png"></div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="left">If propellers 3 and 4 are rotated fast and propellers 1 and 2 are relatively slow, the rear lift of the drone will increase and it will be lifted up and tilted forward. At this time, the thrust is generated forward and it moves forward.</div>
            </td>
            <td>
                <div align="left">If propellers 1 and 2 are rotated fast and propellers 3 and 4 are relatively slow, the front lift of the drone will increase, so it will lift upwards and tilt backwards. At this time, thrust is generated backwards and the vehicle moves backward.</div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center"><img src="images/image24.png"></div>
            </td>
            <td>
                <div align="center"><img src="images/image25.png"></div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="left">If propellers 2 and 3 are rotated quickly, and propellers 1 and 4 are relatively slow, the right lift of the drone will increase and it will tilt to the left while lifting upwards. At this time, momentum is generated to the left and it moves to the left.</div>
            </td>
            <td>
                <div align="left">If propellers 1 and 4 are rotated quickly and propellers 2 and 3 are relatively slow, the left lift of the drone will increase and it will be lifted up and tilted to the right. At this time, momentum is generated to the right and it moves to the right.</div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center"><img src="images/image26.png"></div>
            </td>
            <td>
                <div align="center"><img src="images/image27.png"></div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="left">If propellers 1 and 3 are rotated fast and propellers 2 and 4 are relatively slow, the torque of 1 and 3 (the propeller rotates clockwise) will be greater than 2 and 4, causing the drone to rotate counterclockwise (left). It's possible.</div>
            </td>
            <td>
                <div align="left">If propellers 2 and 4 are rotated quickly and propellers 1 and 3 are relatively slow, the torque of 2 and 4 (the propeller rotates counterclockwise) becomes greater than 1 and 3, causing the drone to rotate clockwise (right). It's possible.</div>
            </td>
        </tr>
    </table>
</div>

<br>

<div align="center"><B>glossary</b></div>
<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">lift</div>
            </td>
            <td>
                <div align="center">It is the force that allows an aircraft to float in the air.</div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">torque</div>
            </td>
            <td>
                <div align="center">As a force to rotate, the aircraft tends to rotate in the opposite direction to the direction in which the propeller rotates.</div>
            </td>
        </tr>
    </table>
</div>

<br>

So far, we have discussed the flying principle of how a drone can fly in a fixed direction.<br>
Now, shall we learn how to fly a coding drone?<br>

<br>

---

<br>


<div align="center">
    <h1>[Note]</h1>
</div>

<br>

Learn how to control a coding drone. There are 4 control modes of the drone, but the basic control mode of the coding drone is mode 2.

<br>

<div align="center">
    <table>
        <tr>
            <td colspan="4">
                <div align="center"><h3>drone control mode</h3></div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center"><img src="images/image28.png"></div>
            </td>
            <td>
                <div align="center"><img src="images/image29.png"></div>
            </td>
            <td>
                <div align="center"><img src="images/image30.png"></div>
            </td>
            <td>
                <div align="center"><img src="images/image31.png"></div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">mode 1</div>
            </td>
            <td>
                <div align="center">mode 2</div>
            </td>
            <td>
                <div align="center">mode 3</div>
            </td>
            <td>
                <div align="center">mode 4</div>
            </td>
        </tr>
    </table>
</div>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center"><h3>Terms</h3></div>
            </td>
            <td>
                <div align="center"><h3>flight action</h3></div>
            </td>
            <td>
                <div align="center"><h3>Contents</h3></div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">PITCH</div>
            </td>
            <td>
                <div align="center">forward/backward</div>
            </td>
            <td>
                <div align="left">Drone moving forward/backward<br>
(= motion of the drone tilting forward/backward)
</div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">ROLL</div>
            </td>
            <td>
                <div align="center">move left/right</div>
            </td>
            <td>
                <div align="left">Drone movement left/right<br>
(= motion of the drone tilting left/right)
</div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">THROTTLE</div>
            </td>
            <td>
                <div align="center">Rise and fall</div>
            </td>
            <td>
                <div align="left">Drone ascending/descending motion
</div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">YAW</div>
            </td>
            <td>
                <div align="center">turn left/right</div>
            </td>
            <td>
                <div align="left">Drone rotation left/right<br>
(= The motion of the drone rotating left/right based on the vertical axis)
</div>
            </td>
        </tr>
    </table>
</div>

<br>

So, let's learn how to take off and land first.<br>
There are two methods for taking off and landing of the coding drone. Automatic take-off and landing and manual take-off and landing.
<br>

<h2>1. Automatic take-off and landing</h2>

<div align="center">
    <table>
        <tr>
            <td rowspan="2">
                <div align="center"><h3>take-off</h3></div>
            </td>
            <td>
                <div align="center"><img src="images/image32.png"></div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="left">When the drone has landed, press the auto takeoff and landing button on the remote controller (L1 button in front of the left lever) for more than 3 seconds to take off the drone. Because the automatic altitude hold function works, it ascends to a certain height and then flies in place.</div>
            </td>
        </tr>
        <tr>
            <td rowspan="2">
                <div align="center"><h3>landing</h3></div>
            </td>
            <td>
                <div align="center"><img src="images/image33.png"></div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="left">When the drone is in flight, press and hold the Auto Takeoff and Landing button (L1 button in front of the left lever) on the remote controller for more than 3 seconds to slowly descend from the spot and land.</div>
            </td>
        </tr>
    </table>
</div>

<br>

<h2>2. Manual takeoff and landing</h2>

<br>

<div align="center">
    <table>
        <tr>
            <td rowspan="2">
                <div align="center"><h3>boot</h3></div>
            </td>
            <td>
                <div align="center"><img src="images/image34.png"></div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="left">As shown in the figure above, if both levers of the remote controller are moved in a diagonal direction (left → lower right/right → lower left or left → lower left/right → lower right) for about 2 seconds, the motor starts and all propellers of the drone rotate. do. Then return the lever back to the neutral position. The drone does not take off just by starting the motor.<br>
                <font color="red"><b>※ If you move the lever of the remote controller in the same way while the motor is running, the motor turns off and all propellers stop rotating.<br>
                ※ Starting and stopping the motor can only be operated when the drone has landed.
</b></font>
                </div>
            </td>
        </tr>
        <tr>
            <td rowspan="2">
                <div align="center"><h3>take-off</h3></div>
            </td>
            <td>
                <div align="center"><img src="images/image35.png"></div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="left">Slowly raise the left lever on the remote controller to take off the drone. While watching the drone move, slowly raise the lever little by little, and when the drone takes off to the desired height, return the lever to the neutral position. At this time, be careful as if you raise the lever too quickly or too much, the drone will suddenly take off.</div>
            </td>
        </tr>
        <tr>
            <td rowspan="2">
                <div align="center"><h3>landing</h3></div>
            </td>
            <td>
                <div align="center"><img src="images/image36.png"></div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="left">While the drone is in flight, slowly lower the left lever on the remote controller to start descending. If you lower the lever to the lowest position after the drone touches the ground, all motors stop and land.</div>
            </td>
        </tr>
    </table>
</div>

<br>

coding drone <font color="blue"><b>emergency stop</b></font> There is a function! The emergency stop function is a function that can prevent safety accidents by stopping the motor of the drone when an emergency situation occurs.

<Br>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center"><img src="images/image37.jpeg"></div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="left">While pushing down the left lever of the remote controller (①), press the L1 button in front of the left lever (②) to stop the drone's motor.<font color="red"><b>All motors are stopped, so if the drone is in the air, it will fall to the floor, so be careful., </b></font> It is used in an emergency where all motors need to be stopped urgently. To use it to land, wait until the drone hits the ground and press the L1 button.</div>
            </td>
        </tr>
    </table>
</div>

<br>

<h2>3. Basic controls</h2>

<br>

Next, let's learn the basics of flying a coding drone.

<br>

<div align="center">
    <table>
        <tr>
            <td rowspan="2">
                <div align="center"><h3>Increase / descent
</h3></div>
            </td>
            <td>
                <div align="center"><img src="images/image38.png"></div>
            </td>
            <td rowspan="2">
                <div align="center"><h3>Advance / junior</h3></div>
            </td>
            <td>
                <div align="center"><img src="images/image39.png"></div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="ledt">①	Raise: Raise the left lever upwards to raise the drone.<br>
                ② Descending: When the left lever is pushed down, the drone descends.<br>
<font color="red"><b>※ Ascent/descent is steered with the same lever and direction as takeoff/landing.</b></font>
</div>
            </td>
            <td>
                <div align="ledt">①	Forward: Move the right lever upwards to move the drone forward.<br>
                ② Reverse: Move the right lever down to move the drone backwards.
</div>
            </td>
        </tr>
        <tr>
            <td rowspan="2">
                <div align="center"><h3>turn left / turn right</h3></div>
            </td>
            <td>
                <div align="center"><img src="images/image40.png"></div>
            </td>
            <td rowspan="2">
                <div align="center"><h3>move left / move right</h3></div>
            </td>
            <td>
                <div align="center"><img src="images/image41.png"></div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="ledt">①	Rotate Left: Move the left lever to the left to rotate the drone to the left.<br>
                ② Rotate Right: Move the left lever to the right to rotate the drone right.
</div>
            </td>
            <td>
                <div align="ledt">①	Move Left: Move the right lever to the left to move the drone to the left.<br>
                ② Move Right: Move the right lever to the right to move the drone to the right.
</div>
            </td>
        </tr>
    </table>
</div>

---

<br>


<div align="center">
    <h1>[Fly]</h1>
</div>

<br>

Now that you've learned how to fly, let's fly the coding drone. Please check the following before flying.
<br>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center"><img src="images/image42.png"></div>
            </td>
            <td>
                <div align="center"><img src="images/image43.jpeg"></div>
            </td>
            <td>
                <div align="center"><img src="images/image44.png"></div>
            </td>
            <td>
                <div align="center"><img src="images/image45.jpeg"></div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="left">Use a battery that has been fully charged using a dedicated charger.</div>
            </td>
            <td>
                <div align="left">Connect the battery to the drone.<br>
<font color="red"><b>※ The remote controller is powered off</b></font>
</div>
            </td>
            <td>
                <div align="left">Secure a safe distance of about 2m from the drone, and check that there are no people or obstacles around.</div>
            </td>
            <td>
                <div align="left">Press and hold the power button on the remote controller for more than 3 seconds to turn on the power. If you hear a buzzer sound from the remote controller and the LED of the drone lights up, pairing is normal.</div>
            </td>
        </tr>
    </table>
</div>

<br>

If there is no problem by checking everything, try flying the coding drone while remembering the control method you learned earlier.

<Br>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center"><img src="images/image46.png"></div>
            </td>
        </tr>
    </table>
</div>

<Br>

---

<br>


<div align="center">
    <h1>[Organize]</h1>
</div>

<br>

Was it fun to fly the coding drone yourself? <br>
Flying the drone can be difficult at first, but with a little practice you will be able to fly it easily. <Br>
And while controlling the coding drone, you can change the speed or change the color of the main LED.<br>
Please read the manual carefully and follow it.

<div align="center">
        <table>
        <tr>
            <td>
                <div align="left">
                    1) The drone's propellers are divided into two types (clockwise rotation / counterclockwise rotation), and are assembled alternately one by one.<br>
                    2) The flying principle of a drone is Move the drone in the desired direction by varying the rotation speed of each propeller.<br>
                    3) The control mode of the drone is from Mode 1 to Mode 4, and the basic control mode of the coding drone is Mode 2.<br>
                    4) There are two types of takeoff and landing methods for coding drones: automatic and manual.<br>
                    5) In the event of an emergency during flight, all motors of the coding drone can be stopped immediately using the emergency stop function.<br>
                    6) Before controlling the drone, first check the battery and pairing status, secure a safe distance, and nearby obstacles.<br>
                </div>
            </td>
        </tr>
    </table>
</div>

<br>

---

### [Coding with a coding drone (English)](../)

 1. [Make friends with Coding Drone!](../lesson1)
 2. **Let's fly a coding drone**
 3. [I code cards with a coding drone (1)] - fifth week of July
 4. [I code cards with a coding drone (2)] - fifth week of July
 5. [I code cards with a coding drone (3)] - first week of August
 6. [Motion coding with a coding drone] -first week of August
 7. [Block coding with a coding drone(1)](../lesson7)
 8. [Block coding with a coding drone(2)](../lesson8)

---

Modified : 2021.7.23