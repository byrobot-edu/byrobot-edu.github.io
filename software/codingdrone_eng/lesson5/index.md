<br>

<div align="center">
    <h1>Lesson 5. 코딩드론으로 카드코딩해요(3)</h1>
</div>

<br>

---

<br>


<div align="center">
    <h1>[들어가기]</h1>
</div>

<br>

드론에는 여러 가지 센서들이 장착되어 있습니다. 이러한 센서들이 정보들을 수집하여 드론에게 알려주면, 드론은 상황에 맞게 동작하게 됩니다. <br>
코딩드론에도 전방 장애물 감지 센서(적외선 센서), 컬러 센서, 자세 센서, 기압 센서, 옵티컬 플로우 센서 등 첨단 센서들이 장착되어 다양한 기능들을 수행합니다.<br>

<Br>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="left">센서(Sensor)란?</div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="left">▶	센서(Sensor)란 무언가를 느끼고, 그 감각으로부터 무언가를 알아내는 것을 의미합니다. <font color="red"><b>빛, 소리, 화학물질, 온도 등과 같이 감각과 관련된 신호들을 수집하여 이 신호들을 과학적인 방법으로 분석하고 상태를 알아내는 장치</b></font>를 통틀어서 센서라고 합니다.<br><br>

▶	센서는 우리 일상생활 속에서 다양하게 사용되고 있습니다. 예를 들어, 사람이 자동문 앞에 서면 센서가 이를 알아내어 문이 열리도록 신호를 보냅니다. 그리고 갑자기 불이 나면 센서가 이를 알아내어 소화 장치가 작동하도록 신호를 보내는 것 모두 센서가 사용되는 경우입니다.<Br><br>

▶	코딩드론에 사용되는 센서들은 장애물 감지(적외선) 센서, 컬러 센서, 자세 센서(가속도, 자이로스코프) 등이 있습니다.<br><br>
①	장애물 감지(적외선) 센서 : 적외선을 이용하여 센서와 장애물까지의 거리를 측정할 수 있고, 장애물을 감지하면서 주행하는 자율비행이 가능합니다.<br>
②	컬러 센서 : 코딩카드의 색상을 인식하여 카드코딩을 할 수 있고, 검은색 또는 흰색 라인을 따라 주행할 수 있습니다.<Br>
③	자세 센서 : 코딩드론이 수평을 유지하며 비행할 수 있고, 코딩드론의 기울임에 따라 명령을 줄 수 있는 모션코딩이 가능합니다.<br>

</div>
            </td>
        </tr>
        <tr>
            <td>여러가지 센서
            </td>
        </tr>
        <tr>
            <td><img src="images/image1.png" alt="여러가지센서">
            </td>
        </tr>
    </table>
</div>
<br>

이번 강의에서는 코딩드론의 다양한 센서 중에서 전방 장애물 감지 센서(적외선 센서)를 이용하여 카드코딩으로 장애물 회피 비행을 해보려고 합니다. <br>
센서를 활용한 코딩은 조건문이란 명령을 사용해야 하는데, 특정 조건에서 어떻게 동작하라는 명령을 줄 수 있습니다. <Br>
코딩카드가 많이 사용되어 어렵게 느껴질 수 있지만, 차근차근 따라해보면 쉽게 해낼 수 있을거예요. 그럼 시작해볼까요?


<br>


---

<br>


<div align="center">
    <h1>[코드 생각하기]</h1>
</div>

<br>

코딩드론은 다음과 같이 동작합니다. <br>
전방에 장애물 유무를 확인하여 장애물이 없을 경우에는 계속 전진 비행하고, 장애물이 있을 경우에는 비행을 멈추고 U턴 후 착륙합니다.

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">① 만약 전방에 장애물이 있으면 비행을 멈추고 U턴 후 착륙하기</div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">② 만약 전방에 장애물이 없으면 계속 전진 비행하기</div>
            </td>
        </tr>
    </table>
</div>

<br>

위와 같이 동작하는 코드를 만들기 위해서는 장애물 유무에 따라 서로 다른 명령을 주는 조건문을 사용해야해요. 그럼 먼저 조건문이 무엇인지 알아볼까요?
<br>


<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">
                    알기 쉬운 코딩
                </div>
            </td>
            <td>
                <div align="center">
                    조건문
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
                    조건문이란 코딩의 주요 문법 중 하나로서 특정 조건을 주고 그 조건에 따라 서로 다른 명령을 수행해야할 때 사용합니다. <br>
                    우리가 흔히 “만약 ~라면, ~하겠다”란 말을 자주 사용하는데, 바로 이러한 상황을 코딩으로 표현한 것이라고 보면 됩니다.<br><Br>
                    주어진 조건이 참인지 거짓인지 판단하여 참이면 명령A를 거짓이면 명령B를 수행할 수 있게 할 수 있습니다.<Br> 또한, 참과 거짓 2가지 경우로만 구분하지 않고 여러가지 경우에 따라 서로 다른 명령을 줄 수도 있습니다.
                </div>
            </td>
        </tr>
    </table>
</div>

<br>

다음으로 조건문을 사용하는 방법을 알아보아요

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
                ☞	조건이 참인 경우에만 특정 명령을 수행하고 싶으면 조건 시작 카드와 조건 끝 카드 사이에 수행할 명령어 카드를 읽습니다. <br>그리고 조건이 참인 경우와 거짓인 경우 각각 다른 명령을 수행하고 싶으면 <font color="blue"><b>“조건이 맞지 않으면,”</b></font> 카드를 사용하여 구분해줍니다. 그래서 조건 시작 카드와 조건이 맞지 않으면 카드 사이에는 참인 경우에 수행할 명령어 카드를, 조건이 맞지 않으면 카드와 조건 끝 카드 사이에는 거짓인 경우에 수행할 명령어 카드를 읽습니다. <Br>항상 마지막엔 <font color="blue"><b>“조건 끝”</b></font> 카드를 읽어줘야 한다는 것을 잊지마세요!
            </td>
        </tr>
    </table>
</div>

<br>

만약, 조건을 1번만 확인하지 않고 계속 확인해야하는 경우에는 지난 강의 시간에 배운 반복문을 사용하면 됩니다. 조건문을 반복문 안에 넣어서 반복적으로 조건을 확인하도록 하는 것입니다.

<br>

<div align="center">
    <table>
        <tr>
            <td>
                <b>반복문과 조건문을 같이 사용하는 경우</b>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center"><img src="images/image5.png"></div>
            </td>
        </tr>
        <tr>
            <td>
                <img src="images/image6.png">
            </td>
        </tr>
        <tr>
            <td>
                ☞	코드를 실행하면 반복 횟수만큼 조건을 반복적으로 확인하여 참, 거짓에 따라 코딩한 명령을 실행합니다. <br>
                만약, 무한 반복을 사용한 경우에는 이 과정을 계속 반복하기 때문에 종료가 되지 않습니다. <br>
                코딩을 종료하고 코딩드론을 멈추기 위해서는 조종기를 사용하여 조종모드로 변환 후 정지시켜야 합니다. <br>
                또는 <font color="blue"><b>“반복 나가기”</b></font> 카드를 사용하여 반복문을 빠져나오게 할 수 있습니다. <Br>
                반복 나가기 카드를 조건이 참이거나 거짓인 경우에 수행할 명령어 카드로 사용하면 해당 조건이 되었을 때 반복을 중단하고 빠져나올 수 있습니다.
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
            <td rowspan="2">
                <div align="center">동작 순서</div>
            </td>
            <td>
                <div align="center">시작 → (<font color="red"><b>앞쪽 장애물을 발견하면</b></font>) U턴 / (조건이 맞지 않으면) 1칸 전진 → 끝</div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">이륙 → ((<font color="red"><b>앞쪽 장애물을 발견하지 못하면</b></font>) <font color="blue"><b>1m 전진</b></font>) x 무한 반복</div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">카드 순서</div>
            </td>
            <td>
                <div align="center">
                <img src="images/image7.png"><br>
                </div>
            </td>
        </tr>
    </table>
</div>

<br>

무한 반복문 안에(무한 반복-반복 끝 카드 사이) 조건문을 사용하여 전방에 장애물이 없는 경우(조건이 맞지 않으면-조건 끝 카드 사이)에는 계속 1m씩 전진하면서 장애물 유무를 확인할 수 있게 하였습니다. <Br>
그리고 전방에 장애물을 발견하면(앞쪽 장애물 발견하면-조건이 맞지 않으면 카드 사이) U턴(180도 좌회전)한 후 반복문을 빠져나갑니다(반복 나가기 카드 사용). <br><br>
반복문을 빠져나오면 바로 착륙하고 코딩을 종료합니다.

<br>

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
                    <img src="images/image8.png"><br>
                    카드코딩에 필요한 코딩카드들을 준비해보아요<br>
                    <font color="red"><b>※ “카드코딩 모드” 카드는 생략</b></font>
                </div>
            </td>
        </tr>
    </table>
</div>
<Br>
<div align="center">
    <table>
        <tr>
            <td colspan="2"><div align="center"><b><br><h3>2단계 코딩카드 배열하기</h3></b><br></div>
            </td>
        </tr>
        <tr>
            <td rowspan="2">
                <div align="center">동작 순서</div>
            </td>
            <td>
                <div align="center">시작 → (<font color="red"><b>앞쪽 장애물을 발견하면</b></font>) U턴 / (조건이 맞지 않으면) 1칸 전진 → 끝</div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">이륙 → ((<font color="red"><b>앞쪽 장애물을 발견하지 못하면</b></font>) <font color="blue"><b>1m 전진</b></font>) x 무한 반복</div>
            </td>
        </tr>
        <tr>
            <td colspan="2">
                <div align="center">
                <img src="images/image9.png"><br>
                </div>
            </td>
        </tr>
        <tr>
            <td colspan="2">
                <div align="center">동작 순서에 맞게 카드를 배열해 보아요. 코딩의 시작과 끝에는 항상 “코딩시작”과 “코딩끝” 카드가 온다는 것을 잊지 마세요!</div>
            </td>
        </tr>
    </table>
</div>
<Br>
<div align="center">
    <table>
        <tr>
            <td><div align="center"><b><br><h3>3단계 코딩카드 읽기</h3><br></b></div></td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image10.png">
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    코딩드론에 배터리를 장착하여 전원을 켜고 코딩카드를 읽습니다. <br>
                    코딩카드가 잘 읽히도록 올바른 위치에 코딩드론을 올려놓고(드론의 가드와 코딩카드의 가드 문양이 일치되게 합니다.) 카드 순서대로 동작버튼을 1번 눌러서 카드를 읽어주세요. <Br>
                    만약, 중간에 카드를 잘못 읽었다면 처음부터(=”코딩시작” 카드부터) 다시 시작합니다.
                </div>
            </td>
        </tr>
    </table>
</div>
<Br>
<div align="center">
    <table>
        <tr>
            <td colspan="2"><div align="center"><b><br><h3>4단계 코딩 실행하기</h3><br></b></div></td>
        </tr>
        <tr>
            <td rowspan="4">
                <div align="center">
                    <img src="images/image11.png" width="500">
                </div>
            </td>
            <td>
                <div align="center">
                    ① 만약 전방에 장애물이 있으면
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image12.png">
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    ② 만약 전방에 장애물이 없으면
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image13.png">
                </div>
            </td>
        </tr>
        <tr>
            <td colspan="2">
                <div align="center">코딩드론을 주변에 사람이나 장애물이 없는 평평한 바닥에 놓습니다. <br>
                그리고 동작버튼을 연속으로 2번 눌러서 코딩을 실행합니다. <br>
                약 3초 후 코딩드론이 자동으로 코딩한 명령을 수행합니다.<br><Br>
                <font color="red"><b>※ 동작버튼을 누른 후 즉시 드론으로부터 안전 거리만큼 떨어집니다. (안전사고 주의!)</b></font></div>
            </td>
        </tr>
    </table>
</div>

<br>

---

<br>

<div align="center">
    <h1>[정리하기]</h1>
</div>

<br>

이번 강의에서는 코딩드론의 센서를 활용한 카드코딩을 해보았습니다. <Br>
코딩드론의 전방 장애물 감지 센서(적외선 센서)로 장애물 유무를 확인하고 장애물을 피해서 비행할 수 있었습니다.<br>
이처럼 센서들을 활용한 코딩이 바로 자율비행의 기초가 됩니다. 그리고 조건문이 무엇이고 어떻게 사용하는지 배워보았습니다. <Br>
센서를 활용한 카드코딩을 하기 위해서는 조건 카드를 꼭 사용해야 한다는 것을 잊지 말아요!

<div align="center">
    <table>
        <tr>
            <td>
                <div align="left">
                    1) 센서(Sensor)란 빛, 소리, 화학물질, 온도 등과 같이 감각과 관련된 신호들을 수집하여 이 신호들을 과학적인 방법으로 분석하고 상태를 알아내는 장치입니다.<br>
                    2) 코딩드론에는 전방 장애물 감지 센서(적외선 센서), 컬러 센서, 자세 센서, 기압 센서, 옵티컬 플로우 센서 등 첨단 센서들이 장착되어 다양한 기능을 수행합니다.<br>
                    3) 코딩드론의 전방 장애물 감지 센서를 이용하여 앞쪽에 장애물 유무를 확인하고 장애물을 피해서 자율비행하는 코딩을 할 수 있습니다.<br>
                    4)센서를 활용한 코딩을 하기 위해서는 조건 카드를 사용합니다.<br>
                    5)조건문을 반복문과 함께 사용하면 조건의 참, 거짓을 판단하고 동작하는 것을 반복적으로 수행할 수 있습니다.<br>
                    6)카드코딩 실행 중에 조종기를 사용하여 조종모드로 변환하면 코딩드론을 정지시킬 수 있습니다. 또한, 무한 반복문을 사용하는 경우에는 “반복 나가기” 카드를 사용하면 반복을 중단하고 반복문을 빠져나올 수 있습니다.
                </div>
            </td>
        </tr>
    </table>
</div>

<br>

---

### [드론으로 코딩해요](../)

 1. [코딩드론과 친구해요](../lesson1)
 2. [코딩드론을 날려보아요](../lesson2)
 3. [코딩드론으로 카드코딩해요(1)](../lesson3)
 4. [코딩드론으로 카드코딩해요(2)](../lesson4)
 5. **코딩드론으로 카드코딩해요(3)**
 6. [코딩드론으로 모션코딩해요](../lesson6)
 7. [코딩드론으로 블록코딩해요(1)](../lesson7)
 8. [코딩드론으로 블록코딩해요(2)](../lesson8)

---

Modified : 2021.1.8