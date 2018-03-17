많은 python 사용자들은 anaconda를 이용해 package 와 dependencies 관리를 손쉽게 한다.
R의 경우에도 버전관리가 필요한 경우 conda로 가상환경을 만들어줘서 관리하는것을 권장한다.


Anaconda 설치
--------------------
1. [자신의 운영체제에 맞는 배포판을 설치한다.](https://www.anaconda.com/download/)
2. 환경변수에 `Anaconda3\Scripts` 추가


콘다에 R 설치하기
---------------
1. 새로운 conda 환경을 만들어준다. : `conda create -n <envname>`
2. r-essentials 혹은 r을 설치할 수 있다.
* r-essentials은 하나의 커맨드로 많이 사용되는 패키지를 모두 설치한다 : `conda install -c r r-essentials`
* r은 기본적인 패키지만 설치한다.: `conda install -c r r`


R studio 설치
----------------
R studio도 R을 설치한 동일한 환경안에 설치해줘야 한다.
[R studio의 버전관리 가이드](https://support.rstudio.com/hc/en-us/articles/200486138-Using-Different-Versions-of-R)에서 설명하는 
interpreter 설정 방법은 conda에 설치한 경우엔 잘 되지 않는다.

```
activate <envname>
conda install -c r rstudiio
```
