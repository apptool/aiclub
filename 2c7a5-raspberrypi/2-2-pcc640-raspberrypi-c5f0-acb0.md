# 2-2. PC와 RaspberryPi 연결

RaspberryPi에 인터넷을 연결한다.

LX Terminal을 실행 후 다음 명령어를 입력한다.

pi@raspberrypi ~ $ sudo raspi-config

Advanced Option &gt; A4 SSH &gt; Enable을 선택한다.

Finish를 눌러 다시 커맨드 창에서 다음 명령어를 입력한다.

pi@raspberrypi ~ $ ifconfig

유선 인터넷은 eth0, 무선 인터넷은 wlan0의 inet addr를 확인한다.



PC에서 접속 하실 수 있도록 PuTTY를 다음 링크에서 다운로드한다.

* [http://https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html](http://https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html)

![](/assets/import2-7.png)

다운로드 받은 파일을 실행한다.

PuTTY에서 RaspberryPi의 IP를 입력 후 Open 클릭.

![](/assets/import1-7.png)



