<br>

<div align="center">
    <h1>Lesson 3. 조종기 화면에 그림을 그려보아요!</h1>
</div>

<br>

---

<br>


<div align="center">
    <h1>[들어가기]</h1>
</div>

<br>
이번 강의에서는 조종기의 디스플레이 화면에 점, 선, 면을 그려보고 문자를 표시하는 코딩을 해보려고 합니다. 페트론 V2의 조종기에는 OLED 디스플레이 화면이 있어서 드론과 비행 관련 정보들을 확인할 수 있고, 드론과 조종기의 각종 설정값을 세팅할 수 있습니다. 바로 이곳에 엔트리 코딩으로 그림을 그리고 문자를 찍어서 조종기를 멋지게 꾸밀 수 있답니다. 그럼 자신만의 조종기를 꾸미러 가볼까요?

---

<br>
<div align="center">
    <h1>[코드 생각하기]</h1>
</div>

<br>

<h2> 1. 점 그리기</h2>

점으로 화면 가운데 덧셈 기호 ‘+’를 그려보세요. 다음은 점 그리기 블록 설명입니다.

<div align="center">
    <table>
        <tr>
            <td><img src="images/image60.png"></td>
            <td>조종기 화면의 지정한 위치에 점을 찍습니다. <br>
            흰색과 검은색 중에서 색상을 선택할 수 있고, 점 찍는 위치는 x, y 좌표값으로 지정합니다.<br>
            x 좌표: 화면상의 가로 위치로서 범위는 0~128입니다. 화면 왼쪽부터 0에서 시작합니다. (중앙: 64)<br>
            y 좌표: 화면상의 세로 위치로서 범위는 0~64입니다. 화면 위쪽부터 0에서 시작합니다. (중앙: 32)
            </td>
        </tr>
    </table>
</div>

<div align="center">
    <img src="images/image32(2).png" alt="음계블록">
</div>

①번 블록에서 영어 음계는 각각 다음 음을 나타냅니다.
<br>
<div align="center">
    <table>
        <tr>
            <td>C</td>
            <td>CS</td>
            <td>D</td>
            <td>DS</td>
            <td>E</td>
            <td>F</td>
            <td>FS</td>
            <td>G</td>
            <td>GS</td>
            <td>A</td>
            <td>AS</td>
            <td>B</td>
        </tr>
        <tr>
            <td>도</td>
            <td>도＃</td>
            <td>레</td>
            <td>레＃</td>
            <td>미</td>
            <td>파</td>
            <td>파＃</td>
            <td>솔</td>
            <td>솔＃</td>
            <td>라</td>
            <td>라＃</td>
            <td>시</td>
        </tr>
    </table>
</div>
<br>
<h2> 2. 드론 LED 꾸며보기</h2>
<br>
드론이 눈과 팔 부분의 LED 색상을 다음과 같이 바꿔가며 비행하는 코드를 만들어봅니다.<br> 드론의 LED 색상을 제어할 수 있는 블록은 “색상” 카테고리에 있습니다.

1) 드론 이륙하기<br>
2) 눈과 팔 LED 모두 빨강으로 바꾸기<br>
3) 3초간 상승하기<br>
4) 눈과 팔 LED 모두 파랑으로 바꾸기<br>
5) 좌로 회전하기<br>
6) 회전하면서 3초 뒤 눈과 팔 LED 모두 초록으로 바꾸기<br>
7) 3초 더 회전 후 회전 멈추기<br>
8) 눈 LED는 빨강, 팔 LED는 파랑으로 바꾸고 깜빡이기<br>
9) 3초간 하강하기<br>
10) 착륙하기<br>

<br>

---

<div align="center">
    <h1>[코딩 및 실행하기]</h1>
</div>

<br>

<h2> 1. 조종기로 음악 연주하기</h2>
<br>
<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image33(2).png"><br>
                </div>
            </td>
            <td>
                <div align="center">
                    <img src="images/image34(2).png"><br>
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    코드 앞부분
                </div>
            </td>
            <td>
                <div align="center">
                    코드 뒷부분
                </div>
            </td>
        </tr>
    </table>
</div>
<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image35(2).png"><br>
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    조종기 버저(음계) 블록
                </div>
            </td>
        </tr>
        <tr>
            <td>
        조종기의 버저로 설정한 음계를 재생할 때 사용합니다. 음계와 옥타브(1~8단계)를 선택할 수 있고, 재생 시간을 입력할 수 있습니다.재생이 완료 후에 다음 블록이 실행됩니다.
            </td>
        </tr>
    </table>
</div>

코드를 실행합니다. 훌륭한 연주가 되었나요? 다른 듣고 싶은 노래들도 코딩하여 멋지게 연주해봐요.

<br>

<h2> 2. 드론 LED 꾸며보기</h2>

<br>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image36(2).png"><br>
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    코드 앞부분
                </div>
            </td>
        </tr>
    </table>
</div>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image37(2).png"><br>
                    드론 LED 끄기 블록
                </div>
            </td>
            <td>
                <div align="left">
                    드론의 모든 LED(눈과 팔 부분)를 끌 때 사용합니다. 
                    LED를 끄지 않고 색상을 바꾸면 이전 색상과 색이 겹쳐지기 때문에 원하는 색상으로 바꿀 수 없습니다.
                    색상 겹침을 피하기 위해서는 꼭 LED를 먼저 끄고 색상을 변경합니다.
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image38(2).png"><br>
                    드론 LED 설정(RGB) 블록
                </div>
            </td>
            <td>
                <div align="left">
                    드론 눈/팔/눈+팔 부분 LED를 설정한 색상으로 켜고 끌 때 사용합니다.
                    색상은 Red, Green, Blue 중에서 선택 가능합니다.
                </div>
            </td>
        </tr>
    </table>
</div>
<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image40(2).png"><br>
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    코드 뒷부분
                </div>
            </td>
        </tr>
    </table>
</div>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image41(2).png"><br>
                    드론 LED 설정(색선택) 블록
                </div>
            </td>
            <td>
                <div align="left">
                    드론 눈/팔/눈+팔 부분 LED를 설정한 색상으로 켜고 끌 때 사용합니다. 
                    색상은 여러 가지 색상 중에서 선택 가능합니다. 
                    <font color="red">※ 의도보다 색상이 더 밝게 표현될 수 있습니다.</font>
                </div>
            </td>
        </tr>
    </table>
</div>
코드를 실행합니다. 드론의 LED 색상이 변하면서 비행하니까 더 멋있지 않나요? 좀 더 다양한 색상으로 드론을 예쁘게 꾸며봐요.

---

<br>


<div align="center">
    <h1>[정리하기]</h1>
</div>

<br>

눈과 귀가 즐거운 강의였나요? 이번 강의에서 배운 것을 활용하여 자신만의 음악을 만들어서 조종기로 연주해보고, 드론의 LED를 좀 더 화려하게 꾸며봐요.

1. 조종기의 Buzzer를 이용하여 음을 재생할 수 있습니다. (음계 선택 or 주파수)

2. 드론에는 눈과 팔 부분에 LED가 장착되어 있는데, 코딩으로 색상을 변경할 수 있습니다.

3. 드론의 LED 색상을 변경할 때, 이미 LED가 다른 색상으로 설정되어 있다면 색상이 겹쳐지기 때문에 꼭 LED를 먼저 끈 후 변경합니다.

<font color="red">※ 색상 겹침을 이용하여 특정 색상을 만들고 싶다면 LED를 끄지 않고 사용합니다.</font>


<br>

---

### [바이블럭으로 코딩해요](../)

 1. [페트론 V2와 바이블럭이 만났어요](../lesson1)
 2. [페트론 V2와 인사해요](../lesson2)
 3. **페트론 V2로 음악을 연주해요**
 4. [페트론 V2로 사각형을 그려보아요](../lesson4)
 5. [페트론 V2로 계단을 오르락내리락 해요](../lesson5)
 6. [페트론 V2를 원하는 높이로 상승시켜 보아요](../lesson6)
 7. [페트론 V2를 손바닥 위에 착륙시켜 보아요](../lesson7)
 8. [페트론 V2를 버튼으로 이륙/착륙시켜 보아요](../lesson8)

---

Modified : 2018.8.28