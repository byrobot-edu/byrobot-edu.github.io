<br>

<div align="center">
    <h1>Lesson 7. Block coding with a coding drone (1)</h1>
</div>

<br>

---

<br>


<div align="center">
    <h1>[Outline]</h1>
</div>

<br>

Coding drone supports not only unplugged coding but also plugged coding function. <Br>
Currently available pluggable coding programs are <b>“Rockitbrick”</b> and <b>“Python”</b>. <br>
In this lecture, we are going to learn how to connect and code a coding drone and a rocket brick.<br>

<div align="center">
    <table>
        <tr>
            <td><div align="left"><h3>What is Plugged Coding?</h3> </div></td>
        </tr>
        <tr>
            <td>
                <div align="left">Plugged means that an electric plug is plugged in.<Br>
                 Plugged coding refers to coding activities using electronic products such as computers and mobile devices. <Br>
                 One example of pluggable coding is block coding, which is a coding learning activity using an educational programming language (EPL). <Br>
                 You can create a program by arranging block-shaped commands in order by using a computer, tablet, etc. Representative educational programming languages include <b>Rockitbrick</b>, Entry, and Scratch. </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image1.png"><img src="images/image2.png">
                </div>
            </td>
        </tr>
    </table>
</div>

<br>

---

<br>


<div align="center">
    <h1>[Connect]</h1>
</div>

<br>

<h2> 1. Connecting the Coding Drone to Rockitbrick</h2>
<br>

Connect the coding drone to the <B>Rockitbrick</b> as follows.

1) What you need: PC, USB cable, coding drone, remote controller

2) Install the battery in the coding drone.

3) Connect the remote controller to the PC using a USB cable.

<font color="red"><b>※ The drone and remote controller must be paired.</b></font><br>
<br>
<div align="center">
    <img src="images/image3.png">
    <br>
</div><br>
4) Download Program<br>
☞ [Rokitbrick Download Windows Version](https://byrobot.co.kr/bbs/download.php?bo_table=download&wr_id=11&no=0)<br>
☞ [Rokitbrick Download MAC OS Version](https://byrobot.co.kr/bbs/download.php?bo_table=download&wr_id=11&no=1)
<br><Br>
5) Run Rockitbrick and click [SELECT]
<div align="center">
    <img src="images/image11.png">
    <br>
</div>
6) [BRC-105] Click.<br>
<div align="center">
    <img src="images/image8.png">
    <br>
</div>
7) Click [Connect to Drone] and click the corresponding port to connect to the drone.
<div align="center">
    <img src="images/image9.png">
    <br>
</div>
8) [Connection successful] If a message appears, the connection is normal.
<div align="center">
    <img src="images/image10.png">
    <br>
</div>
<br>

---

<br>


<div align="center">
    <h1>[Note]</h1>
</div>

<br>

<h2>1. Rockitbrick Block for Coding Drone</h2><br>
<h4>1) Drone sensor block</h4>
<div>
    <table>
        <tr>
            <td>
                <div>
                    <img src="images/image31.png"><br>
                </div>
            </td>
            <td>
                - You can check the real-time measurement values of various sensors of the coding drone and use it as a variable block.<br>
            </td>
        </tr>
    </table>
</div>
<h4>2) Remote Controller Button/Joystick (Lever) Judgment Block</h4>
<div>
    <table>
        <tr>
            <td>
                <div>
                    <img src="images/image32.png"><br>
                </div>
            </td>
            <td>
                - This is a block that determines the operation of the buttons and joystick (lever) of the remote controller and is used as a conditional in the conditional block. <br>
                - 	You can generate a remote controller motion signal to perform a specific command.<br>
            </td>
        </tr>
    </table>
</div>
<h4>3) drone flying block</h4>
<div>
    <table>
        <tr>
            <td>
                <div>
                    <img src="images/image33.png"><br>
                </div>
            </td>
            <td>
                - You can set the drone mode.<br>
                - Drones can take off/land and fly.<br>
            </td>
        </tr>
    </table>
</div>
<h4>4) Drone/Remote Controller LED Block</h4>
<div>
    <table>
        <tr>
            <td>
                <div>
                    <img src="images/image34.png"><br>
                </div>
            </td>
            <td>
                - You can decorate the drone's LED in various colors.<br>
            </td>
        </tr>
    </table>
</div>
<h4>5) Drone/Remote Controller Buzzer Block</h4>
<div>
    <table>
        <tr>
            <td>
                <div>
                    <img src="images/image35.png"><br>
                </div>
            </td>
            <td>
                - You can play the scale with the buzzer sound of the drone/controller.<br>
            </td>
        </tr>
    </table>
</div>
<h4>6) Remote Controller Vibration Block</h4>
<div>
    <table>
        <tr>
            <td>
                <div>
                    <img src="images/image36.png"><br>
                </div>
            </td>
            <td>
                - You can turn the vibration of the remote controller on/off.<br>
            </td>
        </tr>
    </table>
</div>
<br>
<h2> 2. Precautions for use</h2>

1) lease use the drone with a fully charged battery, and if the battery level is less than 50%, flight performance may be affected.

2) Depending on the battery level and the condition of parts such as motors and propellers (motor performance, whether the propeller is defective, etc.), good or bad flight conditions may occur.

3) Drones and remote controllers always have the latest firmware installed.

4) The drone may malfunction due to program errors, so use it in a wide space as much as possible, and check that there are no people or obstacles around.

<br>

<h2> 3. How to Force Stop the Drone</h2>
<br>
<font color="red"><b>※ If an error occurs while using the coding drone in Rockitbrick or the drone does not fly in the desired direction, the drone must be stopped by force.</b></font><br>

☞ If you click Force Stop on the running <B>Rockitbrick</b> screen with the mouse to end the execution, the drone will land directly from the current location.

☞ It is used to make and use a landing code so that it can land in an emergency on the <b>Rockitbrick</b> code. Make the drone land when a specific key on the keyboard is pressed. The code below is an example

<div>
    <table>
        <tr>
            <td>
                <div>
                    <img src="images/image37.png"><br>
                </div>
            </td>
            <td>
                - Press the space key to land the drone. “Flying motion state” is a block made to be used during coding by coding various motions of the coding drone.<br>
                <div align="center">
                <table>
                    <tr>
                        <td>
                            <div align="center">
                                flight mode
                            </div>
                        </td>
                        <td>
                            <div align="center">
                                code
                            </div>
                        </td>
                    </tr>
                    <tr>
                        <td>
                            <div align="center">
                                Ready
                            </div>
                        </td>
                        <td>
                            <div align="center">
                                READY
                            </div>
                        </td>
                    </tr>
                    <tr>
                        <td>
                            <div align="center">
                                Start
                            </div>
                        </td>
                        <td>
                            <div align="center">
                                START
                            </div>
                        </td>
                    </tr>
                    <tr>
                        <td>
                            <div align="center">
                                Take off
                            </div>
                        </td>
                        <td>
                            <div align="center">
                                TAKE OFF
                            </div>
                        </td>
                    </tr>
                    <tr>
                        <td>
                            <div align="center">
                                Flight
                            </div>
                        </td>
                        <td>
                            <div align="center">
                                FLIGHT
                            </div>
                        </td>
                    </tr>
                    <tr>
                        <td>
                            <div align="center">
                                Landing
                            </div>
                        </td>
                        <td>
                            <div align="center">
                                LANDING
                            </div>
                        </td>
                    </tr>
                    <tr>
                        <td>
                            <div align="center">
                                Stop
                            </div>
                        </td>
                        <td>
                            <div align="center">
                                STOP
                            </div>
                        </td>
                    </tr>
                </table>
                </div>
            </td>
        </tr>
    </table>
</div>

---

<br>


<div align="center">
    <h1>[Thinking of code]</h1>
</div>

If you succeed in connecting the coding drone to the rocket brick, shall we try a simple flight with block coding?<br>
Let's try flying forward and then landing.<br>

<br>

<div align="center">
    <table>
        <tr>
            <td rowspan="2">
                <div align="center"><img src="images/image38.png"></div>
            </td>
            <td>
                <div align="center">
                action sequence
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="left">
                ① The drone takes off.<Br>
                ② Drone 1m Hover after moving forward.<br>
                ③ The drone lands.<br>
                </div>
            </td>
        </tr>
    </table>
</div>
<Br>
<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">block</div>
            </td>
            <td colspan="2">
                <div align="center">
                Explanation
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center"><img src="images/image39.png"></div>
            </td>
            <td colspan="2">
                <div align="left">The drone takes off. constant altitude (approx. 1m) And then it will hover.</div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center"><img src="images/image40.png"></div>
            </td>
            <td colspan="2">
                <div align="left">The drone lands while in flight. <br>
                Wait for the motor to come to a complete stop after landing. <Br>
                Do not use the landing command when the drone is too high or too low. <br>
                (1m The height is appropriate.)</div>
            </td>
        </tr>
        <tr>
            <td rowspan="4">
                <div align="center"><img src="images/image41.png"></div>
            </td>
            <td colspan="2">
                <div align="left">The drone will fly by default according to the settings of the following options.<br>
                <font color="red"><b>※ Basic flight: Advance, junior, move left, move right, Increase, descent</b></font>
                </div>
            </td>
        </tr>
        <Tr>
            <td>
                <div align="center">option One</div>
            </td>
            <td>
                <div align="left">Sets the default flight direction.<Br>
                ① forward = move forward<br>
                ② backward = move backward<Br>
                ③ Left = move left<br>
                ④ Right = move right<Br>
                ⑤ up = move up<Br>
                ⑥ down = move down
                </div>
            </td>
        </tr>
        <Tr>
            <td>
                <div align="center">option 2</div>
            </td>
            <td>
                <div align="left">Set the movement speed.<Br>
                (unit: m/s, decimal point available)</div>
            </td>
        </tr>
        <Tr>
            <td>
                <div align="center">option 3</div>
            </td>
            <td>
                <div align="left">Set the flight distance.<Br>
                Street = speed x time ex) 1m/s * 1sec = 1m<br>
                (unit: seconds,decimal point available)
                </div>
            </td>
        </tr>
    </table>
</div>

<br>

Now, how to write code using the above blocks Think about what it will be I thought of the code like this:

<br>

<div align="center">
    <table>
        <tr>
            <td colspan="2">
                <div align="center">code</div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="left">
                action sequence
                </div>
            </td>
            <td>
                <div align="left">
                Takeoff → Wait 5 seconds (= hovering) → Move forward 1m → Landing
                </div>
            </td>
        </tr>
        <tr>
            <td colspan="2">
                <div align="center"><img src="images/image42.png">
                </div>
            </td>
        </tr>
    </table>
</div>

<br>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center"><img src="images/image43.png"></div>
            </td>
            <td>
                <div align="left">
                Use the wait command between takeoff and move commands to give the drone time to position and maintain a stable posture after moving.
                </div>
            </td>
        </tr>
    </table>
</div>

<br>

---

<br>


<div align="center">
    <h1>[Coding and running]</h1>
</div>

<br>

<h2> 1. Coding</h2>

<br>
Let's make code by assembling blocks in <b>Rockitbrick</b>.
<br>

<div align="center"><img src="images/image44.png"></div>

<br>

<h2> 2. Running</h2>

<br>

When you have created all the code, press the space bar to run it.<br>
Before executing, first check the following:<br>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center"><img src="images/image45.png"></div>
            </td>
            <td>
                <div align="left"><b>
                a while! Check it out one more time before running the drone autonomous flight code on Rockitbrick!</b><br><Br>
                1) Secure a safe distance (2m or more) from the drone.<Br>
                2) Make sure there are no people or obstacles around the drone.<br>
                ☞ Make sure that there are no people or obstacles in the path by predicting the direction and distance of the drone's movement in the code.<Br>
                3) Check how to forcefully stop the drone in case of a malfunction of the drone or a rocket brick error.
                </div>
            </td>
        </tr>
    </table>
</div>

<Br>

So, if you're ready, let's run it. <br>
Do the drones fly in the order of movement? <br>
If it doesn't fly as expected, check which part is wrong, correct it, and try again

<Br>

---

<br>

<div align="center">
    <h1>[Organize]</h1>
</div>

<br>

In this lecture, I learned about plug coding, a new coding function of the coding drone, and also tried block coding myself using Entry. <Br>
In Rockitbrick, you can do more diverse and higher-level coding than card coding. <br>
Let's immerse ourselves in the fun of autonomous flight by coding using various blocks of the coding drone!

<div align="center">
    <table>
        <tr>
            <td>
                <div align="left">
                    1) Plugged means that an electric plug is plugged in. Plugged coding refers to coding activities using electronic products such as computers and mobile devices.<br>
                    2) Block coding is a coding learning activity using an Educational Programming Language (EPL) as an example of Plugged Coding. <br>
                    ☞ Educational programming languages: Rockitbrick, Entry, Scratch, etc<Br>
                    3)Coding drone and rocket brick connection method is PC and the controller USB After connecting with a cable, run Rockit Brick to connect the coding drone and hardware.<br>
                    4)The <b>Rockitbrick</b> block for the coding drone is a sensor, flight, LED, It is composed of various categories such as buzzer.<br>
                    5)If an error occurs while using the coding drone in <b>Rockitbrick</b> or the drone does not fly in the desired direction, the drone must be stopped forcibly. The method is as follows.<br>
                    (1)	(1)	If you click Force Stop on the running <b>Rockitbrick</b> screen with the mouse to end the execution, the drone will land directly from the current location.<br>
                    (2)	(2)	It is used to make and use a landing code so that it can land in an emergency on the <b>Rockitbrick</b> code.<Br>
                    6)Before execute the autonomous flight with a coding drone in <b>Rockitbrick</b>, check the safety rules first.
                </div>
            </td>
        </tr>
    </table>
</div>

<Br>

---

### [Coding with a coding drone (English)](../)

 1. [Make friends with Coding Drone!](../lesson1)
 2. [Let's fly a coding drone](../lesson2)
 3. [I code cards with a coding drone (1)] - fifth week of July
 4. [I code cards with a coding drone (2)] - fifth week of July
 5. [I code cards with a coding drone (3)] - first week of August
 6. [Motion coding with a coding drone] -first week of August
 7. **Block coding with a coding drone(1)**
 8. [Block coding with a coding drone (2)](../lesson8)


---

Modified : 2021.7.16