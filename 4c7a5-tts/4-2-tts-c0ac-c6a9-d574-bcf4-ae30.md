# 4-2. TTS 사용해보기

> ###### \#-\*- coding:utf-8 -\*-
>
> ###### import os
>
> ###### import sys
>
> ###### import urllib.request 
>
> ###### client\_id = "YOUR\_CLIENT\_ID" 
>
> ###### client\_secret = "YOUR\_CLIENT\_SECRET" 
>
> ###### encText = urllib.parse.quote\("반갑습니다 네이버"\) 
>
> ###### data = "speaker=mijin&speed=0&text=" + encText; 
>
> ###### url = "https://openapi.naver.com/v1/voice/tts.bin" 
>
> ###### request = urllib.request.Request\(url\) 
>
> ###### request.add\_header\("X-Naver-Client-Id",client\_id\)
>
> ###### request.add\_header\("X-Naver-Client-Secret",client\_secret\) 
>
> ###### response = urllib.request.urlopen\(request, data=data.encode\('utf-8'\)\) rescode = response.getcode\(\) 
>
> ###### if\(rescode==200\):
>
> ######    print\("TTS mp3 저장"\)
>
> ######    response\_body = response.read\(\)
>
> ######    with open\('1111.mp3', 'wb'\) as f:
>
> ######        f.write\(response\_body\)
>
> ###### else:
>
> ######    print\("Error Code:" + rescode\)





