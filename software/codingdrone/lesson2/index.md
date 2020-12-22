<br>

<div align="center">
    <h1>Lesson 2. 코딩드론을 날려보아요</h1>
</div>

<br>

---

<br>


<div align="center">
    <h1>[들어가기]</h1>
</div>

<br>

이번 강의에서는 코딩드론 조종법을 배워보고 직접 날려보도록 해요.<br>
조종법을 배우기에 앞서 먼저 드론이 어떻게 비행을 하는지 비행 원리에 대해 알아보아요.<br>
드론은 어떻게 전후, 좌우로 비행하고 이착륙을 할까요? <Br>
드론의 비행 원리를 알기 위해서는 먼저 드론의 프로펠러가 어떻게 구성되어 있는지 알아야 합니다. 다음 그림을 보면서 알아볼까요?


<br>

<img src="images/image19.png" alt="코딩카드">

<br>

다음으로 드론이 어떻게 전진, 후진하고 회전 비행을 할 수 있는지 비행 원리에 대해 알아보아요.<Br>
드론의 비행 원리는 <font color="red"><b>각 모터의 속도를 조절하여 프로펠러의 회전 속도를 다르게 한다</font></b>는 사실만 알면 쉽게 이해할 수 있어요.

<Br>

<div align="center">
    <table>
        <tr>
            <td>
                <img src="images/image20.png">
            </td>
            <td>
                <img src="images/image21.png">
            </td>
        </tr>
        <tr>
            <td>
                <div align="left">모든 프로펠러를 같은 속도로 빠르게 회전시켜 큰 양력을 발생시키고, 양력이 중력보다 크게 되면 상승하게 됩니다. 이륙할 때에도 같은 방법으로 이륙하게 됩니다.</div>
            </td>
            <td>
                <div align="left">모든 프로펠러를 같은 속도로 느리게 회전시켜 양력을 감소시키고, 양력이 중력보다 작게 되면 하강하게 됩니다. 착륙할 때에도 같은 방법으로 착륙하게 됩니다.</div>
            </td>
        </tr>
        <tr>
            <td>
                <img src="images/image22.png">
            </td>
            <td>
                <img src="images/image23.png">
            </td>
        </tr>
        <tr>
            <td>
                <div align="left">3, 4번 프로펠러는 빠르게, 1, 2번 프로펠러는 상대적으로 느리게 회전시키면, 드론의 뒤쪽 양력이 더 커져 위로 들리면서 앞쪽으로 기울어집니다. 이때 앞쪽으로 추진력이 발생하여 전진하게 됩니다.</div>
            </td>
            <td>
                <div align="left">1, 2번 프로펠러는 빠르게, 3, 4번 프로펠러는 상대적으로 느리게 회전시키면, 드론의 앞쪽 양력이 더 커져 위로 들리면서 뒤쪽으로 기울어집니다. 이때 뒤쪽으로 추진력이 발생하여 후진하게 됩니다.</div>
            </td>
        </tr>
        <tr>
            <td>
                <img src="images/image24.png">
            </td>
            <td>
                <img src="images/image25.png">
            </td>
        </tr>
        <tr>
            <td>
                <div align="left">2, 3번 프로펠러는 빠르게, 1, 4번은 상대적으로 느리게 회전시키면, 드론의 오른쪽 양력이 더 커져 위로 들리면서 왼쪽으로 기울어집니다. 이때 왼쪽으로 추진력이 발생하여 좌로 이동하게 됩니다.</div>
            </td>
            <td>
                <div align="left">1, 4번 프로펠러는 빠르게, 2, 3번은 상대적으로 느리게 회전시키면, 드론의 왼쪽 양력이 더 커져 위로 들리면서 오른쪽으로 기울어집니다. 이때 오른쪽으로 추진력이 발생하여 우로 이동하게 됩니다.</div>
            </td>
        </tr>
        <tr>
            <td>
                <img src="images/image26.png">
            </td>
            <td>
                <img src="images/image27.png">
            </td>
        </tr>
        <tr>
            <td>
                <div align="left">1, 3번 프로펠러는 빠르게, 2, 4번은 상대적으로 느리게 회전시키면, 1, 3번(프로펠러가 시계 방향으로 회전)의 토크가 2, 4번보다 커져서 드론이 반시계 방향(좌)으로 회전하게 됩니다..</div>
            </td>
            <td>
                <div align="left">2, 4번 프로펠러는 빠르게, 1, 3번은 상대적으로 느리게 회전시키면, 2, 4번(프로펠러가 반시계 방향으로 회전)의 토크가 1, 3번보다 커져서 드론이 시계 방향(우)으로 회전하게 됩니다.</div>
            </td>
        </tr>
    </table>
</div>

<br>

<div align="center"><B>용어사전</b></div>
<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">양력</div>
            </td>
            <td>
                <div align="center">항공기가 공중에 뜰 수 있게 해주는 힘입니다.</div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">토크</div>
            </td>
            <td>
                <div align="center">회전하려는 힘으로서 기체는 프로펠러가 도는 방향과 반대로 회전하려는 성질이 있습니다.</div>
            </td>
        </tr>
    </table>
</div>

<br>

지금까지 드론이 어떻게 정해진 방향으로 비행할 수 있는지 비행 원리에 대해 알아보았어요.<br>
그럼 이제 코딩드론 조종법을 배워볼까요?<br>

<br>

---

<br>


<div align="center">
    <h1>[알아두기]</h1>
</div>

<br>

코딩드론 조종법에 대해 알아보아요. 드론의 조종모드는 4가지인데 코딩드론의 기본 조종모드는 모드2입니다.

<div align="center">
    <img src="images/image19.png" alt="이륙/착륙 예제 코드">
</div>

1) 카드코딩 실행 방법은 GoCar를 평평한 곳에 놓고 메인 전등 부분을 2번 연속으로 누르면 약 2~3초 후 부저음(띠리릭)이 울리면서 자동으로 실행됩니다.<br>
2) 한 번 입력된 코딩 명령은 메모리에 저장되어 계속 실행할 수 있습니다. 단, “코딩 시작” 카드를 다시 읽으면 초기화됩니다. <br>
<font color="red"><b>※ GoCar의 전원을 꺼도 저장되어 있습니다. (저장 가능한 최대 카드 개수 : 120장)</b></font>

<br>

---

<br>


<div align="center">
    <h1>[코드 생각하기]</h1>
</div>

<br>

지금부터는 직접 코딩해서 GoCar를 움직여 보기로 해요. <br>
먼저 코딩을 하기 전에 GoCar를 어떻게 움직일 것인지 생각하여 코드를 만들어봅니다.<Br>
이번 강의에서는 전진과 후진, 그리고 좌회전과 우회전을 해볼거예요. <br>
먼저 1칸 전진 후 1칸 후진을 하려면 어떻게 코드를 짜야 할지 생각해봅시다. <Br>
다음과 같이 코드를 생각해보았어요.


<h2>1. 전진/후진</h2>

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">동작 순서</div>
            </td>
            <td>
                <div align="center">시작 → 1칸 전진 → 1칸 후진 → 끝</div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">카드 순서</div>
            </td>
            <td>
                <img src="images/image20.png" alt="전진/후진">
            </td>
        </tr>
    </table>
</div>

<br>


<br>

<h2>2. 좌회전/우회전</h2>

<br>

다음으로 좌회전과 우회전을 한 번씩 번갈아서 동작하려면 코드를 어떻게 짜야할까요?<br>
방금 전에 전진과 후진 코드를 생각하면서 다음과 같이 코드를 생각해보았습니다.

<div align="center">
    <table>
        <tr>
            <td>
                <div align="center">동작 순서</div>
            </td>
            <td>
                <div align="center">시작 → 좌회전 → 우회전 → 끝</div>
            </td>
        </tr>
        <tr>
            <td>
                <div align="center">카드 순서</div>
            </td>
            <td>
                <img src="images/image21.png" height="304" width="866" alt="좌회전/우회전">
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

<h2>1. 전진/후진</h2>

<br>

이제 생각한 코드를 바탕으로 직접 코딩한 후 실행해보아요. <Br>위에서 배웠던 카드코딩하는 방법을 잊지 않았죠? 
<br>다음 순서대로 차근차근 따라해보세요.

<br>

<div align="center">
    <table>
        <tr>
            <td><br><div align="center"><b><h3>1단계 코딩카드 준비하기</h3><br></b></div></td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image22.png" alt="전진후진 1단계"><br>
                    카드코딩에 필요한 코딩카드들을 준비해보아요.
                </div>
            </td>
        </tr>
        <tr>
            <td><div align="center"><b><br><h3>2단계 코딩카드 배열하기</h3><br>
            동작순서 : 1칸 전진 → 1칸 후진<font color="red">(1칸 이동거리 : 약 13cm)<br><br></font></b></div></td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image23.png" height="304" width="1062" alt="전진후진 2단계"><br>
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
                    <img src="images/image24.png" height="304" width="1062" alt="전진후진 3단계"><br>
                    GoCar의 전원을 켜고 코딩카드를 읽습니다. <br>코딩카드가 잘 읽히도록 올바른 위치에 GoCar를 올려놓고 카드 순서대로 메인 전등 부분을 1번 눌러서 카드를 읽어주세요. <br>만약, 중간에 카드를 잘못 읽었다면 처음부터(=”코딩시작” 카드부터) 다시 시작합니다.<br><Br>
                    <font color="red"><b>※ “카드코딩 모드” 카드는 처음 한 번만 읽습니다!</b></font>
                </div>
            </td>
        </tr>
        <tr>
            <td><div align="center"><b><br><h3>4단계 코딩 실행하기</h3><br></b></div></td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image25.png" height="350" width="341" alt="전진후진 4단계1"><img src="images/image26.png" height="500" width="640" alt="전진후진 4단계2"><br>
                    GoCar를 평평한 바닥에 놓고 메인 전등 부분을 연속으로 2번 눌러서 코딩을 실행합니다. <br>약 3초 후 GoCar가 자동으로 코딩한 명령을 수행합니다. <br>GoCar가 잘 주행할 수 있도록 매끄럽고 평평한 바닥에서 실행해주세요.<br><br>
                    <font color="red"><b>※ 1칸 전진과 후진의 이동 거리는 약 <font color="blue">13cm</font>입니다.</b></font>
                </div>
            </td>
        </tr>
    </table>
</div>

<br>

<h2>2. 좌회전/우회전</h2>

<br>

다음으로 90도 좌회전 후 90도 우회전하는 코딩을 해보아요. <br>
전진과 후진 코딩과 동일한 방법으로 진행합니다.

<br>

<div align="center">
    <table>
        <tr>
            <td><div align="center"><b><br><h3>1단계 코딩카드 준비하기</h3><br></b></div></td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image27.png" height="310" width="969" alt="좌회전우회전 1단계"><br>
                    카드코딩에 필요한 코딩카드들을 준비해보아요.
                </div>
            </td>
        </tr>
        <tr>
            <td><div align="center"><b><br><h3>2단계 코딩카드 배열하기</h3><br><br>
            동작순서 : 90도 좌회전 → 90도 우회전<br><br></b></div></td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image28.png" height="310" width="1083" alt="좌회전우회전 2단계"><br>
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
                    <img src="images/image29.png" height="355" width="1083" alt="좌회전우회전 3단계"><br>
                    GoCar의 전원을 켜고 코딩카드를 읽습니다. <Br>코딩카드가 잘 읽히도록 올바른 위치에 GoCar를 올려놓고 카드 순서대로 메인 전등 부분을 1번 눌러서 카드를 읽어주세요. <Br>만약, 중간에 카드를 잘못 읽었다면 처음부터(=”코딩시작” 카드부터) 다시 시작합니다.<br><br>
                    <font color="red"><b>※ “카드코딩 모드” 카드는 처음 한 번만 읽습니다!</b></font>
                </div>
            </td>
        </tr>
        <tr>
            <td><div align="center"><b><br><h3>4단계 코딩 실행하기</h3><br></b></div></td>
        </tr>
        <tr>
            <td>
                <div align="center">
                    <img src="images/image25.png" height="350" width="341" alt="좌회전우회전 4단계1"><img src="images/image30.png" height="350" width="807" alt="좌회전우회전 4단계2"><br>
                    GoCar를 평평한 바닥에 놓고 메인 전등 부분을 연속으로 2번 눌러서 코딩을 실행합니다.<br>
                    약 3초 후 GoCar가 자동으로 코딩한 명령을 수행합니다. <br>
                    GoCar가 잘 주행할 수 있도록 매끄럽고 평평한 바닥에서 실행해주세요.<br>
                </div>
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

직접 코딩하여 GoCar를 움직여보니까 재미있었나요? <br>
전진과 후진, 좌회전과 우회전 명령어를 섞어서 사용하면 좀 더 다양한 주행을 할 수 있고, 출발지에서 도착지까지 찾아가는 길찾기 놀이도 할 수 있습니다.

1. GoCar로 총 43장의 카드를 읽어서 카드코딩을 할 수 있습니다.

2. 카드코딩 순서는 [코딩카드 준비하기 → 코딩카드 배열하기 → 코딩카드 읽기 → 코드 실행하기] 입니다.

3. 전진과 후진 카드를 사용하여 GoCar를 1칸 전진, 1칸 후진시킬 수 있습니다. 1칸 이동 거리는 약 13cm 입니다.

4. 90도 좌회전과 90도 우회전 카드를 사용하여 GoCar를 90도 좌회전, 90도 우회전시킬 수 있습니다.

5. 동일한 카드를 연속해서 사용하면 사용한 횟수만큼 이동하거나 회전합니다.<br>
   ex: 전진 카드를 3번 연속 읽으면 1칸씩 3번 전진하고, 90도 좌회전 카드를 2번 연속 읽으면 90도씩 2번 회전하여 총 180도를 회전합니다.


<br>

---

### [코딩카드로 자율주행해요](../)

 1. [GoCar와 친구해요!](../lesson1)
 2. **GoCar로 카드코딩해요(1)**
 3. [GoCar로 카드코딩해요(2)](../lesson3)
 4. [GoCar로 카드코딩해요(3)](../lesson4)
 5. [GoCar로 카드코딩해요(4)](../lesson5)
 6. [GoCar로 라인코딩해요](../lesson6)
 7. [GoCar로 모션코딩해요](../lesson7)
 8. [GoCar로 따라가기해요](../lesson8)


---

Modified : 2020.6.26