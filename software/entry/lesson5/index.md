<br>

<div align="center">
    <h1>Lesson 5. 엔트리로 드론을 날려보아요</h1>
</div>

<br>

---

<br>


<div align="center">
    <h1>[들어가기]</h1>
</div>

<br>

이번 강의부터는 페트론 V2을 활용한 코딩을 해보려고 합니다. 엔트리 하드웨어 연결 시 ‘바이로봇 페트론 V2 드론’을 선택하여 연결해주세요. 이번 강의에서는 첫번째로 드론의 기본 비행을 엔트리로 코딩하여 자율비행 시켜보도록 하겠습니다. 어렵지 않은 간단한 코드를 직접 만들어보고 코드의 명령대로 드론이 비행하는 것을 보면서 페트론 V2와 친해져 보아요!


<br>

---

<br>


<div align="center">
    <h1>[코드 생각하기]</h1>
</div>

<br>

드론의 기본 비행은 다음과 같습니다.

1. 이륙/착륙<br>
2. 상승/하강<br>
3. 전진/후진<br>
4. 좌/우 이동<br>
5. 좌/우 회전

<br>

기본 비행을 코딩하기 전에 엔트리에서 페트론 V2 자율비행을 코딩하기 위해서는 드론의 비행 원리와 관련된 용어를 알아야합니다. 다음 그림을 보면서 자세히 알아보아요.

<div align="center">
    <img src="images/image146.png">
</div>

①	<b>Throttle</b> : 드론이 상승 또는 하강합니다.<br>
②	<b>Pitch</b> : 드론이 전진 또는 후진합니다.<br>
③	<b>Roll</b> : 드론이 좌 또는 우로 이동합니다.<br>
④	<b>Yaw</b> : 드론이 좌 또는 우로 회전합니다.

<br>

---

<br>


<div align="center">
    <h1>[코딩 및 실행하기]</h1>
</div>

<br>

<h3> 1. 이륙/착륙 </h3>
<br>
모든 비행의 기본이 되는 이착륙부터 시작해보아요. 모든 비행에는 이륙과 착륙이 있어야 합니다.
<br>

<div align="center">
    <img src="images/image147.png">
</div>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image148.png"><br>
                    이륙 블록
                </div>
            </td>
            <td>
                <div align="left">
                    페트론 V2가 이륙합니다. 약 60cm 높이까지 이륙 후 호버링합니다.<br>
                    <font color="red">※ 배터리 잔량과 드론의 상태에 따라 이륙하는 높이는 차이가 날 수 있습니다.</font>
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image149.png"><br>
                    기다리기 블록
                </div>
            </td>
            <td>
                <div align="left">
                    현재 상태를 설정한 시간 동안 유지합니다. 약 60cm 높이까지 상승하여 이륙을 완료하기 위해서는 약 5초의 시간이 필요합니다. 5초 기다리기 블록을 사용하여 이륙 완료 후, 다음 동작이 수행될 수 있도록 합니다.
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image150.png"><br>
                    착륙 블록
                </div>
            </td>
            <td>
                <div align="left">
                    페트론 V2가 착륙합니다. 블록이 실행되면 현재 위치에서 착륙합니다. 드론에 충격을 줄 수 있으므로 착륙은 50cm 정도 높이에서 실행합니다.
                </div>
            </td>
        </tr>
    </table>
</div>

<br>

코드를 다 만들었다면 실행해볼까요?

<br>
<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image151.png">
                </div>
            </td>
            <td>
                <div align="left">
                    <b>잠깐! 엔트리에서 드론 자율비행 코드를 실행하기 전에 한 번 더 확인해봐요!</b><br><br>
                    1. 드론과의 안전거리(3m 이상)를 확보합니다.<br>
                    2. 드론 주변에 사람이나 장애물이 없는지 확인합니다.<br>
                    　☞ 코드의 드론 이동 방향과 거리를 예측하여 경로에 사람이나 장애물이 없는지 확인합니다.<br>
                    3. 드론의 오작동이나 바이블럭 오류 발생 시 드론을 강제로 멈추는 방법을 확인합니다.
                </div>
            </td>
        </tr>
    </table>
</div>

<br>

드론이 어떻게 비행하나요? 자신이 만든 코드 순서대로 드론이 잘 비행한다면 성공한 것입니다. 그럼 다른 기본 비행들도 코드를 만들어서 실행해보아요. 코드를 만들기 전에 단일 조종 블록에 대해서 먼저 알아볼까요?

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image152.png">
                </div>
            </td>
            <td>
                <div align="left">
                    ①	조종유형: Throttle / Roll / Pitch / Yaw 중에서 선택하여 드론을 어떻게 비행할지 정합니다.<br>
                    ②	조종값: -100~100 사이의 값을 입력 가능하고, 값에 따라 드론의 속도를 조절할 수 있습니다. 절대값이 클수록 모터의 출력이 커져서 드론의 속도가 빨라집니다.<br>
                    ③	실행시간: 설정한 조종유형과 조종값으로 드론을 얼마나 비행시킬지 시간을 입력합니다. (0.01초 단위)<br>
                    <font color="red">※	조종값과 실행시간은 주어진 공간과 환경에 맞게 조절하여 사용합니다.</font>
                </div>
            </td>
        </tr>
    </table>
</div>

<h4> Q. 다음 단일 조종 블록의 차이점은? </h4><br>


<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">
                    블록 1
                </div>
            </td>
            <td>
                <div align="center">
                    <img src="images/image153.png">
                </div>
            </td>
            <td>
                <div align="left">
                    설정한 조종유형과 조종값을 계속 유지하면서 드론이 비행합니다. <br>
                    블록이 실행되고 바로 다음 블록으로 넘어가기 때문에 비행 중 다른 명령을 추가하고 싶을 때 사용할 수 있습니다. <br>
                    다시 조종값을 0으로 설정하거나 드론을 착륙시키면 비행을 멈출 수 있습니다.
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    블록 2
                </div>
            </td>
            <td>
                <div align="center">
                    <img src="images/image154.png">
                </div>
            </td>
            <td>
                <div align="left">
                    설정한 조종유형과 조종값으로 실행시간동안 드론이 비행합니다. <br>
                    실행시간이 모두 지나면 비행을 멈추고 다음 블록으로 넘어갑니다. <br>
                    일정 시간동안 특정 비행을 하고 싶을 때 사용합니다.
                </div>
            </td>
        </tr>
    </table>
</div>

<br>

<h3> 2. 상승/하강 </h3>

<br>

<div align="center">
    <img src="images/image155.png">
</div>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image156.png"><br>
                    단일조종(지정시간) – 스로틀(상승) 블록
                </div>
            </td>
            <td>
                <div align="left">
                    페트론 V2가 상승합니다. %는 조종값으로 -100~100까지 입력 가능하고, 절대값이 클수록 모터의 출력이 커져서 드론의 이동 속도가 빨라집니다. 시간은 0.01초 단위로 입력 가능하고, 입력한 시간 동안 상승합니다.<br>
                    ▶조종값 : 양수 → 상승 / 음수 → 하강<br>
                    ▶입력한 시간 동안 상승한 후 다음 블록이 실행됩니다.
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image157.png"><br>
                    단일조종(지정시간) – 스로틀(하강) 블록
                </div>
            </td>
            <td>
                <div align="left">
                    페트론 V2가 하강합니다. %는 조종값으로 -100~100까지 입력 가능하고, 절대값이 클수록 모터의 출력이 커져서 드론의 이동 속도가 빨라집니다. 시간은 0.01초 단위로 입력 가능하고, 입력한 시간 동안 하강합니다.<br>
                    ▶조종값 : 양수 → 상승 / 음수 → 하강<br>
                    ▶입력한 시간 동안 하강한 후 다음 블록이 실행됩니다.
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image158.png"><br>
                    기다리기 블록
                </div>
            </td>
            <td>
                <div align="left">
                    드론이 어떤 동작 후에는 자세를 잡고 센서가 안정화되는 시간이 필요하고, 엔트리에서 코드 명령이 페트론 V2에 잘 전달되기 위해서도 시간이 필요합니다(Delay time). 그래서 이와 같이 비행 관련 블록 다음에는 꼭 기다리기 블록을 사용하여 안정적인 자율비행이 될 수 있도록 합니다.<br>
                    ▶비행 동작 후에는 보통 2~3초 기다리기를 사용합니다.
                </div>
            </td>
        </tr>
    </table>
</div>

<br>
<h3> 3. 전진/후진 </h3>

<br>

<div align="center">
    <img src="images/image159.png">
</div>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image160.png"><br>
                    단일조종(지정시간) – 피치(전진) 블록
                </div>
            </td>
            <td>
                <div align="left">
                    페트론 V2가 전진합니다. %는 조종값으로 -100~100까지 입력 가능하고, 절대값이 클수록 모터의 출력이 커져서 드론의 이동 속도가 빨라집니다. 시간은 0.01초 단위로 입력 가능하고, 입력한 시간 동안 전진합니다.<br>
                    ▶조종값 : 양수 → 전진 / 음수 → 후진<br>
                    ▶입력한 시간 동안 전진한 후 다음 블록이 실행됩니다.
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image161.png"><br>
                    단일조종(지정시간) – 피치(후진) 블록
                </div>
            </td>
            <td>
                <div align="left">
                    페트론 V2가 후진합니다. %는 조종값으로 -100~100까지 입력 가능하고, 절대값이 클수록 모터의 출력이 커져서 드론의 이동 속도가 빨라집니다. 시간은 0.01초 단위로 입력 가능하고, 입력한 시간 동안 후진합니다.<br>
                    ▶조종값 : 양수 → 전진 / 음수 → 후진<br>
                    ▶입력한 시간 동안 후진한 후 다음 블록이 실행됩니다.
                </div>
            </td>
        </tr>
    </table>
</div>
<br>
<h3> 4. 좌/우 이동 </h3>

<br>

<div align="center">
    <img src="images/image162.png">
</div>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image163.png"><br>
                    단일조종(지정시간) – 롤(우 이동) 블록
                </div>
            </td>
            <td>
                <div align="left">
                    페트론 V2가 우(오른쪽)로 이동합니다. %는 조종값으로 -100~100까지 입력 가능하고, 절대값이 클수록 모터의 출력이 커져서 드론의 이동 속도가 빨라집니다. 시간은 0.01초 단위로 입력 가능하고, 입력한 시간 동안 우로 이동합니다.<br>
                    ▶조종값 : 양수 → 우로 이동 / 음수 → 좌로 이동<br>
                    ▶입력한 시간 동안 후진한 후 다음 블록이 실행됩니다.
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image164.png"><br>
                    단일조종(지정시간) – 롤(좌 이동) 블록
                </div>
            </td>
            <td>
                <div align="left">
                    페트론 V2가 좌(왼쪽)로 이동합니다. %는 조종값으로 -100~100까지 입력 가능하고, 절대값이 클수록 모터의 출력이 커져서 드론의 이동 속도가 빨라집니다. 시간은 0.01초 단위로 입력 가능하고, 입력한 시간 동안 좌로 이동합니다.<br>
                    ▶조종값 : 양수 → 우로 이동 / 음수 → 좌로 이동<br>
                    ▶입력한 시간 동안 후진한 후 다음 블록이 실행됩니다.
                </div>
            </td>
        </tr>
    </table>
</div>
<br>
<h3> 5. 좌/우 회전 </h3>

<br>

<div align="center">
    <img src="images/image165.png">
</div>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image166.png"><br>
                    단일조종(지정시간) – 요(우 회전) 블록
                </div>
            </td>
            <td>
                <div align="left">
                    페트론 V2가 우(오른쪽)로 회전합니다. %는 조종값으로 -100~100까지 입력 가능하고, 절대값이 클수록 모터의 출력이 커져서 드론의 이동 속도가 빨라집니다. 시간은 0.01초 단위로 입력 가능하고, 입력한 시간 동안 우로 회전합니다.<br>
                    ▶조종값 : 양수 → 우로 회전 / 음수 → 좌로 회전<br>
                    ▶입력한 시간 동안 후진한 후 다음 블록이 실행됩니다.
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image167.png"><br>
                    우 회전(지정시간) 블록
                </div>
            </td>
            <td>
                <div align="left">
                    페트론 V2가 좌(왼쪽)로 회전합니다. %는 조종값으로 -100~100까지 입력 가능하고, 절대값이 클수록 모터의 출력이 커져서 드론의 이동 속도가 빨라집니다. 시간은 0.01초 단위로 입력 가능하고, 입력한 시간 동안 좌로 회전합니다.<br>
                    ▶조종값 : 양수 → 우로 회전 / 음수 → 좌로 회전<br>
                    ▶입력한 시간 동안 후진한 후 다음 블록이 실행됩니다.
                </div>
            </td>
        </tr>
    </table>
</div>

모든 기본 비행이 잘 동작하나요? 그렇다면 Throttle, Pitch, Roll, Yaw를 번갈아서 비행하는 코드를 만들어보고, 조종값과 실행시간을 변화시키면서 비행시켜보아요.<br>

<font color="red"><b>※	조종값과 실행시간은 주어진 공간과 환경에 맞게 조절하여 사용합니다. 작은 값부터 시작하여 점점 값을 늘려가며 비행시킵니다.</b></font>

<br>

---

<br>


<div align="center">
    <h1>[정리하기]</h1>
</div>

<br>

엔트리, 페트론 V2와 좀 친숙해졌나요? 조종값과 비행 시간을 바꿔보고 블록들을 다르게 조합하여 실행해보면서 좀 더 다양하고 재미있게 자율비행을 즐겨봅시다.

1. 이/착륙 블록은 처음에 드론을 이륙시키고, 마지막에 착륙시킬 때 사용합니다.
2. 기본 비행 블록에서 방향, 조종값, 비행 시간을 설정하여 드론을 자율비행시킬 수 있습니다.
3. 조종값이 크면 모터의 출력이 커져서 드론의 이동 속도가 빨라집니다.
4. 이륙 후 5초 기다리기 블록을 사용하여 드론이 완전히 이륙할 수 있도록 합니다.
5. 비행 동작 후에는 3초 기다리기 블록을 사용하여 다음 명령이 드론에게 잘 전달될 수 있도록 합니다.


<br>

---

### [엔트리로 코딩해요](../)

 1. [페트론 V2와 엔트리가 만났어요](../lesson1)
 2. [조종기로 음악을 연주해보아요](../lesson2)
 3. [조종기 화면에 그림을 그려보아요](../lesson3)
 4. [조종기로 로봇청소기를 돌려보아요](../lesson4)
 5. **엔트리로 드론을 날려보아요**
 6. [드론으로 센서 놀이를 해보아요](../lesson6)
 7. [센서를 활용한 패턴 비행을 해보아요](../lesson7)
 8. [조종기 버튼으로 드론을 날려보아요](../lesson8)
 
---

Modified : 2019.1.15