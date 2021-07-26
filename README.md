자가진단 매크로
=============
> ???: 가상 키패드를 적용하면 자가진단 매크로를 막을 수 있습니다.

가상 키패드에 대응 가능한 자가진단 매크로입니다!

자가진단 사이트가 업데이트될 때마다 지속적으로 수정할 예정입니다!

사용 전 준비
-------------
> https://www.python.org/downloads/

위 링크에서 python 최신버전을 다운로드해 설치해주세요.(설치할 때 ADD Python 3.9 to PATH 항목을 꼭 체크해주셔야 합니다)

설치가 완료되었다면 cmd를 켜고 pip install selenium를 입력해 설치가 완료될 때까지 기다려주세요.

> https://sites.google.com/a/chromium.org/chromedriver/downloads

위 링크에서 본인의 크롬 버전과 OS에 맞는 웹드라이버를 다운로드해주세요.

(크롬 버전 확인은 chrome://version에서 가능합니다)

이후 py파일 내에서 개인정보 및 파일 경로 등을 본인에게 맞게 수정하셔야 합니다.

(프로그램 오류로 인해 상대경로가 아닌 절대경로로 수정해주셔야 합니다.)

이후 SelfDiagnosisMacro.py를 실행해주시면 됩니다!

기타사항
-------------
> https://github.com/SaidBySolo/auto-self-diagnosis

위 코드를 일부 참고했습니다!

현재는 유·초·중·고 자가진단만 제공하지만, 향후 다른 자가진단도 제공할 계획입니다!

쿠키의 경우 유지하게 프로그램을 짰습니다.

만약 이를 유지하고 싶지 않으시다면 py파일 내 주석으로 있는 아래의 4줄을 주석에서 풀어주면 됩니다.

```py
try:
    shutil.rmtree(chromeTemp)
except FileNotFoundError:
    pass
```
