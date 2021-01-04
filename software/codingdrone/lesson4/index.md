<br>

<div align="center">
    <h1>Lesson 4. 코딩드론으로 카드코딩해요(2)</h1>
</div>

<br>

---

<br>


<div align="center">
    <h1>[들어가기]</h1>
</div>

<br>

이번 강의에서는 코딩드론으로 패턴 비행하는 카드코딩을 해보려고 합니다. <br>
패턴 비행이란 일정한 형태의 루트로 비행하는 것을 말하는데, 삼각형, 사각형, 원형, 나선형 등을 예로 들 수 있습니다. <Br>
이러한 패턴 비행은 촬영, 농업, 측량 등 다양한 산업 분야에서 드론이 활용될 때 사용됩니다. 여기서는 사각형 패턴 비행을 해볼거예요.<Br><br>
그리고 패턴 비행은 루트가 정형화되어 있기 때문에 일부 패턴이 반복되는 경우가 있습니다. <br>
이 경우에는 코딩할 때 반복문을 사용하여 코드를 간단하게 만들 수 있습니다. <br>
이번 강의에서 패턴 비행을 통해 반복문이 무엇이고 어떻게 활용할 수 있는지 같이 배워보아요.<br>

<br>

<div align="center">
    <h1>[코드 생각하기]</h1>
</div>

<br>

사각형 패턴 주행 순서는 1칸 전진하기와 좌회전하기를 4회 반복합니다.

<div align="center"><b>4회 반복하기</b></div>
<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">① 1칸 전진하기</div>
            </td>
            <td>
                <div align="center">②좌회전하기</div>
            </td>
        </tr>
    </table>
</div>

<br>

위와 같이 주행하려면 어떻게 코드를 짜야 할지 생각해볼까요? 먼저 반복문을 사용하지 않고 코드를 만들어보아요.

<br>

<h2>1. 사각형 패턴 주행(반복문 미사용)</h2>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">동작 순서</div>
            </td>
            <td>
                <div align="center">시작 → 이륙 → (1칸 전진 → 90도 좌회전) x 4 → 착륙 → 끝</div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">카드 순서</div>
            </td>
            <td>
                <img src="images/image1.png">
            </td>
        </tr>
    </table>
</div>

<br>

다음으로 반복문을 사용하여 코드를 만들어볼까요? 먼저 반복문이 무엇인지 알아봅시다.
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
                    반복문
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
                    반복문이란 코딩의 주요 문법 중 하나로서 동일하거나 비슷한 명령을 반복할 때 사용합니다. <br>반복문을 사용하면 코드의 길이를 줄여줘서 코드를 이해하기 쉽게 해줄 뿐만 아니라, 좀 더 다양하고 효율적인 코딩 구현이 가능합니다.<br><Br>
                    반복문에는 특정 조건이 만족할 때까지 반복하기, 지정한 횟수만큼 반복하기, 무한 반복하기 등 여러 종류가 있는데, GoCar의 카드코딩에서는 지정한 횟수만큼 반복하기와 무한 반복하기가 가능합니다.
                </div>
            </td>
        </tr>
    </table>
</div>

<br>

카드코딩에서 기본적으로 제공되는 반복문은 총 4가지입니다.

<br>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">① 무한 반복</div>
            </td>
            <td>
                <div align="center">② 2회 반복</div>
            </td>
            <td>
                <div align="center">③ 3회 반복</div>
            </td>
            <td>
                <div align="center">④ 4회 반복</div>
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

반복문을 사용하는 방법은 다음과 같습니다.

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
                <div align="center">☞ 반복 시작 카드(무한 반복, 2회 반복, 3회 반복, 4회 반복)와 반복 끝 사이에 반복 수행할 명령어 카드들을 차례대로 읽어주면 반복 명령이 입력됩니다.</div>
            </td>
        </tr>
    </table>
</div>

<br>
그럼 이제 반복문을 사용하여 사각형 패턴 주행 코드를 만들어보아요. 반복문을 사용하지 않은 코드와 어떻게 달라지는지 비교해보아요.
<br>

<br>

<h2>2. 사각형 패턴 주행(반복문 사용)</h2>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">동작 순서</div>
            </td>
            <td>
                <div align="center">시작 → 이륙 → (1칸 전진 → 90도 좌회전) x 4 → 착륙 → 끝</div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">카드 순서</div>
            </td>
            <td>
                <img src="images/image8.png" alt="사각형 패턴 비행(반복문 사용)">
            </td>
        </tr>
    </table>
</div>

<br>

반복문을 사용하지 않은 코드보다 많이 단순화된 것을 알 수 있죠? <br>
이처럼 특정 명령을 반복하는 동작을 수행할 때 반복문을 사용하면 코드를 좀 더 간결하고 쉽게 만들 수 있습니다. 이제 코드를 실행해볼까요?

---

<br>


<div align="center">
    <h1>[코딩 및 실행하기]</h1>
</div>

<br>

<h2>1. 사각형 패턴 주행(반복문 미사용)</h2>

<br>

<div align="center">
    <table>
        <tr>
            <td><br><div align="center"><b><h3>1단계 코딩카드 준비하기</h3><br></b></div></td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image9.png" alt="사각형 패턴 비행(반복문 미사용) 1단계"><br>
                    카드코딩에 필요한 코딩카드들을 준비해보아요<br>
                    <font color="red"><b>※ “카드코딩 모드” 카드는 생략</b></font>
                </div>
            </td>
        </tr>
        <tr>
            <td><div align="center"><b><br><h3>2단계 코딩카드 배열하기</h3><br>
            이륙 → (1칸 전진 → 90도 좌회전) x 4번 반복 → 착륙</b></div></td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image10.png" alt="사각형 패턴 비행(반복문 미사용) 2단계"><br>
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
                    <img src="images/image11.png" alt="사각형 패턴 비행(반복문 미사용) 3단계"><br>
                    코딩드론에 배터리를 장착하여 전원을 켜고 코딩카드를 읽습니다. <br>
                    코딩카드가 잘 읽히도록 올바른 위치에 코딩드론을 올려놓고(드론의 가드와 코딩카드의 가드 문양이 일치되게 합니다.) <br>
                    카드 순서대로 동작버튼을 1번 눌러서 카드를 읽어주세요. <br>
                    만약, 중간에 카드를 잘못 읽었다면 처음부터(=”코딩시작” 카드부터) 다시 시작합니다.<br><Br>
                </div>
            </td>
        </tr>
        <tr>
            <td><div align="center"><b><br><h3>4단계 코딩 실행하기</h3><br></b></div></td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image12.png" height="350" width="341" alt="사각형 패턴 비행(반복문 미사용) 4단계1"><img src="images/image13.png" height="500" width="550" alt="사각형 패턴 비행(반복문 미사용) 4단계2"><br>
                    코딩드론을 주변에 사람이나 장애물이 없는 평평한 바닥에 놓습니다. <br>
                    그리고 동작버튼을 연속으로 2번 눌러서 코딩을 실행합니다. 약 3초 후 코딩드론이 자동으로 코딩한 명령을 수행합니다.<br><br>
                    <font color="red"><b>※ 동작버튼을 누른 후 즉시 드론으로부터 안전 거리만큼 떨어집니다. (안전사고 주의!)</b></font>
                </div>
            </td>
        </tr>
    </table>
</div>
<br>

다음은 반복문을 사용한 코드를 실행해보아요.

<br>

<h2>2. 사각형 패턴 주행(반복문 사용)</h2>

<br>

<div align="center">
    <table>
        <tr>
            <td><div align="center"><b><br><h3>1단계 코딩카드 준비하기</h3><br></b></div></td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image14.png" alt="사각형 패턴 비행(반복문 사용) 1단계"><br>
                    카드코딩에 필요한 코딩카드들을 준비해보아요.<br>
                    <font color="red"><b>※ “카드코딩 모드” 카드는 생략</b></font>
                </div>
            </td>
        </tr>
        <tr>
            <td><div align="center"><b><br><h3>2단계 코딩카드 배열하기</h3><br><br>
            동작순서 : 이륙 → (1칸 전진 → 90도 좌회전) x 4번 반복 → 착륙<br><br></b></div></td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image15.png" alt="사각형 패턴 비행(반복문 사용) 2단계"><br>
                    동작 순서에 맞게 카드를 배열해 보아요. 코딩의 시작과 끝에는 항상 “코딩시작”과 “코딩끝” 카드가 온다는 것을 잊지 마세요!
                </div>
            </td>
        </tr>
        <tr>
            <td><div align="center"><b><br><h3>3단계 코딩카드 읽기</h3><br></b></div></td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image16.png"  alt="사각형 패턴 비행(반복문 사용) 3단계"><br>
                    코딩드론에 배터리를 장착하여 전원을 켜고 코딩카드를 읽습니다.<br>
                    코딩카드가 잘 읽히도록 올바른 위치에 코딩드론을 올려놓고(드론의 가드와 코딩카드의 가드 문양이 일치되게 합니다.) 카드 순서대로 동작버튼을 1번 눌러서 카드를 읽어주세요. <br>
                    만약, 중간에 카드를 잘못 읽었다면 처음부터(=”코딩시작” 카드부터) 다시 시작합니다.<br><br>
                </div>
            </td>
        </tr>
        <tr>
            <td><div align="center"><b><br><h3>4단계 코딩 실행하기</h3><br></b></div></td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image12.png" height="350" width="341" alt="사각형 패턴 비행(반복문 사용) 4단계1"><img src="images/image13.png" height="500" width="550" alt="사각형 패턴 비행(반복문 사용) 4단계2"><br>
                    코딩드론을 주변에 사람이나 장애물이 없는 평평한 바닥에 놓습니다. <br>
                    그리고 동작버튼을 연속으로 2번 눌러서 코딩을 실행합니다. 약 3초 후 코딩드론이 자동으로 코딩한 명령을 수행합니다.<br><br>
                    <font color="red"><b>※ 동작버튼을 누른 후 즉시 드론으로부터 안전 거리만큼 떨어집니다. (안전사고 주의!)</b></font>
                </div>
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

이번 강의에서는 코딩드론으로 카드코딩하여 사각형 패턴 비행을 해보았습니다. <Br>
그리고 동일하게 반복되는 패턴은 반복문을 활용하면 더욱 쉽게 코딩할 수 있다는 것도 배웠습니다. <Br>
이제 사각형 외에 다른 패턴들도 어떻게 코드를 짜야 할지 고민해보고 카드코딩해서 비행시켜보아요.<Br>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="left">
                    1) 패턴 비행이란 일정한 형태의 루트로 비행하는 것을 말하는데, 삼각형, 사각형, 원형, 나선형 등을 예로 들 수 있습니다.<br>
                    2) 패턴 비행은 루트가 정형화되어 있기 때문에 일부 패턴이 반복되는 경우가 있는데, 이 경우에는 반복 카드를 사용할 수 있습니다.<br>
                    3) 코딩에서 반복문을 활용하면 코드를 좀 더 간결하게 만들 수 있어서 코딩을 더욱 쉽게 할 수 있습니다.<br>
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
 4. **코딩드론으로 카드코딩해요(2)**
 5. [코딩드론으로 카드코딩해요(3)] - 업데이트 예정
 6. [코딩드론으로 모션코딩해요] - 업데이트 예정
 7. [코딩드론으로 블록코딩해요(1)] - 업데이트 예정
 8. [코딩드론으로 블록코딩해요(2)] - 업데이트 예정
---

Modified : 2021.1.4