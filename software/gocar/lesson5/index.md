<br>

<div align="center">
    <h1>Lesson 5. GoCar로 카드코딩해요(4)</h1>
</div>

<br>

---

<br>


<div align="center">
    <h1>[들어가기]</h1>
</div>

<br>

GoCar에는 소리를 낼 수 있는 부저와 여러 가지 색상으로 빛을 낼 수 있는 LED가 장착되어 있습니다.<br>
이번 강의에서는 GoCar의 부저와 LED 등을 이용하여 다양한 효과를 내면서 주행하는 코딩을 해보려고 합니다.<br>
그럼 먼저 소리/라이트(Light)와 관련된 카드는 어떤 것들이 있는지 살펴보아요.



<br>


<div align="center">
    <table>
        <tr>
            <td>
                <div align="center"><b>소리 카드(총 8장)</b></div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image1.png">
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
                <div align="center"><b>라이트 카드(총 4장)</b></div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image2.png" height="400" width="250"><img src="images/image3.png" height="139" width="150"><img src="images/image4.png"height="400" width="597">
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image5.png" height="400" width="250"><img src="images/image3.png" height="139" width="150"><img src="images/image6.png"height="300" width="901">
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image7.png" height="400" width="250"><img src="images/image3.png" height="139" width="150"><img src="images/image8.png"height="300" width="901">
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image9.png" height="400" width="250"><img src="images/image3.png" height="139" width="150"><img src="images/image10.png"height="300" width="901">
                </div>
            </td>
        </tr>
    </table>
</div>
<br>

이제 주행하면서 여러가지 음을 연주하고 아름답게 빛나는 GoCar를 만나러 가볼까요?

<br>

---

<br>


<div align="center">
    <h1>[코드 생각하기]</h1>
</div>

<br>

아래 주차 실습판을 활용하여 GoCar로 후진 주차하는 코딩을 해볼거예요. 후진 주차를 하면서 소리와 라이트 카드를 사용하여 효과를 줘보아요.

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">주차 실습판</div>
            </td>
            <td>
                <div align="center"><img src="images/image11.png"><br>
                <img src="images/image12.png" height="80" width="214" a href="images/[Lesson5]GoCar_주차실습판"></div>
            </td>
        </tr>
    </table>
</div>

<br>

먼저 실습판의 “START” 위치에서 “P(Parking)” 위치까지 GoCar를 이동시키려면 어떻게 코드를 짜야 할지 생각해보아요.<br><br>
<b>※	마지막 “P(Parking)” 위치는 <font color="red">후진</font>하여 이동해야 합니다.</b><br>
여러가지 방법이 있겠지만 다음과 같이 동작한다고 가정해서 코드를 만들어보았습니다.

<br>

<br>

조건문을 사용하는 방법은 다음과 같습니다.

<br>

<div align="center">
    <table>
        <tr>
            <td>
                <b>1. 조건이 참인 경우에만 특정 명령 수행</b>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center"><img src="images/image3.png" alt="조건문 사용방법1"></div>
            </td>
        </tr>
        <tr>
            <td>
                <b>2. 조건이 참인 경우와 거짓인 경우 모두 특정 명령 수행</b>
            </td>
        </tr>
        <tr>
            <td>
                <img src="images/image4.png" alt="조건문 사용방법2">
            </td>
        </tr>
        <tr>
            <td>
                ☞	조건이 참인 경우에만 특정 명령을 수행하고 싶으면 조건 시작 카드와 조건 끝 카드 사이에 수행할 명령어 카드를 읽습니다. <br>그리고 조건이 참인 경우와 거짓인 경우 각각 다른 명령을 수행하고 싶으면 “조건이 맞지 않으면,” 카드를 사용하여 구분해줍니다. 그래서 조건 시작 카드와 조건이 맞지 않으면 카드 사이에는 참인 경우에 수행할 명령어 카드를, 조건이 맞지 않으면 카드와 조건 끝 카드 사이에는 거짓인 경우에 수행할 명령어 카드를 읽습니다. <Br>항상 마지막엔 “조건 끝” 카드를 읽어줘야 한다는 것을 잊지마세요!
            </td>
        </tr>
    </table>
</div>

<br>
조건문 사용법을 알았다면 이제 어떻게 코드를 짜야 할지 생각해볼까요?
<br>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">동작 순서</div>
            </td>
            <td>
                <div align="center">시작 → (앞쪽 장애물을 발견하면) U턴 / (조건이 맞지 않으면) 1칸 전진 → 끝</div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">카드 순서</div>
            </td>
            <td>
                <div align="center">
                <img src="images/image5.png"><br>
                <font color="red"><b>※ “카드코딩 모드” 카드는 생략</b></font>
                </div>
            </td>
        </tr>
    </table>
</div>

<br>

조건 시작 카드(앞쪽 장애물 발견하면,)와 조건이 맞지 않으면 카드 사이에 U턴 카드를 사용하여 전방에 장애물이 있으면 U턴을 하도록 하였습니다. <br>
그리고 조건이 맞지 않으면 카드와 조건 끝 카드 사이에 1칸 전진 카드를 사용하여 전방에 장애물이 없으면 1칸 전진하도록 하였습니다.

---

<br>


<div align="center">
    <h1>[코딩 및 실행하기]</h1>
</div>

<br>

<div align="center">
    <table>
        <tr>
            <td><br><div align="center"><b><h3>1단계 코딩카드 준비하기</h3><br></b></div></td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image6.png"><br>
                    카드코딩에 필요한 코딩카드들을 준비해보아요<br>
                    <font color="red"><b>※ “카드코딩 모드” 카드는 생략</b></font>
                </div>
            </td>
        </tr>
        <tr>
            <td><div align="center"><b><br><h3>2단계 코딩카드 배열하기</h3><br>
            (앞쪽 장애물을 발견하면) U턴 / (조건이 맞지 않으면) 1칸 전진<br></b></div></td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image7.png"><br>
                    동작 순서에 맞게 카드를 배열해 보아요. 코딩의 시작과 끝에는 항상 “코딩시작”과 “코딩끝” 카드가 온다는 것을 잊지 마세요
                </div>
            </td>
        </tr>
        <tr>
            <td><div align="center"><b><br><h3>3단계 코딩카드 읽기</h3><br></b></div></td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image8.png"><br>
                    GoCar의 전원을 켜고 코딩카드를 읽습니다. <br>코딩카드가 잘 읽히도록 올바른 위치에 GoCar를 올려놓고 카드 순서대로 메인 전등 부분을 1번 눌러서 카드를 읽어주세요. <br>만약, 중간에 카드를 잘못 읽었다면 처음부터(=”코딩시작” 카드부터) 다시 시작합니다.<br><Br>
                </div>
            </td>
        </tr>
        <tr>
            <td><div align="center"><b><br><h3>4단계 코딩 실행하기</h3><br></b></div></td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image9.png" height="350" width="341"><br>
                    ① 만약 전방에 장애물이 있으면<br>
                    <img src="images/image10.png"><br>
                    ② 만약 전방에 장애물이 없으면<br>
                    <img src="images/image11.png"><br>
                    GoCar를 평평한 바닥에 놓고 메인 전등 부분을 연속으로 2번 눌러서 코딩을 실행합니다. <br>약 3초 후 GoCar가 자동으로 코딩한 명령을 수행합니다. <br>GoCar가 잘 주행할 수 있도록 매끄럽고 평평한 바닥에서 실행해주세요.<br><br>
                    ① GoCar 앞에 손바닥이나 종이 등을 대서 장애물을 인식할 수 있도록 해주세요. 그 상태에서 코딩을 실행하면 GoCar가 장애물을 인식하여 U턴합니다.<br>
② GoCar 앞에 아무것도 없는 상태에서 코딩을 실행합니다. GoCar가 장애물이 없음을 인지하고 1칸 전진합니다.<br>
<font color="red"><b>※ GoCar와 장애물 사이의 거리는 <font color="blue">약 10cm 이내</font>로 해주세요.</b></font>
                </div>
            </td>
        </tr>
    </table>
</div>
<br>

GoCar의 센서를 활용하여 코딩을 해보니 더 신기하고 재미있죠? 그런데 너무 금방 끝나버렸나요?<br>

그렇다면 한 단계 응용된 코딩을 해볼까요? <br>
지난 강의에서 배운 반복문을 사용하여 장애물 유무를 계속 확인하면서 자율주행하는 코딩을 해보도록 해요. 다음과 같이 코드를 만들어서 읽고 실행합니다.

<br>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">
                    <b><br><h3>장애물 회피 자율주행 코드(무한반복, 반복문과 조건문을 함께 사용)</h3><br></b>
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image12.png"><br>
                        <div align="left">
                        위 코드를 실행하면 GoCar는 다음과 같이 동작합니다.<br>
                        실행 후 전방에 장애물이 있는지 확인하여 있으면 U턴, 없으면 1칸 전진을 반복적으로 수행합니다.<br>
                        그래서 장애물을 피해서 주행하는 자율주행을 직접 체험해볼 수 있습니다.<br><br>
                        <font color="red"><b>[꼭 알아두세요!]</b></font><br>
                        ①반복문과 조건문을 함께 사용할 경우에는 반복문 안에 조건문이 들어가 있는 구조로 코딩합니다.<br>
                        그래서 반복적으로 조건의 참과 거짓을 확인하여 결과에 맞는 동작을 수행할 수 있습니다.
                        </div>
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center"><b><br><h3>반복문과 조건문 사용 예시</h3></b><br>
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image13.png"><br>
                    <img src="images/image14.png"><br>
                        <div align="left">②	코드를 실행하면 무한 반복되므로 종료가 되지 않습니다. <br>
                        코딩을 종료하고 GoCar의 주행을 멈추기 위해서는 강제 종료를 시켜야 합니다. <br>
                        강제 종료시키는 방법은 GoCar를 손으로 잡고 들어서 뒤집으면 모터가 회전을 멈추면서 종료됩니다. <br>
                        이러한 강제 종료 방법은 주행 중인 모든 경우에 사용할 수 있습니다.
                        </div>
                </div>
            </td>
        </tr>
    </table>
</div>

<br>

---

<br>


<div align="center">
    <h1>[더 알아보기]</h1>
</div>

<br>

GoCar의 하부에는 색상을 인식할 수 있는 컬러센서가 2개 장착되어 있는데, 이 컬러센서를 이용하여 코딩카드를 읽고 코딩을 할 수 있습니다.<br> 이러한 컬러센서도 전방 장애물 감지 센서처럼 조건문을 사용한 카드코딩이 가능합니다. 다음 코드를 보고 GoCar가 어떻게 동작할지 생각해보아요.

<br>

<div align="center">
    <table>
        <tr>
            <td><div align="center"><b><br><h3>컬러센서를 활용한 카드코딩 예제</h3><br></b></div></td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image15.png"><br>
                </div>
            </td>
        </tr>
    </table>
</div>

<br>
위 코드를 실행하면 다음과 같이 동작합니다. <br>
현재 GoCar가 있는 바닥면의 색상이 무엇인지 확인하여 만약 빨간색이면 U턴 후 1칸 전진하고, 빨간색이 아니면 1칸 전진만 합니다.<br>
그리고 이 동작을 무한 반복합니다.<br>

<div align="center"><b>무한 반복하기</b></div>
<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">만약 바닥 색상이 빨간색이면 U턴 후 1칸 전진하기</div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">만약 바닥 색상이 빨간색이 아니면 1칸 전진하기</div>
            </td>
        </tr>
    </table>
</div>


<Br>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center"><b>① 만약 바닥 색상이 빨간색이면</b></div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center"><img src="images/image16.png"></div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center"><b>② 만약 바닥 색상이 빨간색이 아니면</b></div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center"><img src="images/image17.png"></div>
            </td>
        </tr>
    </table>
</div>

<br>

빨간색 외에도 녹색과 파란색 조건 카드가 기본적으로 제공됩니다. <Br>
빨간색, 녹색, 파란색이 그려진 활동판을 만들어서 길찾기, 장애물 피해서 목적지 찾아가기 등 다양한 활동을 즐길 수 있습니다.<Br>

<br>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center"><b>GoCar 활동판 예시</b></div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center"><img src="images/image18.png"></div>
            </td>
        </tr>
    </table>
</div>
---

<br>

<div align="center">
    <h1>[정리하기]</h1>
</div>

<br>

이번 강의에서는 GoCar의 센서를 활용한 코딩을 해보았습니다. <br>
GoCar의 전방에 있는 장애물 감지 센서로 장애물 유무를 확인하고 장애물을 피해서 주행할 수 있었습니다. <br>
이러한 센서 코딩이 바로 자동차 자율주행의 기초가 됩니다. <Br>
또한, 조건 카드를 사용해보면서 조건문이 무엇이고 어떻게 사용해야 하는지 배워보았습니다. <br>
센서를 활용한 코딩을 하기 위해서는 조건 카드가 꼭 필요하다는 것을 잊지 말아요!

1. 센서(Sensor)란 빛, 소리, 화학물질, 온도 등과 같이 감각과 관련된 신호들을 수집하여 이 신호들을 과학적인 방법으로 분석하고 상태를 알아내는 장치입니다.
2. GoCar는 전방 장애물 감지 센서(적외선 센서), 컬러 센서, 자세 센서 등 첨단 센서들이 장착되어 다양한 기능을 수행합니다.

3. GoCar의 전방 장애물 감지 센서를 이용하여 전방에 장애물 유무를 확인하고 장애물을 피해서 자율주행하는 코딩을 할 수 있습니다.

4. 센서를 활용한 코딩을 하기 위해서는 조건 카드를 사용합니다.

5. 반복문과 조건문을 함께 사용하면 조건의 참, 거짓을 판단하고 동작하는 것을 반복적으로 수행할 수 있습니다.

6. 카드코딩 실행 중에 GoCar를 들어서 뒤집으면 모터가 회전을 멈춰 강제 종료시킬 수 있습니다.

<br>

---

### [코딩카드로 자율주행해요](../)

 1. [GoCar와 친구해요!](../lesson1)
 2. [GoCar로 카드코딩해요(1)](../lesson2)
 3. [GoCar로 카드코딩해요(2)](../lesson3)
 4. **GoCar로 카드코딩해요(3)**
 5. [GoCar로 카드코딩해요(4)] - 6월 넷째주(~6/26) 업데이트 예정
 6. [GoCar로 라인코딩해요] - 7월 첫째주(~7/3) 업데이트 예정
 7. [GoCar로 모션코딩해요] - 7월 둘째주(~7/10) 업데이트 예정
 8. [GoCar로 따라가기해요] - 7월 셋째주(~7/17) 업데이트 예정

---

Modified : 2020.6.19