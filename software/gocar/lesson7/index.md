<br>

<div align="center">
    <h1>Lesson 7. GoCar로 모션코딩해요</h1>
</div>

<br>

---

<br>


<div align="center">
    <h1>[들어가기]</h1>
</div>

<br>

이번 강의에서는 GoCar로 3번째 언플러그드 코딩 기능인 모션코딩을 해보려고 합니다. <br>
먼저 모션코딩이 무엇인지 알아볼까요?



<br>


<div align="center">
    <table>
        <tr>
            <td>
                <div align="left"><b>모션코딩이란?</b></div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="left">☞	GoCar의 몸체를 기울여서 기울이는 방향에 따라 주행 명령을 입력할 수 있는 코딩 방식입니다. <br>
                주행 명령은 총 4가지로, 앞쪽으로 기울이면 1칸 전진, 뒤쪽으로 기울이면 1칸 후진, 왼쪽으로 기울이면 90도 좌회전, 오른쪽으로 기울이면 90도 우회전입니다. <br><br>
                ☞ GoCar에는 내부 메인보드에 <font color="red"><b>6축 자세센서</b></font>가 장착되어 있는데, 이 자세센서가 GoCar의 기울어진 방향과 각도를 측정할 수 있습니다.
                </div>
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
            <td colspan="2">
                <div align="center"><font color="red"><b>※ 6축 자세센서</b></font></div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center"><img src="images/image2.png">
                </div>
            </td>
            <td>
                <div align="left">
                ▶ 6축 자세센서는 3축 가속도 센서와 3축 자이로 센서로 구성되어 있습니다. 여기서 3축은 물체의 중심을 기준으로 X축(가로), Y축(세로), Z축(수직)을 말합니다.<br><br>
                ▶	가속도 센서는 각 축에 작용하는 중력가속도를 측정하여 현재 물체가 현재 어떤 방향으로 얼만큼 기울어져 있는지 확인할 수 있습니다.<br><Br>
                ▶	자이로 센서는 각 축에 작용하는 각속도(회전하는 각도의 변화량)를 측정하여 현재 물체가 어떤 방향으로 얼만큼 기울어져 있는지 확인할 수 있습니다.<br><br>
                ▶	가속도 센서와 자이로 센서는 사용 용도가 같지만 각 센서가 갖고 있는 단점들을 상호 보완하여 더욱 정밀한 측정을 할 수 있습니다.
                </div>
            </td>
        </tr>
    </table>
</div>

<br>

모션코딩이 무엇인지 알았나요? 이제 모션코딩으로 GoCar를 주행시켜보아요.

<Br>

---

<br>


<div align="center">
    <h1>[모션코딩 방법]</h1>
</div>

<br>

모션코딩은 다음 순서로 실시합니다.

<br>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center"><img src="images/image3.png"></div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center"><img src="images/image4.png"></div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="left">① 모션 인식시키는 방법은 GoCar를 손에 들고 평형을 유지한 상태에서, 각 명령에 맞게 GoCar를 기울였다가 다시 원위치 시키면 됩니다.<br>
                기울였을 때 부저음(띠딕)이 울리고, 다시 원위치 시켰을 때 부저음(띠)이 울리면 정상적으로 모션 명령이 입력된 것입니다.<br>
                <font color="red"><b>※ GoCar를 기울일 때 30도 이상 기울여주세요.</b></font>
                <br><Br>
                ② 모션코딩 실행 방법은 GoCar를 평평한 곳에 놓고 메인 전등 부분을 2번 연속으로 누르면 약 2~3초 후에 부저음(띠리릭)이 울리면서 자동으로 실행됩니다.<br><br>
                ③ 한 번 입력된 코딩 명령은 메모리에 저장되어 계속 실행할 수 있습니다. 단, GoCar의 전원이 꺼지거나 “코딩 시작” 카드를 다시 읽으면 초기화됩니다.<Br>
                </div>
            </td>
        </tr>
    </table>
</div>

<br>

---

<br>

<div align="center">
    <h1>[코딩 실행하기]</h1>
</div>

<br>

모션코딩으로 목적지 찾아가기 놀이를 해볼거예요. <Br>
먼저 아래와 같이 한 변의 길이가 13cm인 정사각형 9개를 그려서 실습판을 만들어주세요. <br>
그리기가 마땅치 않으면 정사각형 9개를 평평한 바닥에 붙여서 만들어도 괜찮아요. (컬러는 없어도 되고 가운데 숫자만 표시해주세요.)

<br>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">모션코딩 실습판</div>
            </td>
            <td>
                <div align="center">
                <img src="images/image5.png">
                </div>
            </td>
        </tr>
    </table>
</div>

<br>

<div align="center">
    <table>
        <tr>
            <td rowspan="6">
                <div align="center"><b>1단계</b>
                </div>
            </td>
            <td colspan="3"> 
                <div align="center"> <b>코딩 입력하기</b></div>
            </td>
        </tr>
        <tr>
            <td rowspan="4">
                <div align="center"><img src="images/image6.png"></div>
            </td>
            <td>
                <div align="center"> ① 1칸 전진하기 </div>
            </td>
            <td>
                <div align="center"> ② 90도 좌회전하기 </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center"><img src="images/image7.png">
                </div>
            </td>
            <td>
                <div align="center"><img src="images/image8.png">
                </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center"> ③ 1칸 전진하기 </div>
            </td>
            <td>
                <div align="center"> ④ 1칸 전진하기 </div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center"><img src="images/image7.png">
                </div>
            </td>
            <td>
                <div align="center"><img src="images/image7.png">
                </div>
            </td>
        </tr>
        <tr>
            <td colspan="3">
                <div align="left">
                    ① GoCar가 출발할 위치와 도착할 위치의 번호를 친구가 말해주면 어떻게 주행할지 생각합니다. (ex: 9번에서 출발하여 4번으로 가세요.)<br>
                    ② “모션코딩 모드” 카드와 “코딩 시작” 카드를 순서대로 읽고, 평형을 유지한 채 GoCar를 들어올려서 코딩 명령을 입력합니다.<br>
                    ③ 코딩 명령을 모두 입력시킨 후 “코딩 끝” 카드를 읽어서 코딩을 완료합니다.<br>
                </div>
            </td>
        </tr>
        <tr>
            <td rowspan="3">
                <div align="center"><b>2단계</b>
                </div>
            </td>
            <td colspan="3"> 
                <div align="center"> <b>코딩 실행하기</b></div>
            </td>
        </tr>
        <tr>
            <td colspan="3"> 
                <div align="center"> <img src="images/image9.png"></div>
            </td>
        </tr>
        <tr>
            <td colspan="3">
                <div align="left">
                    GoCar를 9번 위치에 올려놓고 메인 전등 부분을 연속으로 2번 눌러서 코딩을 실행합니다. 약 2~3초 후 GoCar가 자동으로 코딩한 명령을 수행합니다.<br> GoCar가 4번 위치까지 잘 이동하는지 확인하고, 만약 이동하지 않으면 어떤 부분이 잘못됐는지 확인하여 수정 후 재실행합니다.
                </div>
            </td>
        </tr>
   </table>
</div>

<br>

모션코딩으로 GoCar를 도착지까지 잘 이동시킬 수 있었나요? 출발지에서 도착지까지 가는 경로는 여러가지가 있습니다.<br>
 다른 경로도 모션코딩으로 주행해보아요. 그리고 친구들과 출발지와 도착지를 바꿔가면서 모션코딩 놀이를 즐겨보아요.

<br>

---

<br>

<div align="center">
    <h1>[정리하기]</h1>
</div>

<br>

이번 강의에서는 GoCar의 3번째 언플러그드 코딩 기능인 모션코딩을 해보았습니다. <Br>
모션코딩을 할 때, 센서가 GoCar의 기울어짐에 민감하기 때문에 평형을 잘 유지한 상태에서 정확한 방향으로 기울여야 합니다. 
<Br>그리고 카드코딩과 동일하게 코딩의 처음과 끝에 “코딩 시작”과 “코딩 끝” 카드를 읽어줘야 한다는 것을 잊지 마세요.



1. GoCar로 “모션코딩 모드” 카드를 읽으면 모션코딩 모드로 설정됩니다.

2. 모션코딩은 GoCar를 기울여서 코딩 명령을 입력할 수 있고, 코딩 명령은 총 4가지입니다.<Br>
    ☞ 앞쪽 : 1칸 전진 / 뒤쪽 : 1칸 후진 / 왼쪽 : 90도 좌회전 / 오른쪽 : 90도 우회전

3. GoCar의 내부 메인보드에 장착된 6축 자세센서가 GoCar의 기울어진 방향과 각도를 측정할 수 있습니다.


4. GoCar를 기울일 때, 30도 이상 기울여야 하고 다시 원위치로 돌아와야 정상적으로 코딩 명령이 입력됩니다.

<br>

---

### [코딩카드로 자율주행해요](../)

 1. [GoCar와 친구해요!](../lesson1)
 2. [GoCar로 카드코딩해요(1)](../lesson2)
 3. [GoCar로 카드코딩해요(2)](../lesson3)
 4. [GoCar로 카드코딩해요(3)](../lesson4)
 5. [GoCar로 카드코딩해요(4)](../lesson5)
 6. [GoCar로 라인코딩해요](../lesson6)
 7. **GoCar로 모션코딩해요**
 8. [GoCar로 따라가기해요](../lesson8)

---

Modified : 2020.7.16