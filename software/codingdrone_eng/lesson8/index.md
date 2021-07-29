<br>

<div align="center">
    <h1>Lesson 8. Block coding with a coding drone (2)</h1>
</div>

<br>

---

<br>


<div align="center">
    <h1>[Outline]</h1>
</div>

<br>

In this lecture, we will code to control the drone by pressing the button on the remote controller. <Br>
Isn't it strange to think that the drone is controlled by pressing a button instead of using the lever on the remote controller? <br>
If you use the remote controller button event block among the blocks for coding drones, you can give movement commands for each button. <br>
Here we are going to take off and land and do basic flight (forward, reverse, move left, move right).<br>
 So shall we start?

<Br>

---

<div align="center">
    <h1>[Thinking of code]</h1>
</div>

<br>
In <b>Rokitbrick</b>, there are two types of remote controller buttons and lever-related blocks.
<br>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">
                    <h3>Remote Controller Button Event Block</h3>
                </div>
            </td>
            <td colspan="2">
                <div align="left">
                    ▶ Generates a signal when a button on the remote controller is pressed and returns a True value.
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image1.png">
                </div>
            </td>
            <td>
                <div align="center">
                    <b>button type</b>
                </div>
            </td>
            <td>
                <div align="left">
                    1. Front Left Top/Bottom Button<Br>
                    2. Front right top/bottom button<Br>
                    3. Top Left/Right Buttons<Br>
                    4. Bottom left/right button<Br>
                    5. Center Up/Down/Left/Right Buttons (=Trim Button)
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <h3>Remote Controller Joystick (Lever) Event Block</h3>
                </div>
            </td>
            <td colspan="2">
                <div align="left">
                    ▶ When the joystick (lever) of the remote controller is moved in a specific direction, it generates a signal and returns a True value.
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image2.png">
                </div>
            </td>
            <td>
                <div align="center">
                    <b>Joystick (Lever) Direction(Common left/right)</b>
                </div>
            </td>
            <td>
                <div align="left">
                    Total 9 directions: top, top left, top right, bottom, bottom left, bottom right, left, right, center
                </div>
            </td>
        </tr>
        <tr>
            <td colspan="3">
                <div align="left">
                    As follows, assemble and use the conditional block of Rocket Brick as a judgment block.<br><br>
                </div>
                <div align="center">
                    <img src="images/image3.png"><img src="images/image4.png">
                </div>
            </td>
        </tr>
    </table>
</div>

<br>

Let's code the drone to operate as follows depending on the remote controller button.

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image5.png">
                </div>
            </td>
            <td>
                <div align="center">
                    <img src="images/image6.png">
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    Take off: lower left button
                </div>
            </td>
            <td>
                <div align="center">
                    Landing: bottom right button
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image7.png">
                </div>
            </td>
            <td>
                <div align="center">
                    <img src="images/image8.png">
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    1m forward: button above center
                </div>
            </td>
            <td>
                <div align="center">
                    Reverse 1m: button below center
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image9.png">
                </div>
            </td>
            <td>
                <div align="center">
                    <img src="images/image10.png">
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    Move 1m left: Center left button
                </div>
            </td>
            <td>
                <div align="center">
                    Move 1m to the right: Center right button
                </div>
            </td>
        </tr>
    </table>
</div>

<br>

<br>

So first, think about how to create the code for each command.

<br>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">
                    Command
                </div>
            </td>
            <td>
                <div align="center">
                    code
                </div>
            </td>
            <td>
                <div align="center">
                    Explanation
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    take off
                </div>
            </td>
            <td>
                <div align="center">
                    <img src="images/image11.png">
                </div>
            </td>
            <td>
                <div align="left">
                    If you press the lower left button (=S button) on the remote controller, the drone will hover for 3 seconds after take off.
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    to land
                </div>
            </td>
            <td>
                <div align="center">
                    <img src="images/image12.png">
                </div>
            </td>
            <td>
                <div align="left">
                    If you press the bottom right button (=P button) on the remote controller, the drone will hover for 3 seconds and then land.
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    go forward 1 m
                </div>
            </td>
            <td>
                <div align="center">
                    <img src="images/image13.png">
                </div>
            </td>
            <td>
                <div align="left">
                    The button above the center of the remote controller (=trim▲button) to start the dronem Hover for 3 seconds after moving forward.
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    back 1m
                </div>
            </td>
            <td>
                <div align="center">
                    <img src="images/image14.png">
                </div>
            </td>
            <td>
                <div align="left">
                    The lower center button on the remote controller (=Trim▼button) to start the dronem Hover for 3 seconds after reversing
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    move 1m to the left
                </div>
            </td>
            <td>
                <div align="center">
                    <img src="images/image15.png">
                </div>
            </td>
            <td>
                <div align="left">
                    The button above the center of the remote controller (=trim◀button) to start the dronem Move left and hover for 3 seconds.
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    move 1m to the right
                </div>
            </td>
            <td>
                <div align="center">
                    <img src="images/image16.png">
                </div>
            </td>
            <td>
                <div align="left">
                    The button above the center of the remote controller (=trim▶button) to start the dronem Move right and hover for 3 seconds.
                </div>
            </td>
        </tr>
    </table>
</div>

<br>

Now let's combine the above codes to make one code.

<br>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">
                    code
                </div>
            </td>
            <td>
                <div align="center">
                    Explanation
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image17.png">
                </div>
            </td>
            <td>
                <div align="left">
                    Put all the code for each instruction into a repeat block and assemble it into a single code. <br>
                    Because RockitBrick is a sequential coding program, blocks are executed sequentially only once. <br>
                    Therefore, the repeat block must be used to continuously detect a button action signal from the remote controller and execute the command.
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

Let's make code by assembling blocks in <B>Rokitbrick</b>.

<br>

<div align="center">
    <img src="images/image18.png">
</div>

<br>

<h2> 2. Running</h2>

<br>

When you have created the code, click the Start button to run it.<br>
Before executing, first check the following:<Br>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center"><img src="images/image19.png"></div>
            </td>
            <td>
                <div align="left"><b>
                A while! Check it out one more time before running the drone autonomous flight code on Rokitbrick!</b><br><Br>
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

When you are ready, run the code and press the bottom left button (=S button) on the remote controller.<Br>
Do drones take off? Then, press the center up, down, left, and right buttons (=trim button) in sequence and check if the drone flies according to the command.<Br>
If it doesn't fly as expected, check which part is wrong, correct it, and try again.

<br>

---

<br>

<div align="center">
    <h1>[Organize]</h1>
</div>

In this lecture, I tried coding to control the drone by pressing the button on the remote controller. <Br>
Isn't it fun to control the drone with buttons instead of levers on the remote controller? <br>
In this way, by using the remote controller button and lever event block, you can not only fly the drone as if you were actually controlling it, but you can also make your own remote controller by coding the drone to operate differently from the actual control method.

<div align="center">
    <table>
        <tr>
            <td>
                <div align="left">
                    1) When you press a button on the remote controller or move the joystick (lever), you can use the remote controller event block to make the drone perform a specific command.<br>
                    2) There are two types of remote controller event blocks (button event block, Joystick (Lever) event block), It is used as a judgment block of the conditional block.<br>
                    3) Since the remote controller event block must continuously check whether a button or joystick (lever) operation signal has occurred, the repeat block is used together.<br>
                </div>
            </td>
        </tr>
    </table>
</div>

<br>

---

### [Coding with a coding drone (English)](../)

 1. [Make friends with Coding Drone!](../lesson1)
 2. [Let's fly a coding drone](../lesson2)
 3. [I code cards with a coding drone (1)](../lesson3)
 4. [I code cards with a coding drone (2)](../lesson4)
 5. [I code cards with a coding drone (3)] - first week of August
 6. [Motion coding with a coding drone] -first week of August
 7. [Block coding with a coding drone(1)](../lesson7)
 8. **Block coding with a coding drone (2)**


---

Modified : 2021.7.16