<br>

<div align="center">
    <h1>Lesson 4. I code cards with a coding drone (2)</h1>
</div>

<br>

---

<br>


<div align="center">
    <h1>[Outline]</h1>
</div>

<br>

In this lecture, I am going to try coding a card that makes a pattern flight with a coding drone.<br>
Pattern flight refers to flying in a certain form of route, such as triangles, squares, circles, and spirals. <br>
This pattern flight is used when drones are utilized in various industries such as filming, agriculture, and surveying. Here, we are going to do a square pattern flight.<Br><br>
And in the pattern flight, some patterns are repeated because the route is standardized. <br>
In this case, you can simplify your code by using loops when coding. <Br>
In this lesson, we will learn what looping statements are and how to use them through pattern flight.<br>

<br>

<div align="center">
    <h1>[Thinking of code]</h1>
</div>

<br>

The square pattern flight sequence repeats 1 space forward and left turn 4 times.

<div align="center"><b>repeat 4 times</b></div>
<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">① advance 1 space</div>
            </td>
            <td>
                <div align="center">② turn left</div>
            </td>
        </tr>
    </table>
</div>

<br>

So let's think about how to write the code to fly like the one above. First, let's create the code without using a loop.

<br>

<h2>1. Rectangular pattern flight (without loops)</h2>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">action sequence</div>
            </td>
            <td>
                <div align="center">Start → Takeoff → (Go forward 1 space → Turn left 90 degrees) x 4 → Landing → End</div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">card order</div>
            </td>
            <td>
                <img src="images/image1.png">
            </td>
        </tr>
    </table>
</div>

<br>

Next, let's create code using loops. First, let's figure out what a loop is.
<br>


<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">
                    <h3>easy-to-understand coding</h3>
                </div>
            </td>
            <td>
                <div align="center">
                    <H3>loop</h3>
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
                <div align="left">
                    A loop is one of the main grammars of coding and is used to repeat the same or similar commands. By using loops, it not only reduces the length of the code, making it easier to understand, but also allows for more diverse and efficient coding implementations.<Br><Br>
                    There are several types of loops, such as repeating until a specific condition is satisfied, repeating the specified number of times, and repeating infinitely.
                </div>
            </td>
        </tr>
    </table>
</div>

<br>

There are a total of 4 loops that are basically provided in card coding.

<br>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">① infinite loop</div>
            </td>
            <td>
                <div align="center">② 2 repetitions</div>
            </td>
            <td>
                <div align="center">③ 3 repetitions</div>
            </td>
            <td>
                <div align="center">④ 4 reps</div>
            </td>
        </tr>
        <tr>
            <td>
                <img src="images/image3.png" alt="무한반복">
            </td>
            <td>
                <img src="images/image4.png" alt="2회반복">
            </td>
            <td>
                <img src="images/image5.png" alt="3회반복">
            </td>
            <td>
                <img src="images/image6.png" alt="4회반복">
            </td>
        </tr>
    </table>
</div>

<br>

Here's how to use the loop:

<br>

<div align="center">
    <table>
        <tr>
            <td>
                <img src="images/image7.png" alt="4회반복">
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">☞ Repeat command is input by reading the command cards to be repeated between the repeat start card (infinite repeat, repeat 2 times, repeat 3 times, repeat 4 times) and the end of the repeat in sequence.</div>
            </td>
        </tr>
    </table>
</div>

<br>
Now, let's make a square pattern flight code using a loop. Compare how it differs from the code without the loop.
<br>

<br>

<h2>2. Flying a square pattern (using loops)</h2>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">action sequence</div>
            </td>
            <td>
                <div align="center">Start → Takeoff → (Go forward 1 space → Turn left 90 degrees) x 4 → Landing → End</div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">card order</div>
            </td>
            <td>
                <img src="images/image8.png" alt="사각형 패턴 비행(반복문 사용)">
            </td>
        </tr>
    </table>
</div>

<br>

You can see that it's a lot more simplified than the code without loops. <br>
When performing the action of repeating a specific command like this, using a loop can make the code more concise and easier. Now let's run the code.

---

<br>


<div align="center">
    <h1>[Coding and running]</h1>
</div>

<br>

<h2>1. Rectangular pattern flight (without loops)</h2>

<br>

<div align="center">
    <table>
        <tr>
            <td><br><div align="center"><b><h3>Step 1 - Prepare your coding card</h3><br></b></div></td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image9.png" alt="사각형 패턴 비행(반복문 미사용) 1단계"><br>
                    Prepare the coding cards necessary for card coding.<br>
                    <font color="red"><b>※ “Card coding mode” card omitted</b></font>
                </div>
            </td>
        </tr>
        <tr>
            <td><div align="center"><b><br><h3>Step 2 - Arrange the coding cards</h3><br>
            take off → (Go forward 1 space → Turn left 90 degrees) x Repeat 4 times→ landing</b></div></td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image10.png" alt="사각형 패턴 비행(반복문 미사용) 2단계"><br>
                    Arrange the cards in the order of action. Don't forget that there are always “Coding Start” and “End Coding” cards at the beginning and end of coding!
                </div>
            </td>
        </tr>
        <tr>
            <td><div align="center"><b><br><h3>Step 3 - read the coding card</h3><br></b></div></td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image11.png" alt="사각형 패턴 비행(반복문 미사용) 3단계"><br>
                    Put the battery in the coding drone, turn it on, and read the coding card. <br>
                    Place the coding drone in the correct position to read the coding card (make sure the guard pattern of the drone and the guard pattern of the coding card match) and press the operation button once in the order of the card to read the card. <br>
                    If you read the card incorrectly in the middle, start over from the beginning (=“Start coding” card).<br><Br>
                </div>
            </td>
        </tr>
        <tr>
            <td><div align="center"><b><br><h3>Step 4 - run the code</h3><br></b></div></td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image12.png" height="350" width="341" alt="사각형 패턴 비행(반복문 미사용) 4단계1"><img src="images/image13.png" height="500" width="550" alt="사각형 패턴 비행(반복문 미사용) 4단계2"><br>
                    Place the coding drone on a flat surface with no people or obstacles nearby. <br>
                    And press the action button twice in succession to execute the coding. <br>
                    After about 3 seconds, the coding drone automatically executes the coded command<br><br>
                    <font color="red"><b>※ After pressing the action button, immediately move away from the drone by a safe distance. (Beware of safety accidents!)</b></font>
                </div>
            </td>
        </tr>
    </table>
</div>
<br>

Next, try running the code using the loop.

<br>

<h2>2. Rectangular pattern driving (using loops)</h2>

<br>

<div align="center">
    <table>
        <tr>
            <td><div align="center"><b><br><h3>Step 1 - Prepare your coding card</h3><br></b></div></td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image14.png" alt="사각형 패턴 비행(반복문 사용) 1단계"><br>
                    Prepare the coding cards necessary for card coding.<br>
                    <font color="red"><b>※ “Card coding mode” card omitted</b></font>
                </div>
            </td>
        </tr>
        <tr>
            <td><div align="center"><b><br><h3>Step 2 - Arrange the coding cards</h3><br><br>
            take off → (Go forward 1 space → Turn left 90 degrees) x Repeat 4 times→ landing<br><br></b></div></td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image15.png" alt="사각형 패턴 비행(반복문 사용) 2단계"><br>
                    Arrange the cards in the order of action. Don't forget that there are always “Coding Start” and “End Coding” cards at the beginning and end of coding!
                </div>
            </td>
        </tr>
        <tr>
            <td><div align="center"><b><br><h3>Step 3 - read the coding card</h3><br></b></div></td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image16.png"  alt="사각형 패턴 비행(반복문 사용) 3단계"><br>
                    Put the battery in the coding drone, turn it on, and read the coding card. <Br>
                    Place the coding drone in the correct position to read the coding card (make sure the guard pattern of the drone and the guard pattern of the coding card match) and press the operation button once in the order of the card to read the card. <br>
                    If you read the card incorrectly in the middle, start over from the beginning (=“Start coding” card).<br><br>
                </div>
            </td>
        </tr>
        <tr>
            <td><div align="center"><b><br><h3>Step 4 - run the code기</h3><br></b></div></td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image12.png" height="350" width="341" alt="사각형 패턴 비행(반복문 사용) 4단계1"><img src="images/image13.png" height="500" width="550" alt="사각형 패턴 비행(반복문 사용) 4단계2"><br>
                    Place the coding drone on a flat surface with no people or obstacles nearby. <br>
                    And press the action button twice in succession to execute the coding. After about 3 seconds, the coding drone automatically executes the coded command.<br><br>
                    <font color="red"><b>※ After pressing the action button, immediately move away from the drone by a safe distance. (Beware of safety accidents!)</b></font>
                </div>
            </td>
        </tr>
    </table>
</div>

---

<br>

<div align="center">
    <h1>[Organize]</h1>
</div>

<br>

In this lecture, I tried to fly a square pattern by coding a card with a coding drone. <br>
And I also learned that the same repeating pattern can be coded more easily by using a loop. <Br>
Now, think about how to code other patterns besides squares, and try coding the cards and flying them.

<div align="center">
    <table>
        <tr>
            <td>
                <div align="left">
                    1) Pattern flight refers to flying in a certain form of route, such as triangles, squares, circles, and spirals.<br>
                    2) Because pattern flight has a standardized route, there are cases where some patterns are repeated, in which case you can use a repeating card.<br>
                    3) Using loops in coding can make your code more concise, making it easier to code.<br>
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
 4. **I code cards with a coding drone (2)**
 5. [I code cards with a coding drone (3)] - first week of August
 6. [Motion coding with a coding drone] -first week of August
 7. [Block coding with a coding drone(1)](../lesson7)
 8. [Block coding with a coding drone(2)](../lesson8)

---

Modified : 2021.7.30