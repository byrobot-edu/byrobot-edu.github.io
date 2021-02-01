<br>

<div align="center">
    <h1>Lesson 8. 코딩드론으로 블록코딩해요(2)</h1>
</div>

<br>

---

<br>


<div align="center">
    <h1>[들어가기]</h1>
</div>

<br>

이번 강의에서는 조종기의 버튼을 눌러서 드론을 조종하는 코딩을 해보도록 해요. <br>
조종기의 레버를 이용하여 드론을 조종하는 것이 아니라 버튼을 눌러서 조종한다고 생각하니 신기하지 않나요? <br> 
코딩드론용 블록 중에서 조종기 버튼 이벤트 블록을 사용하면 버튼별로 이동 명령을 줄 수 있습니다.<Br>
여기서는 이륙 및 착륙과 기본 비행(전진, 후진, 좌로 이동, 우로 이동)을 해볼거예요. <Br>
<br>
그럼 시작해볼까요?

<Br>

---

<div align="center">
    <h1>[코드 생각하기]</h1>
</div>

<br>
엔트리에서 조종기 버튼과 레버 관련 블록은 2가지 종류가 있습니다.
<br>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">
                    조종기 버튼 이벤트 블록
                </div>
            </td>
            <td colspan="2">
                <div align="left">
                    ▶ 조종기의 버튼을 눌렀을 때 신호를 발생시켜 True 값을 반환합니다.
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
                    <b>버튼 종류</b>
                </div>
            </td>
            <td>
                <div align="left">
                    1. 전면 왼쪽 상단/하단 버튼<br>
                    2. 전면 오른쪽 상단/하단 버튼<br>
                    3. 상단 왼쪽/오른쪽 버튼<br>
                    4. 하단 왼쪽/오른쪽 버튼<br>
                    5. 중앙 위쪽/아래쪽/왼쪽/오른쪽 버튼(=트림 버튼)
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    조종기 조이스틱(레버) 이벤트 블록
                </div>
            </td>
            <td colspan="2">
                <div align="left">
                    ▶ 조종기의 조이스틱(레버)을 특정 방향으로 움직였을 때 신호를 발생시켜 True 값을 반환합니다.
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
                    <b>조이스틱(레버) 방향(왼쪽/오른쪽 공통)</b>
                </div>
            </td>
            <td>
                <div align="left">
                    총 9방향 : 상, 좌상, 우상, 하, 좌하, 우하, 좌, 우, 센터
                </div>
            </td>
        </tr>
        <tr>
            <td colspan="3">
                <div align="left">
                    다음과 같이 엔트리의 조건문 블록에 판단 블록으로 조립하여 사용합니다.<br><br>
                </div>
                <div align="center">
                    <img src="images/image3.png">
                </div>
            </td>
        </tr>
    </table>
</div>

<br>

조종기 버튼에 따라 드론이 다음과 같이 동작하는 코딩을 해보아요.

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image4.png">
                </div>
            </td>
            <td>
                <div align="center">
                    <img src="images/image5.png">
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    이륙하기 : 하단 왼쪽 버튼
                </div>
            </td>
            <td>
                <div align="center">
                    착륙하기 : 하단 오른쪽 버튼
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image6.png">
                </div>
            </td>
            <td>
                <div align="center">
                    <img src="images/image7.png">
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    1m 전진하기 : 중앙 위 버튼
                </div>
            </td>
            <td>
                <div align="center">
                    1m 후진하기 : 중앙 아래 버튼
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image8.png">
                </div>
            </td>
            <td>
                <div align="center">
                    <img src="images/image9.png">
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    1m 좌로 이동하기 : 중앙 왼쪽 버튼
                </div>
            </td>
            <td>
                <div align="center">
                    1m 우로 이동하기 : 중앙 오른쪽 버튼
                </div>
            </td>
        </tr>
    </table>
</div>

<br>

<br>

그럼 먼저 각 명령별로 코드를 어떻게 만들어야 할지 생각해보아요.

<br>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">
                    명령
                </div>
            </td>
            <td>
                <div align="center">
                    코드
                </div>
            </td>
            <td>
                <div align="center">
                    설명
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    이륙하기
                </div>
            </td>
            <td>
                <div align="center">
                    <img src="images/image10.png">
                </div>
            </td>
            <td>
                <div align="left">
                    조종기의 하단 왼쪽 버튼(=S버튼)을 누르면 드론이 이륙한 후 3초간 호버링 합니다.
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    착륙하기
                </div>
            </td>
            <td>
                <div align="center">
                    <img src="images/image11.png">
                </div>
            </td>
            <td>
                <div align="left">
                    조종기의 하단 오른쪽 버튼(=P버튼)을 누르면 드론이 3초간 호버링 후 착륙합니다.
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    1m 전진하기
                </div>
            </td>
            <td>
                <div align="center">
                    <img src="images/image12.png">
                </div>
            </td>
            <td>
                <div align="left">
                    조종기의 중앙 위 버튼(=트림 ▲버튼)을 누르면 드론이 1m 전진한 후 3초간 호버링합니다.
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    1m 후진하기
                </div>
            </td>
            <td>
                <div align="center">
                    <img src="images/image13.png">
                </div>
            </td>
            <td>
                <div align="left">
                    조종기의 중앙 아래쪽 버튼(=트림 ▼버튼)을 누르면 드론이 1m 후진한 후 3초간 호버링합니다.
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    1m 좌로 이동하기
                </div>
            </td>
            <td>
                <div align="center">
                    <img src="images/image14.png">
                </div>
            </td>
            <td>
                <div align="left">
                    조종기의 중앙 위 버튼(=트림 ◀버튼)을 누르면 드론이 1m 좌로 이동한 후 3초간 호버링합니다.
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    1m 우로 이동하기
                </div>
            </td>
            <td>
                <div align="center">
                    <img src="images/image15.png">
                </div>
            </td>
            <td>
                <div align="left">
                    조종기의 중앙 위 버튼(=트림 ▶버튼)을 누르면 드론이 1m 우로 이동한 후 3초간 호버링합니다.
                </div>
            </td>
        </tr>
    </table>
</div>

<br>

이제 위 코드들을 합쳐서 하나의 코드로 만들어볼까요?

<br>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">
                    코드
                </div>
            </td>
            <td>
                <div align="center">
                    설명
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image16.png">
                </div>
            </td>
            <td>
                <div align="left">
                    각 명령별 코드를 모두 계속 반복하기 블록 안에 넣어 하나의 코드로 조립합니다. <br>
                    엔트리는 순차적 코딩 프로그램이기 때문에 블록이 순차적으로 1번씩만 실행됩니다.<br>
                    그러므로 계속 반복하기 블록을 사용해야 조종기의 버튼 동작 신호를 지속적으로 감지하여 명령을 실행할 수 있습니다.
                </div>
            </td>
        </tr>
    </table>
</div>

<br>

---

<br>


<div align="center">
    <h1>[코딩 및 실행하기]</h1>
</div>

<br>

<h2> 1. 코딩하기</h2>
<br>

엔트리에서 블록들을 조립하여 코드를 만들어보아요

<br>

<div align="center">
    <img src="images/image17.png">
</div>

<br>

<h2> 2. 실행하기</h2>

<br>

코드를 모두 만들었다면 시작하기 버튼을 클릭하여 실행해보아요.<br>
실행하기 전에 다음 사항을 먼저 확인합니다.<br>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center"><img src="images/image18.png"></div>
            </td>
            <td>
                <div align="left"><b>
                잠깐! 엔트리에서 드론 자율비행 코드를 실행하기 전에 한 번 더 확인해봐요!</b><br><Br>
                1) 드론과의 안전거리(2m 이상)를 확보합니다.<Br>
                2) 드론 주변에 사람이나 장애물이 없는지 확인합니다.<br>
                ☞ 코드의 드론 이동 방향과 거리를 예측하여 경로에 사람이나 장애물이 없는지 확인합니다.<Br>
                3) 드론의 오작동이나 엔트리 오류 발생 시 드론을 강제로 멈추는 방법을 확인합니다.
                </div>
            </td>
        </tr>
    </table>
</div>

<Br>

준비가 되었다면 코드를 실행하고 조종기의 하단 왼쪽 버튼(=S버튼)을 눌러보아요. <br>
드론이 이륙하나요? 그럼 다음으로 중앙 위, 아래, 왼쪽, 오른쪽 버튼(=트림 버튼)을 차례대로 누르면서 명령대로 드론이 비행하는지 확인합니다. <Br>
만약 자신이 생각한대로 비행하지 않는다면 어느 부분이 잘못되었는지 확인하여 수정한 후 다시 실행해보세요.<Br>

<br>

---

<br>

<div align="center">
    <h1>[정리하기]</h1>
</div>

이번 강의에서는 조종기의 버튼을 눌러서 드론을 조종하는 코딩을 해보았습니다. <br>
조종기의 레버 대신에 버튼으로 드론을 조종해보니 재미있지 않나요? <Br>
이처럼 조종기 버튼과 레버 이벤트 블록을 이용하면 실제 조종하는 것처럼 드론을 비행시킬 수 있을 뿐만 아니라, 실제 조종법과 다르게 드론이 동작하도록 코딩하여 나만의 조종기를 만들 수도 있습니다.

<div align="center">
    <table>
        <tr>
            <td>
                <div align="left">
                    1) 조종기의 버튼을 누르거나 조이스틱(레버)를 움직였을 때, 조종기 이벤트 블록을 사용하여 드론이 특정 명령을 수행하도록 할 수 있습니다.<br>
                    2) 조종기 이벤트 블록은 2가지 종류(버튼 이벤트 블록, 조이스틱(레버) 이벤트 블록)가 있고, 조건문 블록의 판단 블록으로 사용합니다.<br>
                    3)조종기 이벤트 블록은 버튼이나 조이스틱(레버)의 동작 신호가 발생하였는지 지속적으로 확인해야 하기 때문에 계속 반복하기 블록을 같이 사용합니다.<br>
                </div>
            </td>
        </tr>
    </table>
</div>

---

### [드론으로 코딩해요](../)

 1. [코딩드론과 친구해요](../lesson1)
 2. [코딩드론을 날려보아요](../lesson2)
 3. [코딩드론으로 카드코딩해요(1)](../lesson3)
 4. [코딩드론으로 카드코딩해요(2)](../lesson4)
 5. [코딩드론으로 카드코딩해요(3)](../lesson5)
 6. [코딩드론으로 모션코딩해요](../lesson6)
 7. [코딩드론으로 블록코딩해요(1)](../lesson7)
 8. **코딩드론으로 블록코딩해요(2)**
---

Modified : 2021.2.1