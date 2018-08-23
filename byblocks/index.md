---
layout: page
title: Byblocks
description: Byblocks
sitemap:
    priority: 0.7
    lastmod: 2018-8-23
    changefreq: weekly
---

파이썬 코드 테스트

```py
from time import sleep

from e_drone.drone import *
from e_drone.protocol import *


def eventAck(ack):
    print("eventAck() / {0} / 0x{1:04X} / {2}".format(ack.dataType.name, ack.crc16, ack.systemTime))


if __name__ == '__main__':

    drone = Drone()
    drone.open("COM22")


    # 이벤트 핸들링 함수 등록
    drone.setEventHandler(DataType.Ack, eventAck)
    sleep(0.01)


    drone.sendMotor(1000, 1200, 1300, 1400)
    sleep(1)

    drone.sendMotor(0, 0, 0, 0)
    sleep(0.1)


    drone.close()
```
